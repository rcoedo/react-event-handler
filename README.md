# react-event-handler

## Description

react-event-handler is a component that allows you to handle the events of children elements, delay the invocation of
the handlers, and manage some extra events like "clickAnywhere".

## Installation

```
npm install --save react-event-handler
```

## Usage
```
import EventHandler from "react-event-handler";

const MyButton () =>
  <EventHandler
    onClick={() => console.log("click!")>
    onMouseEnter={handler: () => console.log("mouse enter!"), delay: 1000}
  >
    <div>click here</div>
  </EventHandler>
```


## API

Props can either be simple handler function or an object with the properties `handler` and `delay`.

| Prop            | Type               | Optional |
|:----------------|:-------------------|:---------|
| onClick         | function or object |    yes   |
| onMouseEnter    | function or object |    yes   |
| onMouseLeave    | function or object |    yes   |
| onFocus         | function or object |    yes   |
| onBlur          | function or object |    yes   |
| onClickAnywhere | function or object |    yes   |

## CHANGELOG

### v0.3.1

* Fix bad event handler usage

### v0.3.0

* Added onContextMenuAnywhere handler
* Fix setTimeout related bugs

### v0.2.0

* Added onContextMenu handler

### v0.1.3

* Fix propType added in v0.1.2 :(

### v0.1.2

* Added missing propType

### v0.1.1

* Fixed broken package

### v0.1.0

* Initial release
