# Sublime Text 4 - Custom settings

### Required packages (⌘ + ⇧ + P) "Advanced Install Package"

---
AlignTab, 
ChangeQuotes, 
Color Highlight,
ColorPicker,
CommandsBrowser, 
Compare Side-By-Side,
Default File Type, 
GitGutter, 
JSON Key-Value,
Kotlin, 
Multicommand, 
Pretty JSON, 
RainbowBrackets, 
RegReplace, 
SideBarEnhancements, 
SublimeLinter,
Terminal, 
Theme - One,
UnicodeMath, 
url-utils, 
WordCount, 
WordHighlight,

SublimeLinter-javac, 
SublimeLinter-jshint, 
SublimeLinter-json, 
SublimeLinter-mdl, 
SublimeLinter-xmllint

---
### Settings
```bash
cd ~/Library/Application\ Support/Sublime\ Text/Packages/User/ && \
curl -LJO https://github.com/liviolopez/sublime-text-settings/raw/master/settings/sublime-settings.zip && \
unzip sublime-settings.zip && rm sublime-settings.zip

# Download a single settings file
# curl -LJO https://raw.githubusercontent.com/liviolopez/sublime-text-settings/master/settings/Main.sublime-menu
```
### Quick Actions
```bash
cd ~/Library/Services/ && \
curl -LJO https://github.com/liviolopez/sublime-text-settings/raw/master/quick-actions/sublime-quick-actions.zip && \
unzip sublime-quick-actions.zip && rm sublime-quick-actions.zip
```
Right-click any directory, choose _**Quick Actions ⇨ Customize**_ and check sublime's actions, then close the window

---
### Check command syntax
1. Open sublime console: View ⇨ Show Console
2. Set log debug to true. execute on the console: ```sublime.log_commands(True)```

### Check installed packages
```bash
subl ~/Library/Application\ Support/Sublime\ Text/Packages/User/Package\ Control.sublime-settings
```
---
### Associate all code files with Sublime
https://alexpeattie.com/blog/associate-source-code-files-with-editor-in-macos-using-duti/
```bash
brew install duti python python-yq
```
```bash
curl "https://raw.githubusercontent.com/github/linguist/master/lib/linguist/languages.yml" \
  | yq -r "to_entries | (map(.value.extensions) | flatten) - [null] | unique | .[]" \
  | xargs -L 1 -I "{}" duti -s com.sublimetext.4 {} all
```
---

## Required packages
| Package                                                                           |                                                                                                                                               |
|-----------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
| [AlignTab](https://packagecontrol.io/packages/AlignTab)                           |                                                                                                                                               |  
| [ChangeQuotes](https://packagecontrol.io/packages/ChangeQuotes)                   |                                                                                                                                               |  
| [Color Highlight](https://packagecontrol.io/packages/Color%20Highlight)           |                                                                                                                                               |  
| [ColorPicker](https://packagecontrol.io/packages/ColorPicker)                     |                                                                                                                                               |  
| [CommandsBrowser](https://packagecontrol.io/packages/CommandsBrowser)             |                                                                                                                                               |  
| [Compare Side-By-Side](https://packagecontrol.io/packages/Compare%20Side-By-Side) |                                                                                                                                               |  
| [Default File Type](https://packagecontrol.io/packages/Default%20File%20Type)     |                                                                                                                                               |  
| [GitGutter](https://packagecontrol.io/packages/GitGutter)                         |                                                                                                                                               |  
| [JSON Key-Value](https://packagecontrol.io/packages/JSON%20Key-Value)             |                                                                                                                                               |  
| [Kotlin](https://packagecontrol.io/packages/Kotlin)                               |                                                                                                                                               |  
| [Multicommand](https://packagecontrol.io/packages/Multicommand)                   |                                                                                                                                               |  
| [Pretty JSON](https://packagecontrol.io/packages/Pretty%20JSON)                   |                                                                                                                                               |  
| [RainbowBrackets](https://packagecontrol.io/packages/RainbowBrackets)             |                                                                                                                                               |  
| [RegReplace](https://packagecontrol.io/packages/RegReplace)                       |                                                                                                                                               |  
| [SideBarEnhancements](https://packagecontrol.io/packages/SideBarEnhancements)     |                                                                                                                                               |  
| [Terminal](https://packagecontrol.io/packages/Terminal)                           |                                                                                                                                               |  
| [Theme - One](https://packagecontrol.io/packages/Theme%20-%20One)                 |                                                                                                                                               |  
| [UnicodeMath](https://packagecontrol.io/packages/UnicodeMath)                     | [Emoji](https://github.com/mvoidex/UnicodeMath/blob/master/emoji.md) - [Symbols](https://github.com/mvoidex/UnicodeMath/blob/master/table.md) |
| [url-utils](https://packagecontrol.io/packages/url-utils)                         |                                                                                                                                               |  
| [WordCount](https://packagecontrol.io/packages/WordCount)                         |                                                                                                                                               |  
| [WordHighlight](https://packagecontrol.io/packages/WordHighlight)                 |                                                                                                                                               |                   

