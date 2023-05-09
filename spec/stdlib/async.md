# Async
Zircon's Asynchronous Handling Module of the Standard Library. It contains methods to deal with async callbacks, futures, and more.

## `timeout(time: Number)`
The `timeout` function takes in an amount of time in miliseconds and then causes the current thread to sleep for that duration, similar to `setTimeout` in JavaScript. 

```rb
io.write "Before Timeout"
async.timeout 1000
io.write "After 1s"
```

## `delayed_callback(time: Number, action: Lambda<Any>)`
The `delayed_callback` function is essentially `timeout`, however, it calls a function supplied to it after the end of the timeout. 

```rb
async.delayed_callback 5000, with 
	io.write "Meow."
end
```
