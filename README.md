## Small library to add mouse gestures

---

```js
NiceGesture.start(container, {
  up: (e) => {
    // Do something
  },
  down: (e) => {
    // Do something
  },
  left: (e) => {
    // Do something
  },
  right: (e) => {
    // Do something
  },
  up_and_down_1: (e) => {
    // Do something
  },
  up_and_down_2: (e) => {
    // Do something
  },
  left_and_right_1: (e) => {
    // Do something
  },
  left_and_right_2: (e) => {
    // Do something
  },
  default: (e) => {
    if (App.cursor_on_item(e, App.window_mode)) {
      let item = App.get_cursor_item(App.window_mode, e)

      if (!item.highlighted) {
        if (App.get_highlights(App.window_mode).length > 0) {
          App.pick_item(item)
        }
      }

      App.show_item_menu(item, e.clientX, e.clientY)
      e.preventDefault()
    }
  }
})
```