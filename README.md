# CrysaliCSS
A component library template to store your CSS code

---

<img width="64" height="auto" src="https://raw.githubusercontent.com/vitto/crysalicss/master/src/crysalicss-logo.png">

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

| File | Description |
|-|-|
| `metalsmith.yml` | This is the main **Metalsmith** configuration used inside `metalsmith.js` |

Some info about the project folders

| Folder | Description |
|-|-|
| `assets` | Where all images are stored |
| `js` | Where all **JavaScript** files are stored, like iframe nav interaction |
| `posts` | Where all **Markdown** documentation posts are stored |
| `sass` | The component library styles |
| `src` | Just source files, not used inside the build |
| `twig` | The **HTML templates** written with Twig |
