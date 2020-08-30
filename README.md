## DENO SANDBOX

A sandbox app for playing with Deno.JS

### What you are not going to find (yet)

* Unit testing
* Lint strategy
* CI/CD
* Any kind of automation

### What you are going to find:

* App deployed on heroku (free plan);
* Simple endpoints just for testing the deploy on heroku (so I can ensure it is running);


### Important Links

* Heroku buildpacks: https://devcenter.heroku.com/articles/buildpacks
* Unofficial Deno buildpack: https://github.com/chibat/heroku-buildpack-deno.git

### Accessing the app

1. Open the url: https://deno-sandbox.herokuapp.com
2. `HTTP GET /` endpoint is the "ping" route.  It will always return http 200 with "ok = true";
3. `HTTP GET /todos` will return a static list of "items";

**IMPORTANT:** The first access to any rout is going to be very slow because the app is probably sleeping on Heroku. It is also important to notice that Heroku still doesn't have an "official" buildpack, so I used the one listed above.

