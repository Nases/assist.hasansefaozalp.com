# Things that I learned during node auth

`req.flash('messages')` will delete the session variable after this function has been called once.  
So assign it to a variable if we want to use it more than one time.   
Also if there is no messages in `req.flash('messages')` for example, it will return an empty array so that we don't have to do it like `req.flash('messages') || []`

If we don't call `req.flash('messages')` after redirect it will persist in the session and wait for to be called. We can have multiple redirects before calling the `req.flash('messages')`.

