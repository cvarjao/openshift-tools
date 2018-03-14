# Request Logger
A simple python web-application that prints a page with all the HTTP request headers


# Using
For using in openshift, use the oc command line as follow:

```
oc new-app openshift/python:2.7~https://github.com/cvarjao/openshift-tools.git --context-dir=utils/request_logger --name=request-logger
oc create route edge request-logger --service=request-logger --hostname=<hostname>
```
