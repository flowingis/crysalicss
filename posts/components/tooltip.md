---
collection: components
title: Tooltip
date: 2018-09-12T09:09
view: example.twig

snippets:
  -
    text: 'A basic tooltip, it should be used inside other components as in the `button` example.'
    code: |
      <a href="#" class="button button--inline button--outline tooltip">
        Tooltip
        <div class="tooltip__container">
          <div class="tooltip__balloon">
            Hello, this is a tooltip message, yes I know, it's very cool!
          </div>
        </div>
      </a>
    render: |
      <div style="padding-top: 60px; margin-left: 60px;">
        <a href="#" class="button button--inline button--outline tooltip">
          Tooltip
          <div class="tooltip__container">
            <div class="tooltip__balloon">
              Hello, this is a tooltip message, yes I know, it's very cool!
            </div>
          </div>
        </a>
      </div>
  -
    text: 'A tooltip with a title.'
    code: |
      <a href="#" class="button button--inline button--outline tooltip">
        Tooltip rich
        <div class="tooltip__container">
          <div class="tooltip__balloon">
            <div class="tooltip__title">
              Important notice
            </div>
            <p class="tooltip__text">
              Ahem, sorry, I just forgot what the notice was.
            </p>
          </div>
        </div>
      </a>
    render: |
      <div style="padding-top: 80px; margin-left: 50px;">
        <a href="#" class="button button--inline button--outline tooltip">
          Tooltip rich
          <div class="tooltip__container">
            <div class="tooltip__balloon">
              <div class="tooltip__title">
                Important notice
              </div>
              <p class="tooltip__text">
                Ahem, sorry, I just forgot what the notice was.
              </p>
            </div>
          </div>
        </a>
      </div>
  -
    text: 'A tooltip with a title.'
    cover: true
    code: |
      <a href="#" class="button button--inline button--outline tooltip tooltip--show">
        Tooltip shown by default
        <div class="tooltip__container">
          <div class="tooltip__balloon">
            This is a tooltip opened by default.
          </div>
        </div>
      </a>
    render: |
      <div style="padding-top: 60px; margin-left: 5px;">
        <a href="#" class="button button--inline button--outline tooltip tooltip--show">
          Tooltip shown by default
          <div class="tooltip__container">
            <div class="tooltip__balloon">
              This is a tooltip opened by default.
            </div>
          </div>
        </a>
      </div>
---
