# js hero
![jshero](https://raw.githubusercontent.com/fedeghe/jshero-app/master/jsheroIcon.png)

Experimental js console for 

This app is under development, for fun, still there are a lot of limitations, among which, but not limited to the following:
- requires node installed
- there's no code assistance neither transpilation
- preferences are lost at each restart (the only preference for the moment is just the theme 🤣, thus not a big deal then)
- if u see the _herojs_ central spinner for unexpectedly too long, quit and restart (hopefully u saved the script); I still could not reproduce it exactly, thus I do not know the cause (only happens in the shipped app, not in the dev one). If happens and you have some time/love to give back then please file an issue on github putting as much informations as possible for me to try reproduce & fix it 👍
- to see some output use `console.log`.
- all global modules are accessible with CommonJS (`require`), a the moment it starts the climb search from Applications folder, thus it must really be up.
- double click on the top bar to maximize the window
- choose among many _light_ & _dark_ themes (also the very very very very hot special dark [signavio](https://signavio.com) theme)
- shortcuts:
    - ` + r`: execute the current script
    - ` + backspace`: reset the current script content. 
    - ` + n`: clears the content and forget about the current file if any.
    - ` + o`: open an existing file selecting from your filesystem 
    - ` + s`: save the current script
    - ` + shift + s`: save the current script as (u name it)
    - ` + b`: toggles on/off the webview
 - about the webview: in yout script `window` will refer exactly to the webview global scope

There are other problems but to some extent it is usable and will get better soon 👍




[download latest version (0.0.8)](https://github.com/fedeghe/jshero-app/raw/master/versions/jshero-0.0.8-x64.dmg)  

[changelog](https://github.com/fedeghe/jshero-app/blob/master/CHANGELOG.md)  


![a screenshot](https://raw.githubusercontent.com/fedeghe/jshero-app/master/jshero.png "jsHero")
![a screenshot](https://raw.githubusercontent.com/fedeghe/jshero-app/master/jsheroB.png "jsHero")