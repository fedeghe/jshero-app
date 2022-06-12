# js hero
![jshero](https://raw.githubusercontent.com/fedeghe/jshero-app/master/jsheroIcon.png)

Experimental js console for  ([why?](https://github.com/fedeghe/jshero-app/blob/master/WHY.md))

This app is under development, for fun, still there are a lot of limitations, among which, but not limited to the following:
- requires node installed
- there's no code assistance neither transpilation
- if u see the _herojs_ central spinner for unexpectedly too long, quit and restart (the script can anyway be found on `/Applications/jshero.app/Contents/Resources/app/.webpack/main/native_modules/jsheroScript.js`); I still could not reproduce it exactly, thus I do not know the cause (only happens in the shipped app, not in the dev one). If happens and you have some time/love to give back then please file an issue on github putting as much informations as possible for me to try reproduce & fix it 👍  
- (BOM) `window.fetch` is blocked (cors) .... I still have to find the time to find a solution. Heeeeelp me plz!!!

...what should work properly:
- `console.log` is the way to get some output
- all global modules are accessible with CommonJS (`require`) from your home directory (since 0.0.9).
- double click on the top bar to maximize the window (ok ...not exactly a feature 🤦 )
- choose among many _light_ & _dark_ themes (all those shipped with [codemirror](https://codemirror.net/) + x)
- shortcuts:
    - ` + r`: execute the current script
    - ` + backspace`: reset the current script content. 
    - ` + n`: clear the content and forget about the current file if any.
    - ` + o`: open an existing file selecting from your filesystem 
    - ` + s`: save the current script
    - ` + shift + s`: save a copy of the current script naming it as you want
    - ` + b`: toggles on/off the webview
    - plus all sublime bindings
 - about the webview:
    - in yout script `window` will refer exactly to the webview global scope, some limitations (how can I be so confident _cors_ is not the only one ?)
    - first toggle the webview on, then execute the script

There are other problems but to some extent it is usable and will get better soon 👍

So in the end ... **do not use it for "real"** ...but but but please **consider** to **help me** in case you see something **between those confused lines**.




[download latest version (0.0.21)](https://github.com/fedeghe/jshero-app/raw/master/versions/jshero-0.0.21-x64.dmg)  

[changelog](https://github.com/fedeghe/jshero-app/blob/master/CHANGELOG.md)  


![a screenshot](https://raw.githubusercontent.com/fedeghe/jshero-app/master/jshero.png "jsHero")
![a screenshot](https://raw.githubusercontent.com/fedeghe/jshero-app/master/jsheroB.png "jsHero")