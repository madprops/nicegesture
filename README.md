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
    // On normal right click
  }
})
```

---

## Variables

```js
// Enable gestures or not
NiceGesture.enabled = true

// Can be `right` or `middle`
NiceGesture.button = `right`

// The bigger the less sensitive it is
NiceGesture.threshold = 10