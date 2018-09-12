---
collection: forms
title: Radio
date: 2018-09-12T08:24
view: example.twig

snippets:
  -
    text: 'A form **radio** used by default'
    code: |
      <label class="input-radio">
        <input class="input-radio__field" type="radio" name="some-radio-name" value="1">
        <i class="input-radio__icon material-icons">radio_button_unchecked</i>
        <i class="input-radio__icon material-icons">radio_button_checked</i>
        <div class="input-radio__text">
          Radio button text description
        </div>
      </label>
    render: |
      <form>
        <label class="input-radio">
          <input class="input-radio__field" type="radio" name="some-radio-name" value="1">
          <i class="input-radio__icon material-icons">radio_button_unchecked</i>
          <i class="input-radio__icon material-icons">radio_button_checked</i>
          <div class="input-radio__text">
            Radio button text description
          </div>
        </label>
        <label class="input-radio">
          <input class="input-radio__field" type="radio" name="some-radio-name" value="2">
          <i class="input-radio__icon material-icons">radio_button_unchecked</i>
          <i class="input-radio__icon material-icons">radio_button_checked</i>
          <div class="input-radio__text">
            Another radio button with its text
          </div>
        </label>
      </form>


---
