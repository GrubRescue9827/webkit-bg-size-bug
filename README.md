# webkit-bg-size-bug
Repo to reproduce a WebKitGTK bug in which an element will use the wrong background-size property when translated over a scrolling element.

## Found Workarounds:
* Disable hw accel (`WEBKIT_DISABLE_COMPOSITING_MODE=1`)
* Set `background-repeat` to `repeat`
* Set `background-attachment` to `fixed` or `local`
