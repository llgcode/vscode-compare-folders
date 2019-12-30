[![Build Status](https://dev.azure.com/moshfeu-vscode/CompareFoldersExtension/_apis/build/status/moshfeu.vscode-compare-folders?branchName=master)](https://dev.azure.com/moshfeu-vscode/CompareFoldersExtension/_build/latest?definitionId=1&branchName=master)

The extension allows the user to compare folders, show the diffs in a list and present diff in a splitted view side by side.

![screen record](https://user-images.githubusercontent.com/3723951/71602305-751e5b80-2b60-11ea-8525-800129a7c748.gif)

### Notice
- The extension works only when the vscode instance has one workspace (or one folder) or more. It's not working for [empty workspace](https://user-images.githubusercontent.com/3723951/70967746-d560c800-209f-11ea-8148-12c5251b00ea.png).

- The extension shows only differences in files at the same path with different content. For example:

```
folderA/file.txt
folderB/file.txt
```

It will not show differences in

```
folderA/file.txt
folderB/folderA/file.txt
```

In this case, the extension will show a message that it couldn't find any changes

You can find the series of the posts about how this extension developed step by step in [medium.com](https://medium.com/@moshfeu/comparefolders-visual-studio-code-extension-journey-intro-b540a0539629?source=friends_link&sk=db37e1889766ccd8fe553958a12a8f69).

## Change log

**0.4.0**

Show missing/additional files [#9](https://github.com/moshfeu/vscode-compare-folders/issues/9) (Thanks to [@fbaligand](https://github.com/fbaligand))

<img width="334" alt="missing/additional files screenshot" src="https://user-images.githubusercontent.com/3723951/71563330-90bd2f80-2a96-11ea-91b3-e2f531f2f74d.png">

**0.3.0**

Support multiple workspaces

<img width="496" alt="Multiple workspaces screenshot" src="https://user-images.githubusercontent.com/3723951/71128162-44036a00-21f5-11ea-88fe-9c2519b8a2e8.png">

**0.2.0**
- Improve UI: [#5](https://github.com/moshfeu/vscode-compare-folders/issues/5), [#6](https://github.com/moshfeu/vscode-compare-folders/issues/6), [#7](https://github.com/moshfeu/vscode-compare-folders/issues/7) thanks to [@gjsjohnmurray](https://github.com/gjsjohnmurray)
- Supports dark mode!


## Credits
Activity bar's icon (and more) by [Stockio.com](https://www.stockio.com/free-icon/folders)
Null icon made from <a href="http://www.onlinewebfonts.com/icon">Icon Fonts</a> is licensed by CC BY 3.0
External link icon made by <a href="https://www.flaticon.com/authors/dave-gandy" title="Dave Gandy">Dave Gandy</a> from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a>