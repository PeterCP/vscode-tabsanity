# TabSanity for Visual Studio Code

Navigate or modify soft tabs as if they were hard tabs.

[![Build Status](https://travis-ci.org/jedmao/vscode-tabsanity.svg?branch=master)](https://travis-ci.org/jedmao/vscode-tabsanity)

<img src="https://github.com/jedmao/vscode-tabsanity/blob/master/images/demo.gif?raw=true" width="384" height="170" alt="TabSanity Demo">

## Supported features

- The cursor moves `tabSize` spaces:
	- If the cursor is detected to be within indentation range.
		- Left/right arrow-key navigation or selection is performed.
		- Backspace or delete key operations are performed.
- The cursor moves by only one space:
	- If the cursor is detected to be within alignment range.
	- Or the cursor is detected to be outside of indentation range.
- Multiple cursors.

_Pro Tip: In lieu of the `tabSize` setting being read for this extension, it is strongly recommended that you also install the [`EditorConfig`][] extension to ensure that the correct `tabSize` setting is being applied per file. Visit [editorconfig.org](http://editorconfig.org/) to learn more about the project._

## On the backlog

- Look into code coverage solutions that are compatible with TypeScript.

## Known issues

- Too many commands seem to be undone in a single undo command (requires research).
- There are no plans to support mixed tabs and spaces within the range of indentation.
	- It is perfectly acceptable to have tabs for indentation and spaces that follow for alignment and is not considered mixing tabs with spaces.

## Related extensions

- [`EditorConfig`][]
- [`backspace-plusplus`][]


[`EditorConfig`]: https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig
[`backspace-plusplus`]: https://marketplace.visualstudio.com/items?itemName=jrieken.backspace-plusplus
