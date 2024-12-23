### 0.0.32
This is just a love tribute to Siggi.  
The dark `signavio` theme has a bold reference to her ❤️

### 0.0.30
Menu rearranged and cleaned up a bit.

### 0.0.29
Added notifications when coping to clipboard with y or m;
DMG avaialbe only for arm64 (Apple Silicon) from now on.

### 0.0.28  
added a utility shortcut function `console.json` simply defined as:  
``` js
console.json = j => console.log(JSON.stringify(j, null, 2))
```

### 0.0.27  
now is possible to create a bookmarklet (will be copied in the clipboard) just using the keyboard shortcut ` + y` or the right new option in the _edit_ menu. 

### 0.0.26  
the previous version feature _copy as markdown Details tag_ was missing a keyboard short cut ` + m`  

### 0.0.25  
- the _edit_ menu contains a new option labelled  _copy as markdown Details tag_ which when triggered copies in the clipboard a markdown friendly `<Details>+<Summary>` expandable tag containing the code in the editor.  
    An example follows, you get always a free :icecream: wrapping your code:
    <details>
    <summary>free :icecream:</summary>

    ``` js  
    var uniqueID = new function () {
        var count = 0,
            self = this;
        this.prefix = 'NS_';
        this.toString = function () {
            count += 1;
            return self.prefix + count;
        };
    }
    ```
    </details>

    when u need to indent the whole thing be sure to select the whole clipboard pased content and indent/ unindent the whole.

### 0.0.24  
- Fix a small bug related to 'save as' and the 'recents' list  
### 0.0.23  
- Allow to open json and jsx files  
### 0.0.22  
- Fixed a minor bug not allowing all recents to be selectable when +n is used  
### 0.0.21  
- Solved a minor issue that was throwing an error when the main window is closed and one of the shortcuts get triggered  
### 0.0.20
- Some minor refactor and hide the preferences panel which is not ready to be shipped, some small bug fixes
### 0.0.17 
- Fix a small bug about 'recent files' when starting
### 0.0.16 
- _Open recents_ submenu added to the _File_ menu (up to 20 items)
### 0.0.15 
- disable some not fitting options from output codemirror instance

### 0.0.14 
- better internal setting separation (groundfield for the setting panel)
- exploit most of the codemirror shipped addons:
    - sublime bindings
    - js linter (es9)
    - js hint (alt + space)
    - code folding
    - auto close brakets
    - brakets match highlight
    - comment toggle shortcuts ( + /)

### 0.0.13 
- just updated electron

### 0.0.12 
- fixed a bug preventing the possibility to require relative files
### 0.0.11 
- fixed a bug preventing errors to show after `console.log` gets called

### 0.0.10 
- `NODE_PATH` now correctly points to `~/node_modules` thus now (once for all) all modules in that folder can be successfully required and used

### 0.0.9
- `require` now really starts from the search in your home dir (`process.env.NODE_PATH = os.homedir()`)
- at least theme choice is persistent; the preference panel is WIP
- dark jshero theme added (default)

### 0.0.8
- better console.log
- better spinner on execution

### 0.0.7
- browser context is separated (in 0.0.6 `window` was the app one 👎 )
- a webview can be toggled using +b; `window` will reference its BOM context
- to use the webview first toggle it on and then execute the script

### 0.0.6
- all BOM should be also accessible

### 0.0.5
- upper right save status
- way better fork, use freely `console.log` for output

### 0.0.4
- open, save, save as in menu, some refactoring + cleanup
### 0.0.3
- codemirror used in editor and output (readonly); this means the theme applies to both sides
- the header have some enhancements, double click on it to maximize the window