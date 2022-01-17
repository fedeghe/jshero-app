### 0.0.3
- codemirror used in editor and output (readonly); this means the theme applies to both sides
- the header have some enhancements, double click on it to maximize the window

### 0.0.4
- open, save, save as in menu, some refactoring + cleanup

### 0.0.5
- upper right save status
- way better fork, use freely `console.log` for output

### 0.0.6
- all BOM should be also accessible

### 0.0.7
- browser context is separated (in 0.0.6 `window` was the app one 👎 )
- a webview can be toggled using +b; `window` will reference its BOM context
- to use the webview first toggle it on and then execute the script