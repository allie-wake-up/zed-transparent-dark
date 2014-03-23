zed-transparent-dark
====================

A zed theme that slightly modifies the default dark theme.

The main differences are in goto and autocomplete.  The boxes are now slightly transparent and have a box shadow.  The goto hint is hidden.  Macs also use custom scrollbar css.

![goto screenshot](/readme/goto.png)

![autocomplete screenshot](/readme/autocomplete.png)

### Installing

You can install the theme using zpm's install command or editing your user.json packages array.  Either way you can use the following url:

    gh:thekiteeatingtree/zed-transparent-dark
    
### Ace Theme

By default this theme uses the monokai ace theme.  Fortunately this is easy to edit.  Open /packages/gh/thekiteeatingtree/zed-transparent-dark/config.json in your configuration project.  It looks like this:

    {
        "themes": {
            "transparent-dark": {
                "name": "Transparent Dark",
                "dark": true,
                "cssClass": "ace-monokai",
                "css": [
                    "/default/theme/monokai.css",
                    "./transparent-dark.css"
                ]
            }
        }
    }
    
If you edit the cssClass and the first entry in css you can use whatever ace theme you prefer.