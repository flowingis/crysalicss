<img width="64" height="auto" src="https://raw.githubusercontent.com/ideatosrl/crysalicss/master/src/crysalicss-logo.png">

# CrysaliCSS
A component library template to store your CSS code

---

<img width="100%" height="auto" src="https://raw.githubusercontent.com/ideatosrl/crysalicss/master/src/showreel.gif">

#### Installation

To install **CrysaliCSS** just clone it:

```
git clone https://github.com/ideatosrl/crysalicss.git component-library && rm -rf component-library/.git
```

This script will create a folder named `component-library` where the template is ready to be used to host your CSS components. This also removes the `.git` folder to ensure it is correctly tracked into your project.

Then install it's node packages:

```
npm install
```

---

#### Development

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

To build your library without run any watchers / HTTP servers:

```
npm run build
```

The library will be built inside `build` folder with relative paths, this means it should run without the HTTP server.

---

#### Configuration

This is the configuration of **CrysaliCSS** component library ONLY.

To let your **CSS source** run inside the component library, you'll need to customize the `source-styles` npm script [stored here][source_css_path].

| File | Description |
|-|-|
| `metalsmith.yml` | This is the main **Metalsmith** configuration used inside `metalsmith.js`, there is background and viewports configuration, then all the stuff you need to customize. Be sure your [CSS source is correctly set here][source_css_name]. The **icons** are based on [Material design icons][material] codes. |

Some info about the project folders

| Folder | Description |
|-|-|
| `assets` | Where all images are stored. |
| `js` | Where all **JavaScript** files are stored, like iframe nav or clipboard interaction. |
| `posts` | Where all **Markdown** documentation posts are stored. You will add HTML components and how they work with [markdown syntax][markdown]. |
| `sass` | The component library styles, you can customize it's [main colors here][theme_colors] in combination with the [selected logo][logo]. |
| `src` | Just source files, not used inside the build. |
| `twig` | The **HTML templates** written with [Twig][twig]. |

---

#### Writing markdown pages

You should put your CSS documentation inside `posts` folder, in the code below you'll see how a page should be written.

Front matter structure

| Variable | Optional | Description |
|-|:-:|-|
| `collection` | **✗** | Used to **group** components. |
| `date` | ✓ | The **date** of the documentation page created. |
| `title` | **✗** | The **title** of the documentation page created. |
| `view` | **✗** | The template page used, it should be used with `example.twig` template. |
| `snippets` | ✓ | An array of code snippets, used to display all the components of this page. |
| `snippets[0].title` | ✓ | A title of the component. |
| `snippets[0].text` | ✓ | A description of the component (markdown is supported). |
| `snippets[0].code` | **✗** | The code snippet of the component, will be copied in the clipboard and rendered on the page if `render` is not defined. |
| `snippets[0].render` | ✓ | The rendered HTML of the component's code snippet, this is used just to improve render with additional html which should be not copied as code snippet. |
| `snippets[0].extension` | ✓ | Defines the language used by `code` to be properly colored. The file `metalsmith.yml` contains the defined available languages for `prismjs` which is used to color your code. Find `prism.languages` and check if your languages are included. You can checkout the available [list of languages][primsjs-syntax] used in the [prismjs website][primsjs]. |

A template page as example:

```yaml
---
collection: buttons
date: 2018-08-29T11:24
title: Button
view: example.twig

snippets:
  -
    title: 'The main buttons'
    text: 'A basic button, used all around the app.'
    html: |
      <a href="#" class="button">
        A simple button
      </a>
  -
    text: 'Button used to cancel actions. You can use `render` field to display a different content to make better explanations on how components are displayed.'
    html: |
      <a href="#" class="button button--cancel">
        Cancel
      </a>
    render: |
      <div style="display: flex;">
        <a href="#" class="button button--cancel">
          Cancel
        </a>
        <a href="#" class="button">
          Do it!
        </a>
      </div>
---

This is the optional markdown block with additional documentation.

```
---

[CrysaliCSS](https://github.com/ideatosrl/crysalicss) is made with ❤ by [vitto](https://github.com/vitto/) @ [ideato](https://www.ideato.it).

[logo]: https://github.com/ideatosrl/crysalicss/blob/master/metalsmith.yml#L8
[markdown]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
[material]: https://material.io/icons/
[source_css_name]: https://github.com/ideatosrl/crysalicss/blob/master/metalsmith.yml#L7
[source_css_path]: https://github.com/ideatosrl/crysalicss/blob/master/package.json#L17
[theme_colors]: https://github.com/ideatosrl/crysalicss/blob/master/sass/_config/vars.scss
[twig]: https://twig.symfony.com/
[primsjs-syntax]: https://prismjs.com/#languages-list
[primsjs]: https://prismjs.com/
