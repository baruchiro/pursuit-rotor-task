# pursuit-rotor-task
Web Component for Pursuit Rotor Task to embed in web application.

[![](https://data.jsdelivr.com/v1/package/gh/baruchiro/pursuit-rotor-task/badge)](https://www.jsdelivr.com/package/gh/baruchiro/pursuit-rotor-task)

## Usage

The Web Component source code is in Github Pages of this repository. To use in an HTML document, just add the script and use the component:

```html
<!DOCTYPE html>
<html>
  <head>
    <script type="text/javascript" src="https://cdn.jsdelivr.net/gh/baruchiro/pursuit-rotor-task/src/PursuitRotorTask.js"></script>
  </head>

  <body>
    <pursuit-rotor-task></pursuit-rotor-task>
    <script>
      document.querySelector("pursuit-rotor-task")
        .addEventListener("finish", e => console.log(e.detail));
    </script>
  </body>
</html>
```

You can look on the `src/index.html` file (also available in Github Pages [here](https://baruchiro.github.io/pursuit-rotor-task/src/index.html)) to see more complicated example.

## API

### Component Attributes

- `component-radius` The radius of the circle bounded by a square. The square is the component size. Default: `"100px"`.
- `dot-radius` The radius of the rotor. Default: `"40px"`.
- `circle-time` The number of seconds to complete a round. Default: `"4"`.

### Finish

To get the task results, you can listen to the `finish` event.

The result object is not defined yet.
