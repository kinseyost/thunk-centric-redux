# redux-socket.io-message-thunk
A redux middleware that maps socket.io messages to action creators and thunks.

### This library is super opinionated:
Requires use of the `redux-thunk` middleware for handling errors.  Requires that all socket.io messages will arrive with a `type` property, and there will be a corresponding action creator mapped for each message `type`.  Handles errors by dispatching thunks that throw errors, which makes sense only if you also use an error handling middleware like `redux-thunk-error-handler`

If you're looking for a slightly less opinionated socket.io -> redux connector, or an easy way to use socket.io in a request/response paradigm from inside thunks, look instead at:
 * [redux-socket.io](https://www.npmjs.com/package/redux-socket.io)
 * [socket.io-promise](https://www.npmjs.com/package/socket.io-promise)

## A part of the [thunk-centric-redux](//github.com/itaylor/thunk-centric-redux) set of tools
This library is part of a larger set of tools that can be helpful for making thunk-centric Redux applications.  [Visit that project](//github.com/itaylor/thunk-centric-redux) to see a runnable example app that makes use of this code in context.

### MIT License
Copyright (c) 2015-2018 Ian Taylor

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
