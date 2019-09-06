# stencil-xclangspec

Xcode syntax highlighting for [Stencil](https://stencil.fuller.li)

This is fairly naive and not as complete as the [Stencil-provided](https://github.com/stencilproject) syntax highlighting for other editors. The xclangspec format is not documented and so is based on other existing examples.

## Supported Xcode Versions

Xcode will only attempt to load an .ideplugin if its Info.plist contains a UUID that matches the DVTPlugInCompatibilityUUID value in the Xcode's Info.plist. This UUID changes with each version of Xcode, so plugin authors need to keep adding UUIDs for each new Xcode that's released. This plugin should support recent Xcode versions up to 10.3.

Xcode 11 doesn't seem to support user-installed .xclangspecs, even though it loads the .ideplugin and supports the defined filetype, so this plugin won't support those versions.

## Resources

- [Adding syntax highlighting and source file support for TypeScript to Xcode — Erica Sadun](https://ericasadun.com/2018/12/17/adding-syntax-highlighting-and-source-file-support-for-typescript-to-xcode/)
- [GitHub - erica/TypeScript-xclangspec: A langspec-ish thing for Daniel](https://github.com/erica/TypeScript-xclangspec)
- [d-for-xcode/d.xclangspec at master · michelf/d-for-xcode · GitHub](https://github.com/michelf/d-for-xcode/blob/master/Resources/d.xclangspec)
- `/Applications/Xcode.app/Contents/SharedFrameworks/DVTFoundation.framework/Versions/A/Resources/*.xclangspec`
