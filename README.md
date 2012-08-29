http-responder
===================

### start me up

    http-responder daemon

go to http://<whatever>/conf to setup your response. Any other url than /conf
will respond with the response currently configured

### usage

http-responder lets you configure it's HTTP response with some fields:

* headers
* body
* status
* sleep

##### headers

This is the headers you want your request to have. It will pick up some more
(for now), the default mojo ones. Just enter them like this

    Cache-Control: max-age=1, no-cache
    Content-type: application/xml+rss

##### body

The body you want to respond with. Put in anything you want, we don't do much
with it.

##### status

The status code to respond with, can use this to test that you respond in the
right way in your app to different status codes.

##### sleep

This is the number of milliseconds to sleep during the request. 1000 means
sleep for 1 second. Good for testing that your apps handle timeouts for
instance.


