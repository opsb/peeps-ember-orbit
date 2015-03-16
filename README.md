# Ember-Orbit Client for "Peeps"

This is a client app illustrating the use of
[ember-orbit](https://github.com/orbitjs/ember-orbit/).

It communicates with a [JSON API](http://jsonapi.org/) backend provided by
[Peeps](https://github.com/cerebris/peeps-uuids), a Rails server that was
written using [JSONAPI::Resources](https://github.com/cerebris/jsonapi-resources).

This client also uses Orbit to synchronize its memory source with a local
storage source so that it can work offline.

> The offline synchronization features are not yet complete and require further
work in this project and Orbit itself.

## Prerequisites

You will need the following things properly installed on your computer.

* [Git](http://git-scm.com/)
* [Node.js](http://nodejs.org/) (with NPM)
* [Bower](http://bower.io/)
* [Ember CLI](http://www.ember-cli.com/)
* [PhantomJS](http://phantomjs.org/)
* [Firebase](http://firebase.com/) # create an account which will create a new app for you, note the URL of the new app

It also requires the unpackaged
[orbit-firebase](https://github.com/opsb/orbit-firebase).

After installiing and running orbit-firebase, do the following:

* change to orbit-firebase's build directory
* bower link

## Installation

* `git clone <repository-url>` this repository
* change into the new directory
* bower link orbit-firebase
* `ember install`

## Running / Development

* edit this line in app/initializers/ember-orbit.js and replace with your app's firebase url:

```js
 firebaseRef: new Firebase("[your firebase app url]")
 ```

* `ember server -p 4300` # run on port 4300 to not conflict with
  orbit-firebase on 4200
* Visit your app at [http://localhost:4300](http://localhost:4300).

### Code Generators

Make use of the many generators for code, try `ember help generate` for more details

### Running Tests

* `ember test`
* `ember test --server`

### Building

* `ember build` (development)
* `ember build --environment production` (production)

### Deploying

Specify what it takes to deploy your app.

## Further Reading / Useful Links

* [ember.js](http://emberjs.com/)
* [ember-cli](http://www.ember-cli.com/)
* Development Browser Extensions
  * [ember inspector for chrome](https://chrome.google.com/webstore/detail/ember-inspector/bmdblncegkenkacieihfhpjfppoconhi)
  * [ember inspector for firefox](https://addons.mozilla.org/en-US/firefox/addon/ember-inspector/)
