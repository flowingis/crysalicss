---
collection: components
title: Tag
date: 2018-09-10T18:01
view: example.twig

snippets:
  -
    text: 'A basic label, used all around the app.'
    html: |
      <div class="tag">
        <div class="tag__text">Tag name</div>
      </div>
    render: |
      <div style="margin-left: 10px;">
        <div class="tag">
          <div class="tag__text">Tag</div>
        </div>
        <div class="tag">
          <div class="tag__text">Tag with a very long text that is impossible to read</div>
        </div>
      </div>
  -
    text: 'A basic label, used for **minor** updates.'
    html: |
      <div class="tag tag--silent">
        <div class="tag__text">Silent</div>
      </div>
    render: |
      <div style="margin-left: 10px;">
        <div class="tag tag--silent">
          <div class="tag__text">Silent</div>
        </div>
      </div>
  -
    text: 'A label, used for **problems to solve**.'
    html: |
      <div class="tag tag--error">
        <div class="tag__text">Error</div>
      </div>
    render: |
      <div style="margin-left: 10px;">
        <div class="tag tag--error">
          <div class="tag__text">Error</div>
        </div>
      </div>
  -
    text: 'A label, used for **changes** to the app.'
    html: |
      <div class="tag tag--info">
        <div class="tag__text">Information</div>
      </div>
    render: |
      <div style="margin-left: 10px;">
        <div class="tag tag--info">
          <div class="tag__text">Information</div>
        </div>
      </div>
  -
    text: 'A label, used for **goals** succeded.'
    html: |
      <div class="tag tag--success">
        <div class="tag__text">Success</div>
      </div>
    render: |
      <div style="margin-left: 10px;">
        <div class="tag tag--success">
          <div class="tag__text">Success</div>
        </div>
      </div>
---
