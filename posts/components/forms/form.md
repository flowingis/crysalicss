---
collection: forms
title: Form
date: 2018-09-12T08:12
view: example.twig

snippets:
  -
    text: 'A basic form, used all around the app.'
    code: |
      <form class="form">
        <div class="form__row">
          <div class="form__cell form__cell--half">
            <div class="input-select input-select--fill">
                <select class="input-select__field">
                  <option value="0">Select your destiny...</option>
                  <option value="1">Chef</option>
                  <option value="2">Developer</option>
                  <option value="3">Famous</option>
                  <option value="4">Killer</option>
                  <option value="5">Lobby boy</option>
                  <option value="6">Poor</option>
                  <option value="7">Rich</option>
                  <option value="8">Rock star</option>
                </select>
                <i class="input-select__icon material-icons">keyboard_arrow_down</i>
            </div>
          </div>
          <div class="form__cell form__cell--half">
            <label class="input-switch tooltip">
              <input class="input-switch__field" type="checkbox" name="switch-checkbox-name" value="1">
              <div class="input-switch__box">
                <div class="input-switch__dot"></div>
              </div>
              <div class="input-switch__text">
                Do something nice
                <div class="tooltip__container">
                  <div class="tooltip__balloon tooltip__balloon--warning">
                    I know you can check this switch!
                  </div>
                </div>
              </div>
            </label>
          </div>
        </div>

        <div class="form__row form__row--readable">
          <div class="form__cell form__cell--tiny">
            <label class="input-radio">
              <input class="input-radio__field" type="radio" name="some-radio-name" value="1">
              <i class="input-radio__icon material-icons">radio_button_unchecked</i>
              <i class="input-radio__icon material-icons">radio_button_checked</i>
              <div class="input-radio__text">
                I would like to do this if you think this isn't a problem.
              </div>
            </label>
          </div>
          <div class="form__cell form__cell--tiny">
            <label class="input-radio">
              <input class="input-radio__field" type="radio" name="some-radio-name" value="1">
              <i class="input-radio__icon material-icons">radio_button_unchecked</i>
              <i class="input-radio__icon material-icons">radio_button_checked</i>
              <div class="input-radio__text">
                Also this option could not be bad, just shut up and take my money!
              </div>
            </label>
          </div>
          <div class="form__cell form__cell--tiny">
            <label class="input-radio">
              <input class="input-radio__field" type="radio" name="some-radio-name" value="1">
              <i class="input-radio__icon material-icons">radio_button_unchecked</i>
              <i class="input-radio__icon material-icons">radio_button_checked</i>
              <div class="input-radio__text">
                No, I really don't think it's ok to do this.
              </div>
            </label>
          </div>
        </div>

        <div class="form__row">
          <div class="form__cell form__cell--almost">
            Doing this action will be nice for your entire life.
          </div>
          <div class="form__cell form__cell--tiny">
            <a href="#" class="button button--safe">Save contents</a>
          </div>
        </div>
      </form>
---
