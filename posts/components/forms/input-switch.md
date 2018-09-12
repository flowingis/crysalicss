---
collection: forms
title: Switch (checkbox)
date: 2018-09-12T08:39
view: example.twig

snippets:
  -
    text: 'A form **checkbox** used as switch'
    code: |
      <label class="input-switch">
        <input class="input-switch__field" type="checkbox" name="switch-checkbox-name" value="1">
        <div class="input-switch__box">
          <div class="input-switch__dot"></div>
        </div>
        <div class="input-switch__text">
          Do something normal
        </div>
      </label>
  -
    text: 'A form **checkbox** used as switch with a tooltip'
    code: |
      <label class="input-switch tooltip">
        <input class="input-switch__field" type="checkbox" name="switch-checkbox-name" value="1">
        <div class="input-switch__box">
          <div class="input-switch__dot"></div>
        </div>
        <div class="input-switch__text">
          Do something terrible
          <div class="tooltip__container">
            <div class="tooltip__balloon tooltip__balloon--warning">
              Are you sure you wanna activate this? It's just crazy!
            </div>
          </div>
        </div>
      </label>
    render: |
      <label class="input-switch tooltip" style="margin-top: 100px; margin-left: 10px;">
        <input class="input-switch__field" type="checkbox" name="switch-checkbox-name" value="1">
        <div class="input-switch__box">
          <div class="input-switch__dot"></div>
        </div>
        <div class="input-switch__text">
          Do something terrible
          <div class="tooltip__container">
            <div class="tooltip__balloon tooltip__balloon--warning">
              Are you sure you wanna activate this? It's just crazy!
            </div>
          </div>
        </div>
      </label>
---
