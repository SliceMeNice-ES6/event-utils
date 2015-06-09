# event-utils
ECMAScript 6 Event Utilities

---

* [debounce()](#debounce) returns a function, that, as long as it continues to be invoked, will not call the provided function.

---

### debounce
Returns a function, that, as long as it continues to be invoked, will not
call the provided function. The given function will be called after the debounce
function has stopped being called for N milliseconds. If `immediate` is passed, trigger
the function on the leading edge, instead of the trailing.

###### Example

```
window.addEventListener( 'resize', debounce( onResize, 250, false ) );
```

###### Parameters

* _func_  
the function to be invoked, when the debounce function has stopped being called for N milliseconds.

* _wait_
is the time to wait before calling the provided function, after the debounce function has stopped being called. If `immediate` is passed, this defines the time between two calls to the given function.

* _immediate_ (optional)
defines whether to trigger the function on the leading edge, instead of the trailing.

###### Returns

* A function, that, as long as it continues to be invoked, will not call the provided function.