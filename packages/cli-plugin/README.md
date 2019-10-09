## Usage

The cli-plugin allows users to work with the command line interface for their web applications. 
 
Features for this plugin include: 

1) Configurable commands
2) Configurable Color Schemes
3) History of used commands 

```

## How to install with npm

npm install cli-plugin
```

## Setup

Initialize cliPlugin using a custom colorscheme/config file.

cliPlugin.init(config);
```
Initialize cliPlugin using a custom colorscheme/config file.

cliPlugin.init(config);
Config accepts following properties:

Property	Usage	Default	Required
textColor	text color	#111111	no
cursorColor	cursor color	#111111	no
backgroundColor	background color	whitesmoke	no

Register commands
Register your own commands:

cliPlugin.bind('list', function () {
  cliPlugin.print('<p>items on the shopping list:</p>');
  cliPlugin.print('<ul><li>milk</li><li>bacon</li><li>eggs</li></ul>');
});
Useful functions
Use cliPlugin.print(text) command to print text on the screen, accepts html.

Use cliPlugin.clear() command to clear the screen.
