# FluffyLabsConfigManagerTools

This is a library which extends the functionality of BepInEx.ConfigurationManager

## Setup For Users

This on its own is not a mod but a library which other mods can use to help make different configuration formats.

If you are using any mods which depend on this then you will need to have this mod installed along with any dependencies it has.

To install all you will need to do is download this mod and put `FluffyLabsConfigManagerTools.dll` and `ConfigurationManager.dll` (from Bepinex.ConfigurationManager dependency) put into your `Bepinex/plugins` folder.

## Setup For Developers

Add `FluffyLabsConfigManagerTools.dll` as a reference to your plugin project. If you do not know how to do this then consult [documentation](https://docs.microsoft.com/en-us/visualstudio/ide/how-to-add-or-remove-references-by-using-the-reference-manager?view=vs-2019)

Once you have added the reference correctly you will have access to {FluffyLabsConfigManagerTools} namespace.

At the top of your BepInPlugin .cs file you will need to add the following using statements:
- `using FluffyLabsConfigManagerTools.Util;`
This namespace gives you access to utilities which make it easier for you to add the custom configuration types (e.g. `ButtonUtil`)

- `using FluffyLabsConfigManagerTools.Infrastructure;`
This namespace gives you access to the classes and structs which hold the types you will need in your custom ConfigEntry (e.g. `Conditional<T>`)

To enable XML comments intellisense be sure to leave `FluffyLabsConfigManagerTools.xml` in the same install location as `FluffyLabsConfigManagerTools.dll`

Don't forget to add the attribute at the top of your plugin `[PluginDependency(FluffyLabsConfigManagerTools.FluffyConfigLabsPlugin.PluginGuid)]` to register this dependency for the chainloader.

## Utilities

The most useful way to use this lib is through the utilities. The following is a quick summary of what there is and how it is used.

Note: All utilities have XML comments so should show intellisense when you use them in Visual Studio.

### ButtonUtil
Adds a button configuration with customisable Action

Example:
```csharp
public class FluffyLabsTest : BaseUnityPlugin
{
	public void Awake()
	{
		var buttonUtil = new ButtonUtil(this);
		buttonUtil.AddButtonConfig("Button", "Button", "Describe this button", GetDic());        
	}

	private Dictionary<string, Action> GetDic()
	{
		return new Dictionary<string, Action>
			{
				{ "Button01",  () => Debug.Log("Button 1 press") },
				{ "Button02",  () => Debug.Log("Button 2 press") },
				{ "Button03",  Example }
			};
	}

	private void Example()
	{
		Debug.Log("Button 3 press");
	}
}
```

### ConditionalUtil
Adds a configuration which has a value and can be enabled/disabled

Example:
```csharp
public class FluffyLabsTest : BaseUnityPlugin
{
    private ConditionalConfigEntry<float> FloatConfig;
    private ConditionalConfigEntry<int> IntConfig;
    private ConditionalConfigEntry<double> DoubleConfig;

	public void Awake()
	{
		const string conditionalSectionName = "Conditional";

        var conditionUtil = new ConditionalUtil(this);
		FloatConfig = conditionUtil.AddConditionalConfig<float>(
			conditionalSectionName,
            "Float", 
            0.5f, 
            false, 
            new ConfigDescription("This is float"));

        IntConfig = conditionUtil.AddConditionalConfig<int>(
            conditionalSectionName,
            "Integer", 
            0, 
            false, 
            new ConfigDescription("This is int"));

        DoubleConfig = conditionUtil.AddConditionalConfig<double>(
            conditionalSectionName,
            "Double", 
            6.789, 
            true, 
            new ConfigDescription("This is double"));
	}
}   
```

### MacroUtil
Adds a configuration specifically designed for adding a macro configuration

Example:
```csharp
public class FluffyLabsTest : BaseUnityPlugin
{
    private MacroConfigEntry MyMacro1;
    private MacroConfigEntry MyMacro2;
    private MacroConfigEntry MyMacro3;
       
    public void Awake()
    {
        const string macroSectionName = "Macro";

        var macroUtil = new MacroUtil(this);
        MyMacro1 = macroUtil.AddMacroConfig(macroSectionName, "macro 1", "description", false);
        MyMacro2 = macroUtil.AddMacroConfig(macroSectionName, "macro 2", "description", false);
        MyMacro3 = macroUtil.AddMacroConfig(macroSectionName, "macro 3", "description", true);
    }
}   
```

### Combined example

The following is an example showing a mixture of the utils together.

```
    public class FluffyLabsTest : BaseUnityPlugin
    {
        private ConditionalConfigEntry<int> ConditionalConf;
        private MacroConfigEntry MacroConf;

        public void Awake()
        {
            var cUtil = new ConditionalUtil(this);
            ConditionalConf = cUtil.AddConditionalConfig<int>("con", "con", 5, true, new ConfigDescription("desc"));

            var bUtil = new ButtonUtil(this);
            bUtil.AddButtonConfig("Button", "button", "description", GetDic());

            var mUtil = new MacroUtil(this);
            MacroConf = mUtil.AddMacroConfig("Macro", "Macro", "Description", false);
        }
        
        private Dictionary<string, Action> GetDic()
        {
            return new Dictionary<string, Action>
            {
                { "button", () => { Debug.Log("Button action" } }
            };
        }
    }   
```

## Contact

If you have any issues you can usually find me on the ROR2 modding discord (@Fluffatron). Please bear in mind that as with all mods here this is something I do in my spare time so may not always be able to immediately fix any issues that you come up with. 

## Changelog

v1.0.1
- Added public constant PluginGuid for dependency reference

v1.0.0
- Released