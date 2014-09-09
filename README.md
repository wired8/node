node
====

# Control Flow

[vasync] (https://www.npmjs.org/package/vasync)
[Async](https://github.com/caolan/async) 

```
async.map(['file1','file2','file3'], fs.stat, function(err, results){
    // results is now an array of stats for each file
});

async.filter(['file1','file2','file3'], fs.exists, function(results){
    // results now equals an array of the existing files
});

async.parallel([
    function(){ ... },
    function(){ ... }
], callback);

async.series([
    function(){ ... },
    function(){ ... }
]);
```


[Q](https://github.com/kriskowal/q)

```\Q.fcall(promisedStep1)
.then(promisedStep2)
.then(promisedStep3)
.then(promisedStep4)
.then(function (value4) {
    // Do something with value4
})
.catch(function (error) {
    // Handle any error from all above steps
})
.done();
```


# Testing

* [Mocha](http://visionmedia.github.io/mocha/)
* [Should](https://github.com/visionmedia/should.js/)
* [Sinon](http://sinonjs.org/)
* [Nock]()
* [Supertest]()

Code Coverage

* [Istanbul](https://github.com/gotwarlost/istanbul)

Code Analysis

* [JSHint](https://github.com/jshint/jshint/)
* [JSCS](https://github.com/mdevils/node-jscs)


# IDE

* [Webstorm](http://www.jetbrains.com/webstorm/)
* [Intellij](http://www.jetbrains.com/idea/)

# Middleware

* [Express] (http://expressjs.com/)
