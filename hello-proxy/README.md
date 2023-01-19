# Hello Proxy!

This is a trival example proxy used to test that a deployment can occur to Apigee,
and that the runtime is correctly processing requests.  It's also possible to infer
if the analytics are working when issuing tests by looking for examples of execution
of the proxy.

## How to deploy

Create a zipfile with the content of `apiproxy` and all content immediately under
the zip.  This zip can then be imported manually, using the Apigee APIs or the 
command line tools.

## How to test

This proxy listens under the `/hello-proxy` basepath.  Any request sent to this
basepath is responded to with the `text/plain` payload `Hello from Proxy!`