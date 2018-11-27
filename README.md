# firefox-quantum-theme

Reverse-engineered https://twitter.com/jasonlaster11/status/1022547128818782208

![](/screenshot.png)

Install theme https://addons.mozilla.org/en-US/firefox/addon/quantumgradient/

Put below in userChrome.css 

```
@namespace url("http://www.mozilla.org/keymaster/gatekeeper/there.is.only.xul");

#nav-bar {
    box-shadow: none !important;
}   

#navigator-toolbox::after {
    border-bottom: none !important; 
}

#navigator-toolbox {
    --tabs-border-color: rgba(100,0,0,.1) !important;
}

:root {
    --toolbar-bgcolor: rgba(0,0,0,0.2) !important;
}

.tab-line {
    background-color: transparent !important;
}
```

If you don't have userChrome.css:

`about:support -> Profile Folder > Open Folder > create directory chrome > create userChrome.css inside chrome directory`
