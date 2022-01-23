### 1
Copy setting, keymaps and MarkdownPreview plugin settings to sublime
text folder:
```
_SBLTXT=~/Library/Application\ Support/Sublime\ Text/Packages/User/
cp settings/* "${_SBLTXT}"
```

### 2
Then install the packages listed in `installed_packages.txt`.

### 3
Install the custom `MarkdownPreview`:
```
cp MarkdownPreviewPlugin/MarkdownPreview.sublime-package ~/Library/Application\ Support/Sublime\ Text/Installed\ Packages/
```

(Optional) Create the sublime package zip from the custom
`MarkdownPreview` source code that only uses offline markdown
rendring.
```
zip -r ../MarkdownPreview.sublime-package .
```

### 4
Finally copy the dark markdown rendering theme:
```
cp github-markdown-dark.css ~/Library/Application\ Support/Sublime\ Text/
```

### Note
*DO NOT INSTALL*: `MarkdownPreview` from github.com/facelessuser MarkdownPreview
The plugin BY DEFAULT uses github/gitlab API to convert your
markdown to html which means that it uploads your markdown online!!
My settings above just ensure offline rendering in case you
accidentally install it...
