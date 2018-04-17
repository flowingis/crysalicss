# CrysaliCSS
A component library template to store your CSS code

---

<img width="64" height="auto" src="data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+PCFE%0D%0AT0NUWVBFIHN2ZyBQVUJMSUMgIi0vL1czQy8vRFREIFNWRyAxLjEvL0VOIiAiaHR0cDovL3d3dy53%0D%0AMy5vcmcvR3JhcGhpY3MvU1ZHLzEuMS9EVEQvc3ZnMTEuZHRkIj48c3ZnIHdpZHRoPSIxMDAlIiBo%0D%0AZWlnaHQ9IjEwMCUiIHZpZXdCb3g9IjAgMCAzMCAyMiIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0%0D%0AcDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8x%0D%0AOTk5L3hsaW5rIiB4bWw6c3BhY2U9InByZXNlcnZlIiB4bWxuczpzZXJpZj0iaHR0cDovL3d3dy5z%0D%0AZXJpZi5jb20vIiBzdHlsZT0iZmlsbC1ydWxlOmV2ZW5vZGQ7Y2xpcC1ydWxlOmV2ZW5vZGQ7c3Ry%0D%0Ab2tlLWxpbmVqb2luOnJvdW5kO3N0cm9rZS1taXRlcmxpbWl0OjEuNDE0MjE7Ij48Zz48cGF0aCBk%0D%0APSJNNiwyMGM1Ljk4LC0xLjMyOCAxMS45OCwtMS4zMzMgMTgsMGwwLC05Yy02LjAyNCwtMS4zNDgg%0D%0ALTEyLjAyNCwtMS4zNDUgLTE4LDBsMCw5WiIgc3R5bGU9ImZpbGw6dXJsKCNfTGluZWFyMSk7Ii8+%0D%0APHBhdGggZD0iTTE0LDhsLTgsM2wwLDIuNjY3bC00LC0xLjY2N2wwLC0xMGwxMiw1bDAsMVoiIHN0%0D%0AeWxlPSJmaWxsOiNmZmU0MDA7Ii8+PHBhdGggZD0iTTYsMTMuNjY3bDgsMy4zMzNsLTgsM2wwLC02%0D%0ALjMzM1oiIHN0eWxlPSJmaWxsOiNmZmU0MDA7Ii8+PHBhdGggZD0iTTE0LDE3bC04LC0zLjMzM2ww%0D%0ALC0yLjY2N2w4LC0zbDAsOVoiIHN0eWxlPSJmaWxsOiNmYzA7Ii8+PHBhdGggZD0iTTE2LDhsMCwt%0D%0AMWwxMiwtNWwwLDEwbC00LDEuNjY3bDAsLTIuNjY3bC04LC0zWiIgc3R5bGU9ImZpbGw6I2ZmZTQw%0D%0AMDsiLz48cGF0aCBkPSJNMjQsMTMuNjY3bDAsNi4zMzNsLTgsLTNsOCwtMy4zMzNaIiBzdHlsZT0i%0D%0AZmlsbDojZmZlNDAwOyIvPjxwYXRoIGQ9Ik0yNCwxMWwwLDIuNjY3bC04LDMuMzMzbDAsLTlsOCwz%0D%0AWiIgc3R5bGU9ImZpbGw6I2ZjMDsiLz48L2c+PGRlZnM+PGxpbmVhckdyYWRpZW50IGlkPSJfTGlu%0D%0AZWFyMSIgeDE9IjAiIHkxPSIwIiB4Mj0iMSIgeTI9IjAiIGdyYWRpZW50VW5pdHM9InVzZXJTcGFj%0D%0AZU9uVXNlIiBncmFkaWVudFRyYW5zZm9ybT0ibWF0cml4KDE4LDAsMCwxMC4wMTAxLDYsMTQuOTk1%0D%0AKSI+PHN0b3Agb2Zmc2V0PSIwIiBzdHlsZT0ic3RvcC1jb2xvcjojMDAwO3N0b3Atb3BhY2l0eTow%0D%0ALjE1Ii8+PHN0b3Agb2Zmc2V0PSIwLjUiIHN0eWxlPSJzdG9wLWNvbG9yOiMwMDA7c3RvcC1vcGFj%0D%0AaXR5OjAiLz48c3RvcCBvZmZzZXQ9IjEiIHN0eWxlPSJzdG9wLWNvbG9yOiMwMDA7c3RvcC1vcGFj%0D%0AaXR5OjAuMTUiLz48L2xpbmVhckdyYWRpZW50PjwvZGVmcz48L3N2Zz4=">

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
