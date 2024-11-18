# js hero
![jshero](https://raw.githubusercontent.com/fedeghe/jshero-app/master/jsheroIcon.png)

Experimental js console for  ([why?](https://github.com/fedeghe/jshero-app/blob/master/WHY.md))

This app is under development, for fun, still there are a lot of limitations, among which, but not limited to the following:
- requires node installed
- there's no code assistance neither transpilation
- if u see the _herojs_ central spinner for unexpectedly too long, quit and restart (the script content u were editing can anyway be found on `/Applications/jshero.app/Contents/Resources/app/.webpack/main/native_modules/jsheroScript.js`); I still could not reproduce it exactly, thus I do not know the cause (only happens in the shipped app, not in the dev one). If happens and you have some time/love to give back then please file an issue on github putting as much informations as possible for me to try reproduce & fix it 👍  
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
    - ` + b`: toggle on/off the webview
    - ` + m`: create & copy the code in the clipboard as a `<details>` markdown friendly snippet
    - ` + y`: create & copy to the clipboard a bookmarklet which executes the code in the editor
    - plus all sublime bindings
 - about the webview:
    - in your script `window` will refer exactly to the webview global scope, some limitations (e.g. _cors_)
    - first toggle the webview on, then execute the script

There are other problems but to some extent it is usable and will get better soon 👍





download
- [the latest version (0.0.32) jshero.0.0.32.zip (https://github.com/fedeghe/jshero-app/raw/master/versions/jshero.0.0.32.zip)  

- [one of the previous .dmg installer - only x64](https://github.com/fedeghe/jshero-app/raw/master/versions/)  


# if you download the app

this is the only available option from version >= 0.0.32  
and it is only compatible with `darwin-arm64` architecture.  
Download the `.zip` file, uncompress it and move the resulting `.app` in the `applications` folder.

# if you download the installer

After downloading be sure to open just the first time as follows:  

![a screenshot](https://raw.githubusercontent.com/fedeghe/jshero-app/master/img/o1.png "jsHero")  


then click open (might happen that the _open_ button is not visible, in that case discard and try another time from the contextual menu open it)    


![a screenshot](https://raw.githubusercontent.com/fedeghe/jshero-app/master/img/o2.jpeg "jsHero")

---

![a screenshot](https://raw.githubusercontent.com/fedeghe/jshero-app/master/jshero.png "jsHero")

---

![a screenshot](https://raw.githubusercontent.com/fedeghe/jshero-app/master/jsheroB.png "jsHero")