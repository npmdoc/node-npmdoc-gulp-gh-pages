# api documentation for  [gulp-gh-pages (v0.5.4)](https://github.com/shinnn/gulp-gh-pages#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-gulp-gh-pages.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gulp-gh-pages) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gulp-gh-pages.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gulp-gh-pages)
#### gulp plugin to publish contents to Github pages

[![NPM](https://nodei.co/npm/gulp-gh-pages.png?downloads=true)](https://www.npmjs.com/package/gulp-gh-pages)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-gh-pages/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-gulp-gh-pages_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-gh-pages/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-gulp-gh-pages/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-gulp-gh-pages/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Micheal Benedict",
        "email": "micheal@visionmasterdesigns.com",
        "url": "https://github.com/rowoot"
    },
    "bugs": {
        "url": "https://github.com/shinnn/gulp-gh-pages/issues"
    },
    "contributors": [
        {
            "name": "Shinnosuke Watanabe",
            "url": "https://github.com/shinnn"
        }
    ],
    "dependencies": {
        "gift": "^0.6.1",
        "gulp-util": "^3.0.7",
        "readable-stream": "^2.0.2",
        "rimraf": "^2.4.3",
        "vinyl-fs": "^2.2.1",
        "wrap-promise": "^1.0.1"
    },
    "description": "gulp plugin to publish contents to Github pages",
    "devDependencies": {
        "@shinnn/eslint-config-node-legacy": "^1.0.0",
        "eslint": "^1.7.2",
        "graceful-fs": "^4.1.2",
        "istanbul": "^0.4.0",
        "log-symbols": "^1.0.2",
        "mocha": "^2.3.3",
        "node-uuid": "^1.4.3",
        "octonode": "^0.7.4",
        "read-remove-file": "^3.0.0",
        "vinyl": "^1.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "a6732ca475ab9b5a53253c1c24734c40c21b6546",
        "tarball": "https://registry.npmjs.org/gulp-gh-pages/-/gulp-gh-pages-0.5.4.tgz"
    },
    "files": [
        "index.js",
        "lib"
    ],
    "gitHead": "e740e1c4d8789317db706b3fdb712d82454cbc03",
    "homepage": "https://github.com/shinnn/gulp-gh-pages#readme",
    "keywords": [
        "git",
        "push",
        "commit",
        "branch",
        "deploy",
        "deployment",
        "publish",
        "site",
        "website",
        "gulp",
        "gulpplugin",
        "gh-pages",
        "dist",
        "github"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "rowoot",
            "email": "micheal@visionmasterdesigns.com"
        },
        {
            "name": "shinnn",
            "email": "snnskwtnb@gmail.com"
        }
    ],
    "name": "gulp-gh-pages",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/shinnn/gulp-gh-pages.git"
    },
    "scripts": {
        "coverage": "istanbul cover _mocha test.js -x=test.js -- --timeout 50000",
        "pretest": "eslint --config @shinnn/node-legacy --env mocha --rule 'no-underscore-dangle: 0' --rule 'camelcase: 0' index.js test.js lib",
        "test": "mocha test.js --timeout 50000 --full-trace",
        "test-only": "mocha test.js --timeout 50000 --full-trace"
    },
    "version": "0.5.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module gulp-gh-pages](#apidoc.module.gulp-gh-pages)
1.  [function <span class="apidocSignatureSpan">gulp-gh-pages.</span>git (repo, initialBranch)](#apidoc.element.gulp-gh-pages.git)
1.  object <span class="apidocSignatureSpan">gulp-gh-pages.</span>git.prototype

#### [module gulp-gh-pages.git](#apidoc.module.gulp-gh-pages.git)
1.  [function <span class="apidocSignatureSpan">gulp-gh-pages.</span>git (repo, initialBranch)](#apidoc.element.gulp-gh-pages.git.git)
1.  [function <span class="apidocSignatureSpan">gulp-gh-pages.git.</span>getRemoteUrl (repo, remote)](#apidoc.element.gulp-gh-pages.git.getRemoteUrl)
1.  [function <span class="apidocSignatureSpan">gulp-gh-pages.git.</span>prepareRepo (remoteUrl, origin, dir)](#apidoc.element.gulp-gh-pages.git.prepareRepo)

#### [module gulp-gh-pages.git.prototype](#apidoc.module.gulp-gh-pages.git.prototype)
1.  [function <span class="apidocSignatureSpan">gulp-gh-pages.git.prototype.</span>addFiles (files, options)](#apidoc.element.gulp-gh-pages.git.prototype.addFiles)
1.  [function <span class="apidocSignatureSpan">gulp-gh-pages.git.prototype.</span>checkoutBranch (name)](#apidoc.element.gulp-gh-pages.git.prototype.checkoutBranch)
1.  [function <span class="apidocSignatureSpan">gulp-gh-pages.git.prototype.</span>commit (commitMsg)](#apidoc.element.gulp-gh-pages.git.prototype.commit)
1.  [function <span class="apidocSignatureSpan">gulp-gh-pages.git.prototype.</span>createAndCheckoutBranch (name)](#apidoc.element.gulp-gh-pages.git.prototype.createAndCheckoutBranch)
1.  [function <span class="apidocSignatureSpan">gulp-gh-pages.git.prototype.</span>createBranch (name)](#apidoc.element.gulp-gh-pages.git.prototype.createBranch)
1.  [function <span class="apidocSignatureSpan">gulp-gh-pages.git.prototype.</span>status ()](#apidoc.element.gulp-gh-pages.git.prototype.status)



# <a name="apidoc.module.gulp-gh-pages"></a>[module gulp-gh-pages](#apidoc.module.gulp-gh-pages)

#### <a name="apidoc.element.gulp-gh-pages.git"></a>[function <span class="apidocSignatureSpan">gulp-gh-pages.</span>git (repo, initialBranch)](#apidoc.element.gulp-gh-pages.git)
- description and source-code
```javascript
function Git(repo, initialBranch) {
  this._repo = repo;
  this._staged = [];
  this._localBranches = [];
  this._remoteBranches = [];
  this._currentBranch = initialBranch;
  this._commits = [];
}
```
- example usage
```shell
...
  if (newBranchCreated) {
    resolve(repo);
    return;
  }

  // updating to avoid having local cache not up to date
  gutil.log(TAG, 'Updating repository');
  repo._repo.git('pull', function(err) {
    if (err) {
      reject(err);
      return;
    }
    resolve(repo);
  });
});
...
```



# <a name="apidoc.module.gulp-gh-pages.git"></a>[module gulp-gh-pages.git](#apidoc.module.gulp-gh-pages.git)

#### <a name="apidoc.element.gulp-gh-pages.git.git"></a>[function <span class="apidocSignatureSpan">gulp-gh-pages.</span>git (repo, initialBranch)](#apidoc.element.gulp-gh-pages.git.git)
- description and source-code
```javascript
function Git(repo, initialBranch) {
  this._repo = repo;
  this._staged = [];
  this._localBranches = [];
  this._remoteBranches = [];
  this._currentBranch = initialBranch;
  this._commits = [];
}
```
- example usage
```shell
...
  if (newBranchCreated) {
    resolve(repo);
    return;
  }

  // updating to avoid having local cache not up to date
  gutil.log(TAG, 'Updating repository');
  repo._repo.git('pull', function(err) {
    if (err) {
      reject(err);
      return;
    }
    resolve(repo);
  });
});
...
```

#### <a name="apidoc.element.gulp-gh-pages.git.getRemoteUrl"></a>[function <span class="apidocSignatureSpan">gulp-gh-pages.git.</span>getRemoteUrl (repo, remote)](#apidoc.element.gulp-gh-pages.git.getRemoteUrl)
- description and source-code
```javascript
function getRemoteUrl(repo, remote) {
  return wrapPromise(function(resolve, reject) {
    repo.config(function(err, config) {
      if (err) {
        reject(new Error('Failed to find git repository in ' + config.path));
        return;
      }
      resolve(config.items['remote.' + remote + '.url']);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-gh-pages.git.prepareRepo"></a>[function <span class="apidocSignatureSpan">gulp-gh-pages.git.</span>prepareRepo (remoteUrl, origin, dir)](#apidoc.element.gulp-gh-pages.git.prepareRepo)
- description and source-code
```javascript
function prepareRepo(remoteUrl, origin, dir) {
  var promise;
  if (remoteUrl) {
    // if a remoteUrl was provided, use it
    promise = wrapPromise.Promise.resolve(remoteUrl);
  } else {
    // else try to extract it from the .git folder of
    // the current directory.
    promise = getRemoteUrl(git(process.cwd()), origin);
  }

  return promise.then(function(rUrl) {
    remoteUrl = rUrl;

    return wrapPromise(function(resolve, reject) {
      function initRepo(repo) {
        repo.branch(function(err, head) {
          if (err) {
            reject(err);
            return;
          }
          resolve(new Git(repo, head.name).status());
        });
      }

      function clearAndInitRepo() {
        rimraf(dir, function(rmErr) {
          if (rmErr) {
            reject(rmErr);
            return;
          }

          git.clone(rUrl, dir, function(cloneErr, repo) {
            if (cloneErr) {
              reject(cloneErr);
              return;
            }
            initRepo(repo);
          });
        });
      }

      // assume that if there is a .git folder get its remoteUrl
      // and check if it mathces the one we want to use.
      getRemoteUrl(git(dir), origin).then(function(cwdRemoteUrl) {
        if (remoteUrl === cwdRemoteUrl) {
          initRepo(git(dir));
          return;
        }
        clearAndInitRepo();
      }, function() {
        clearAndInitRepo();
      });
    });
  });
}
```
- example usage
```shell
...
  gutil.log(TAG, 'No files in the stream.');
  cb();
  return;
}

var newBranchCreated = false;

git.prepareRepo(options.remoteUrl, origin, options.cacheDir || '.publish')
.then(function(repo) {
  gutil.log(TAG, 'Cloning repo');
  if (repo._localBranches.indexOf(branch) > -1) {
    gutil.log(TAG, 'Checkout branch '' + branch + ''');
    return repo.checkoutBranch(branch);
  }
...
```



# <a name="apidoc.module.gulp-gh-pages.git.prototype"></a>[module gulp-gh-pages.git.prototype](#apidoc.module.gulp-gh-pages.git.prototype)

#### <a name="apidoc.element.gulp-gh-pages.git.prototype.addFiles"></a>[function <span class="apidocSignatureSpan">gulp-gh-pages.git.prototype.</span>addFiles (files, options)](#apidoc.element.gulp-gh-pages.git.prototype.addFiles)
- description and source-code
```javascript
addFiles = function (files, options) {
  var self = this;

  return wrapPromise(function(resolve, reject) {
    self._repo.add(files, options, function(err) {
      if (err) {
        reject(err);
        return;
      }

      resolve(self.status());
    });
  });
}
```
- example usage
```shell
...
      destStream.write(file);
    });

    destStream.end();
  });
})
.then(function(repo) {
  return repo.addFiles('.', {force: options.force || false});
})
.then(function(repo) {
  var filesToBeCommitted = Object.keys(repo._staged).length;
  if (filesToBeCommitted === 0) {
    gutil.log(TAG, 'No files have changed.');
    cb();
    return;
...
```

#### <a name="apidoc.element.gulp-gh-pages.git.prototype.checkoutBranch"></a>[function <span class="apidocSignatureSpan">gulp-gh-pages.git.prototype.</span>checkoutBranch (name)](#apidoc.element.gulp-gh-pages.git.prototype.checkoutBranch)
- description and source-code
```javascript
checkoutBranch = function (name) {
  var self = this;

  return wrapPromise(function(resolve, reject) {
    self._repo.checkout(name, function(err) {
      if (err) {
        reject(err);
        return;
      }

      self._currentBranch = name;
      resolve(self.status());
    });
  });
}
```
- example usage
```shell
...
      var newBranchCreated = false;

      git.prepareRepo(options.remoteUrl, origin, options.cacheDir || '.publish')
      .then(function(repo) {
gutil.log(TAG, 'Cloning repo');
if (repo._localBranches.indexOf(branch) > -1) {
  gutil.log(TAG, 'Checkout branch '' + branch + ''');
  return repo.checkoutBranch(branch);
}

if (repo._remoteBranches.indexOf(origin + '/' + branch) > -1) {
  gutil.log(TAG, 'Checkout remote branch '' + branch + ''');
  return repo.checkoutBranch(branch);
}
...
```

#### <a name="apidoc.element.gulp-gh-pages.git.prototype.commit"></a>[function <span class="apidocSignatureSpan">gulp-gh-pages.git.prototype.</span>commit (commitMsg)](#apidoc.element.gulp-gh-pages.git.prototype.commit)
- description and source-code
```javascript
commit = function (commitMsg) {
  var self = this;

  return wrapPromise(function(resolve, reject) {
    self._repo.commit(commitMsg, {all: true}, function(err) {
      if (err) {
        reject(err);
      } else {
        resolve(self.status());
      }
    });
  });
}
```
- example usage
```shell
...
  gutil.log(TAG, 'No files have changed.');
  cb();
  return;
}

gutil.log(TAG, 'Adding ' + filesToBeCommitted + ' files.');
gutil.log(TAG, 'Committing "' + message + '"');
repo.commit(message).then(function(newRepo) {
  if (options.push === undefined || options.push) {
    gutil.log(TAG, 'Pushing to remote.');
    newRepo._repo.git('push', {
      'set-upstream': true
    }, [origin, newRepo._currentBranch], function(err) {
      if (err) {
        cb(err);
...
```

#### <a name="apidoc.element.gulp-gh-pages.git.prototype.createAndCheckoutBranch"></a>[function <span class="apidocSignatureSpan">gulp-gh-pages.git.prototype.</span>createAndCheckoutBranch (name)](#apidoc.element.gulp-gh-pages.git.prototype.createAndCheckoutBranch)
- description and source-code
```javascript
createAndCheckoutBranch = function (name) {
  return this.createBranch(name)
  .then(function(repo) {
    return repo.checkoutBranch(name);
  });
}
```
- example usage
```shell
...
  if (repo._remoteBranches.indexOf(origin + '/' + branch) > -1) {
    gutil.log(TAG, 'Checkout remote branch '' + branch + ''');
    return repo.checkoutBranch(branch);
  }

  gutil.log(TAG, 'Create branch '' + branch + '' and checkout');
  newBranchCreated = true;
  return repo.createAndCheckoutBranch(branch);
})
.then(function(repo) {
  return wrapPromise(function(resolve, reject) {
    if (newBranchCreated) {
      resolve(repo);
      return;
    }
...
```

#### <a name="apidoc.element.gulp-gh-pages.git.prototype.createBranch"></a>[function <span class="apidocSignatureSpan">gulp-gh-pages.git.prototype.</span>createBranch (name)](#apidoc.element.gulp-gh-pages.git.prototype.createBranch)
- description and source-code
```javascript
createBranch = function (name) {
  var self = this;

  return wrapPromise(function(resolve, reject) {
    self._repo.create_branch(name, function(err) {
      if (err) {
        reject(err);
      } else {
        self._currentBranch = name;
        resolve(self.status());
      }
    });
  });
}
```
- example usage
```shell
...
};

/*
 * Create and checkout a branch
 * @param name {String} -  String name of the new branch.
**/
Git.prototype.createAndCheckoutBranch = function(name) {
return this.createBranch(name)
.then(function(repo) {
  return repo.checkoutBranch(name);
});
};

Git.prototype.addFiles = function(files, options) {
var self = this;
...
```

#### <a name="apidoc.element.gulp-gh-pages.git.prototype.status"></a>[function <span class="apidocSignatureSpan">gulp-gh-pages.git.prototype.</span>status ()](#apidoc.element.gulp-gh-pages.git.prototype.status)
- description and source-code
```javascript
status = function () {
  var self = this;

  return wrapPromise(function(resolve, reject) {
    self._repo.status(function(err, repo) {
      if (err) {
        reject(err);
        return;
      }

      self._repo = repo.repo;
      self._staged = repo.files;
      wrapPromise.Promise.all([
        getCommits(self._repo, self._currentBranch),
        listRemoteBranches(self._repo),
        listLocalBranches(self._repo)
      ])
      .then(function(args) {
        self._remoteBranches = args[1];
        self._localBranches = args[2];
        self._commits = args[0];
        resolve(self);
      }, reject);
    });
  });
}
```
- example usage
```shell
...
// remove all files
return wrapPromise(function(resolve, reject) {
  repo._repo.remove('.', {r: true}, function(err) {
    if (err) {
      reject(err);
      return;
    }
    resolve(repo.status());
  });
});
      })
      .then(function(repo) {
gutil.log(TAG, 'Copying files to repository');

return wrapPromise(function(resolve, reject) {
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
