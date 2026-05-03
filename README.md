# webkit-bg-size-bug
Repo to reproduce a WebKitGTK bug in which an element will render at the wrong scale (ignoring background-size) when translated over a scrolling element. This only occurs after scrolling said scrollable element.

## Found Workarounds:
* Disable hw accel (`WEBKIT_DISABLE_COMPOSITING_MODE=1`)
* Set `background-repeat` to `repeat`
* Set `background-attachment` to `fixed` or `local`
