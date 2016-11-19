# NewMacSetup2016

Trying to set some road to making the MAC work in the way I want it to


1. Go to GetMacApps to get the thing u need right [here](http://www.getmacapps.com/)

2. Change the default from bash to zsh

3. Setup the material theme for zsh + cmder + 
   


## What is the difference between PromiseKit and RxSwift?

The higher level too, Promises (and PromiseKit) are just a tool you can use to write code that needs to go off and do some stuff and return at some unknown time.

Where a simple line print("hello world") executes immediately, something like fetchWeatherIn(state: California) doesn't execute immediately because it makes an HTTP request, and then waits for a response, and then parses the response, (etc, etc, etc). So if you wanted to have something happen after fetchWeatherIn was all done, you'd have to write some tricky code yourself to wait for it to finish, or keep checking to see if it's finished, or something even more clever. Promises are a well-accepted way for writing code like this, and saying "this runs, at some point it comes back when it's finished, and then ..... do the next thing!". Promises also exist in the other big languages, so learning how to use them is valuable for the world outside of Swift.

So with Promises, you can write code that "waits" for things to happen and yet is easy to read. It's possible to do everything you can do with Promises without using Promises, but you'll end up writing a lot of code to do very basic things that have nothing to do with what your app is actually trying to accomplish.

RxSwift is a much bigger idea and promotes a different way of writing apps in general. PromiseKit is great to include in any project that does asynchronous stuff (stuff that does not execute immediately), regardless of whether or not you are using RxSwift.

