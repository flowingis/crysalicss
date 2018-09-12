---
collection: forms
title: Textarea
date: 2018-09-12T08:45
view: example.twig

snippets:
  -
    text: "A form **textarea** used as by default, it contains the state message used in `input-text__message` selector."
    code: |
      <label class="input-text">
        <textarea class="input-text__field input-text__field--textarea" name="name" placeholder="Please, insert something or go away."></textarea>
        <p class="input-text__message">
          This message should be not shown
        </p>
      </label>
  -
    text: "A form **textarea** used as by default, it contains the state message shown with  `input-text--default` modifier."
    code: |
      <label class="input-text input-text--default">
        <textarea class="input-text__field input-text__field--textarea" name="name" placeholder="Please, insert something or go away."></textarea>
        <p class="input-text__message">
          This is a default message
        </p>
      </label>
  -
    text: "A form **textarea** used as by default, it contains the state message shown with  `input-text--error` modifier."
    code: |
      <label class="input-text input-text--error">
        <textarea class="input-text__field input-text__field--textarea" name="name" placeholder="Please, insert something or go away."></textarea>
        <i class="input-text__icon material-icons">mail</i>
        <p class="input-text__message">
          This is an error example
        </p>
      </label>

---
