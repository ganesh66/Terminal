# ColorTool - colortool.exe

```
Usage:
    colortool.exe [options] <schemename>
ColorTool is a utility for helping to set the color palette of the Windows Console.
By default, applies the colors in the specified .itermcolors or .ini file to the current console window.
This does NOT save the properties automatically. For that, you'll need to open the properties sheet and hit "Ok".
Included should be a `schemes/` directory with a selection of schemes of both formats for examples.
Feel free to add your own prefered scheme to that directory.
Arguments:
    <schemename>: The name of a color scheme. ct will try to first load it as an .itermcolors color scheme.
                  If that fails, it will look for it as an .ini file color scheme.
Options:
    -?, --help     : Display this help message
    -c, --current  : Print the color table for the currently applied scheme
    -q, --quiet    : Don't print the color table after applying
    -d, --defaults : Apply the scheme to only the defaults in the registry
    -b, --both     : Apply the scheme to both the current console and the defaults.
    -v, --version  : Display the version number
```

## Included Schemes

  Included are two important color schemes in .ini file format - `cmd-legacy` and `campbell`.

  * `cmd-legacy` is the legacy color scheme of the Windows Console, before July 2017
    
  * `campbell` is the new default scheme used by the Windows Console Host, as of the Fall Creator's Update.

  There are a few other schemes in that directory in both .ini format and .itermcolors. 

## Adding Schemes

  You can also add color schemes to the colortool easily. Take any existing scheme in `.itemcolors` format, and paste it in the `schemes/` directory.

  I recommend the excellent [iTerm2-Color-Schemes](https://github.com/mbadolato/iTerm2-Color-Schemes) repo, which has TONS of schemes to chose from, and previews.

## Building

  Either build with Visual Studio, or use the included `build.bat` from the commandline to try and auto-detect your msbuild version.

## Contributing

  This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.