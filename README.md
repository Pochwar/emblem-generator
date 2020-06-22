## Emblem Generator: JavaScript Library used to generate SVG emblems

Based on unmaintained repository [GW2Emblem](https://github.com/mtodor/gw2emblem)

### Requirements

[Raphaël](https://github.com/DmitryBaranovskiy/raphael/) - JavaScript library is used for drawing SVG image.

### How to use!

Include following files into HTML:

```
    raphael-min.js
    gw2emblem-defs.js
    gw2emblem.js
```

Init gw2emblem in empty div with [ID = 'gw2embelm-div']:

```
    // 'gw2embelm-div' is div ID and 256 is size of emblem in pixels
    gw2emblem.init('gw2embelm-div', 256);
```

Display GW2 Emblem with object fatched from [GW2 API Docs](https://forum-en.guildwars2.com/forum/community/api/API-Documentation):

```
    gw2emblem.drawEmblemGw2({
    	"background_id":2,
    	"foreground_id":103,
    	"flags":[],
    	"background_color_id":673,
    	"foreground_primary_color_id":443,
    	"foreground_secondary_color_id":473
    });
```

### Notes:

It's possible to use background color (instead of default image) - it's sent as 3rd argument for init function call, fe:
```
gw2emblem.init('gw2embelm-div', 128, 'transparent');
```
or
```
gw2emblem.init('gw2embelm-div', 128, '#3682a0');
```

### Author

Benoît Ripoche

#### Author of original library
Mladen Todorovic
mtodor@gmail.com
