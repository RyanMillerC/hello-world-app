# Hello World (Spring Boot)

## Deploy using S2I

```bash
$ oc new-project rest-http-example
$ oc new-app java~https://git.taco.moe/lab/rest-http-example
$ watch -d oc get builds
# Wait for build to complete
$ oc expose svc/rest-http-example
$ curl http://rest-http-example-rest-http-example.apps.ocp.taco.moe/api/greeting
```
