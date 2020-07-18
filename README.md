# Modal

'Modal' is a native javascript module for show and hide modal windows on a web page.

- Show by clicking a button.
- Hide by clicking a button, outside of modal.
- No scroll when modal active.
- When user scroll down to the end of a page modal shows.

Example of usage:

```javascript
const modalTimerId = setTimeout(() => openModal('.modal', modalTimerId), 300000);

modal('[data-modal]', '.modal', modalTimerId);
```

Example of html markup:

```html
<button data-modal class="btn btn_white">Contact Us</button>
<div class="modal">
    <div class="modal__dialog">
        <div class="modal__content">
            <form action="#">
                <div data-close class="modal__close">&times;</div>
                <div class="modal__title">We will contact you as soon as possible!</div>
                <input required placeholder="You name" name="name" type="text" class="modal__input">
                <input required placeholder="Your phone" name="phone" type="phone" class="modal__input">
                <button class="btn btn_dark btn_min">Call me</button>
            </form>
        </div>
    </div>
</div>
```