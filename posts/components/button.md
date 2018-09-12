---
collection: components
title: Button
date: 2018-09-10T18:01
view: example.twig

snippets:
  -
    title: 'The main buttons'
    text: 'A basic button, used all around the app.'
    html: |
      <a class="button" href="#">
        A simple button
      </a>
  -
    text: "An inline button that doesn't fill the container area by it's width."
    html: |
      <a class="button button--inline" href="#">
        Inline button
      </a>
  -
    text: "Used for actions which should attract user attention."
    html: |
      <a class="button button--inline button--action" href="#">
        Read more
      </a>
  -
    text: "Used for **dangerous** actions which should attract user attention."
    html: |
      <a class="button button--inline button--danger" href="#">
        Delete your data
      </a>
      <script>console.log('ciaone');</script>
  -
    text: "Used for **safe** actions which should attract user attention."
    html: |
      <a class="button button--inline button--safe" href="#">
        Accept terms
      </a>
  -
    text: "Used secondary actions located around the page."
    html: |
      <a class="button button--inline button--small" href="#">
        Resend e-mail verification
      </a>
  -
    text: "Used to go back."
    html: |
      <a class="button button--inline button--outline" href="#">
        Cancel
      </a>
  -
    text: "You can concat button modifiers."
    html: |
      <a class="button button--inline button--outline button--small" href="#">
        Go back
      </a>
---
