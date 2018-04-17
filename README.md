<img width="64" height="auto" src="https://raw.githubusercontent.com/vitto/crysalicss/master/src/crysalicss-logo.png">

# CrysaliCSS
A component library template to store your CSS code

---

To test locally the component library usually at [this address](http://localhost:3000):

```
npm run dev
```

This script will run watchers and **browser sync** to ensure everything you update will be detected, so `twig` templates, `sass` styles, `md` posts, `js` scripts, assets and also `metalsmith.js` and `metalsmith.yml` files.

If you are working with a **virtual machine** and you don't need **browser sync**, you can run watchers only with this:

```
npm run watch
```

---

To build your library without run any watchers / server http:

```
npm run build
```

The library will be built inside `build` folder with relative paths, so it should run also without HTTP server.

---

#### Configuration

This is the configuration of the component library ONLY.

To let your **CSS source** run inside the component library, you'll need to customize the `source-styles` npm script [stored here][source_css].

| File | Description |
|-|-|
| `metalsmith.yml` | This is the main **Metalsmith** configuration used inside `metalsmith.js`, there is background and viewports configuration, then all the stuff you need to customize. Be sure your [CSS source is correctly set here][souce_css_name]. The **icons** are based on [Material design icons][material] codes. |

Some info about the project folders

| Folder | Description |
|-|-|
| `assets` | Where all images are stored. |
| `js` | Where all **JavaScript** files are stored, like iframe nav interaction |
| `posts` | Where all **Markdown** documentation posts are stored. You will add HTML components and how they work with [markdown syntax][markdown]. |
| `sass` | The component library styles, you can customize it's [main colors here][theme_colors]. |
| `src` | Just source files, not used inside the build. |
| `twig` | The **HTML templates** written with [Twig][twig]. |

[material]: https://material.io/icons/
[souce_css_name]: https://github.com/vitto/crysalicss/blob/master/metalsmith.yml#L7
[markdown]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
[source_css]: https://github.com/vitto/crysalicss/blob/master/package.json#L16
[theme_colors]: https://github.com/vitto/crysalicss/blob/master/sass/_config/vars.scss
[twig]: https://twig.symfony.com/
