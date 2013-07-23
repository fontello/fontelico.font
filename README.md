Fontelico
=========

This collection was started by [fontello project](http://fontello.com) to
collaborate different small sets, missed in other iconic fonts.
Also, it helps authors to share their works with community, as
font glyphs.

If you have not enougth icons, to create independent font, but still wish to
share - suggest your images here.


Installation
------------

This step is required, if you wish to contribute icons.

1. You need `node.js` 0.8+ and `fontforge` installed first.
2. run `npm install` in project folder
3. (optional) install [ttfautohint](http://www.freetype.org/ttfautohint/). Under
   Ubuntu just run `make dependencies` command. You can safely skip
   this step.


Contributing
------------

Note, we accept icons under pure CC BY license, without additional requirements.
Please, don't add icons, which require users to give links, mention author and
do any other kinds of promotion.

1. Create fork and clone your repo locally.
2. Add icon to `./src/svg_orig` folder
  - icon should be 1000x1000
  - black and white, no colors
  - no fills, filling is defined by contour direction
3. run `make dump`, it will automatically reoptimize images
4. check result in `./src/svg` folder. It should contain only on `path`
   in it. If you are satisfied, copy your image back to `./svg_orig`
5. Edit `config.yaml`, add your icon description there. Every icon MUST have
   unique id. You can generate those by command
   `node -e "for(var i=10; i>0; i--) console.log(require('crypto').randomBytes(16).toString('hex'));"`
6. That's not mandatory, but you can built font with `make dist` command
7. Commit content of `./src` folder and make pull request on github.
   _Attention! Don't commit font files!_ That can create unnesessary
   merge conflicts.

If this is difficult for you, just create new [ticket](https://github.com/fontello/brandico.font/issues)
and attach there your icon, as described in step 2, and icon description. We will
do the rest


Contributors
------------

- Angela Berbentseva (emoticons, spinners).
  [Email](mailto:berbentseva_angela@yahoo.com)
- Sebastian Janzen (crowns).
  [Email](sebastian.janzen@hl-services.de), [@sja](https://github.com/sja)


Contacts
--------

Vitaly Puzrin (Fontello project)

- [Email](mailto:vitaly@rcdesign.ru)
- [Github](https://github.com/puzrin)
- [Twitter](https://twitter.com/puzrin)


Licence
-------

Font is distributed under
[SIL](http://scripts.sil.org/cms/scripts/page.php?site_id=nrsi&id=OFL) licence.

All icons are distributed under
[CC BY](http://creativecommons.org/licenses/by-sa/3.0/) licence.

We suggest to use this font via [fontello](http://fontello.com) project, but
you also can materials in any other way, if follow license.
