node-red-node-coffee
====================

This is a similar node to the 'function'-node, which allows custom javascript to be executed (in a sandbox).
This node will allow the enduser to use beautifull compact (sandboxed) coffeescript.

# Installation

Run: 

    npm install node-red-contrib-coffeescript

# Example

    mongo = @context.global.mongo
    msg.succes = false

    if msg.payload.length 
      mongo.getItems (err,items) ->
        msg.succes = true
        cb(msg)
    else return msg

Did you notice the support for *both* synchronous and asynchronous flows?

# Extra notes

I love Node-red!

# Author

Leon van Kammen, http://coderofsalvation.github.io / http://github.com/coderofsalvation
