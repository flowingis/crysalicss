---
collection: forms
title: Text
date: 2018-09-12T08:45
view: example.twig

snippets:
  -
    text: 'A form **text** used as by default, it contains the state message used in `input-text__message` selector.'
    code: |
      <label class="input-text">
        <input type="text" class="input-text__field" name="" value="" placeholder="Please, insert something or go away.">
        <p class="input-text__message">
          This message should be not shown
        </p>
      </label>
  -
    text: 'A form **text** used as by default, it contains the state message shown with  `input-text--default` modifier.'
    cover: true
    code: |
      <label class="input-text input-text--default">
        <input type="text" class="input-text__field" name="" value="" placeholder="Please, insert something or go away.">
        <p class="input-text__message">
          This is a default message
        </p>
      </label>
  -
    text: 'A form **text** used as by default, it contains the state message shown with  `input-text--error` modifier.'
    code: |
      <label class="input-text input-text--error">
        <input type="text" class="input-text__field" name="" value="Heilo. Let's go." placeholder="Please, insert something or go away.">
        <i class="input-text__icon material-icons">mail</i>
        <p class="input-text__message">
          This is an error example
        </p>
      </label>

---
