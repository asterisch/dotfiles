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
Finally copy the dark markdown rendering theme:
```
cp github-markdown-dark.css ~/Library/Application\ Support/Sublime\ Text/
```

### Note
`MarkdownPreview` plugin uses github/gitlab API to convert your
markdown to html which means that it may upload your markdown online!!

With the above setting the rendering is done offline according to
documentation: 
https://github.com/facelessuser/MarkdownPreview/
https://facelessuser.github.io/MarkdownPreview/usage/#offline
