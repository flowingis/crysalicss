---
collection: forms
title: Checkbox
date: 2018-09-12T08:24
view: example.twig

snippets:
  -
    text: 'A form **checkbox** used by default'
    code: |
      <label class="input-checkbox">
        <input class="input-checkbox__field" type="checkbox" name="some-name" value="1">
        <i class="input-checkbox__icon material-icons">check_box_outline_blank</i>
        <i class="input-checkbox__icon material-icons">check_box</i>
        <div class="input-checkbox__text">
          Checkbox text description
        </div>
      </label>
  -
    text: 'A form **checkbox** used to reject stuff'
    code: |
      <label class="input-checkbox input-checkbox--avoid">
        <input class="input-checkbox__field" type="checkbox" name="some-name" value="1">
        <i class="input-checkbox__icon material-icons">check_box_outline_blank</i>
        <i class="input-checkbox__icon material-icons">block</i>
        <div class="input-checkbox__text">
          I don't want to recive this stuff
        </div>
      </label>
---
