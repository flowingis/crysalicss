---
title: Indice dei componenti
date: 2018-08-29T11:53
view: default.twig
---

### Cos'è una component library?

Questo strumento serve a condividere la documentazione di componenti web. Al suo interno troverai esempi di come utilizzarli nelle pagine del tuo progetto.

Viene utilizzato dai team di sviluppo per seguire una linea guida sull'utilizzo corretto dei componenti modulari che si inseriscono nei template contenenti markup.

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
    code: |
      <a href="#" class="button">
        A simple button
      </a>
  -
    text: 'Button used to cancel actions. You can use `render` field to display a different content to make better explanations on how components are displayed.'
    code: |
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

### Snippet di codice

Gli snippet sono fatti per essere copiati ed incollati nei nuovi contenuti HTML che andranno in produzione.

Una volta incollato, il codice va personalizzato in base ai contenuti necessari, tutti gli attributi `style` sono inseriti solo per scopo cosmetico all'interno della libreria per poter facilitare lo scopo dell'esempio.

###### Codice di esempio

```html
<div class="set--text-right" style="background: white;">
  Codice di esempio
</div>
```

È importante ricordarsi di rimuovere gli attributi `style` cosmetici che non sono relazionati alle fixtures.

```html
<div class="set--text-right">
  Codice da mantenere
</div>
```

Ci sono situazioni dove gli attributi `style` vanno comunque mantenuti, generalmente se devono caricare delle immagini, in questo caso gli esempi avranno immagini placeholder:

```html
<div class="set--text-right" style="background-image: url('//via.placeholder.com/640x480');">
  Codice di esempio
</div>
```

Lo snippet sarà da customizzare con i dati che arrivano dal database in base al sistema di templating che state utilizzando:

```twig
<div class="set--text-right" style="background-image: url('{{ database.image }}');">
  {{ database.text }}
</div>
```

[bem]: https://speakerdeck.com/vitto/workshop-sass-for-bem-development
[frontsize]: https://github.com/ideatosrl/frontsize
[include-media]: http://include-media.com
[sass]: https://sass-lang.com
[primsjs-syntax]: https://prismjs.com/#languages-list
[primsjs]: https://prismjs.com/
