# api documentation for  [fs-promise (v2.0.2)](https://github.com/kevinbeaty/fs-promise#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-fs-promise.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-fs-promise) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-fs-promise.svg)](https://travis-ci.org/npmdoc/node-npmdoc-fs-promise)
#### Filesystem methods as promises with fs-extra

[![NPM](https://nodei.co/npm/fs-promise.png?downloads=true)](https://www.npmjs.com/package/fs-promise)

[![apidoc](https://npmdoc.github.io/node-npmdoc-fs-promise/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-fs-promise_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-fs-promise/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-fs-promise/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-fs-promise/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Kevin Beaty"
    },
    "bugs": {
        "url": "https://github.com/kevinbeaty/fs-promise/issues"
    },
    "dependencies": {
        "any-promise": "^1.3.0",
        "fs-extra": "^2.0.0",
        "mz": "^2.6.0",
        "thenify-all": "^1.6.0"
    },
    "description": "Filesystem methods as promises with fs-extra",
    "devDependencies": {
        "@types/fs-extra": "0.0.37",
        "@types/mz": "0.0.30",
        "bluebird": "^3.0.0",
        "es6-promise": "^4.0.0",
        "mocha": "^3.0.0",
        "q": "^1.0.0",
        "rsvp": "^3.0.0",
        "when": "^3.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "cfea45c80f46480a3fd176213fa22abc8c159521",
        "tarball": "https://registry.npmjs.org/fs-promise/-/fs-promise-2.0.2.tgz"
    },
    "gitHead": "7bc0779243defc93cc4b0921d330ba3d5af79519",
    "homepage": "https://github.com/kevinbeaty/fs-promise#readme",
    "keywords": [
        "promise",
        "fs",
        "file",
        "file system"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "kevinbeaty",
            "email": "kevin@simplectic.com"
        }
    ],
    "name": "fs-promise",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/kevinbeaty/fs-promise.git"
    },
    "scripts": {
        "test": "mocha"
    },
    "version": "2.0.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module fs-promise](#apidoc.module.fs-promise)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>FileReadStream (path, options)](#apidoc.element.fs-promise.FileReadStream)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>FileWriteStream (path, options)](#apidoc.element.fs-promise.FileWriteStream)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>ReadStream (path, options)](#apidoc.element.fs-promise.ReadStream)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>Stats ( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec)](#apidoc.element.fs-promise.Stats)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>WriteStream (path, options)](#apidoc.element.fs-promise.WriteStream)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>_toUnixTimestamp (time)](#apidoc.element.fs-promise._toUnixTimestamp)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>access ()](#apidoc.element.fs-promise.access)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>accessSync (path, mode)](#apidoc.element.fs-promise.accessSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>appendFile ()](#apidoc.element.fs-promise.appendFile)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>appendFileSync (path, data, options)](#apidoc.element.fs-promise.appendFileSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>chmod ()](#apidoc.element.fs-promise.chmod)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>chmodSync (target, mode)](#apidoc.element.fs-promise.chmodSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>chown ()](#apidoc.element.fs-promise.chown)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>chownSync (target, uid, gid)](#apidoc.element.fs-promise.chownSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>close ()](#apidoc.element.fs-promise.close)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>closeSync (fd)](#apidoc.element.fs-promise.closeSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>copy ()](#apidoc.element.fs-promise.copy)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>copySync (src, dest, options)](#apidoc.element.fs-promise.copySync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>createFile ()](#apidoc.element.fs-promise.createFile)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>createFileSync (file)](#apidoc.element.fs-promise.createFileSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>createLink ()](#apidoc.element.fs-promise.createLink)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>createLinkSync (srcpath, dstpath, callback)](#apidoc.element.fs-promise.createLinkSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>createReadStream (path, options)](#apidoc.element.fs-promise.createReadStream)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>createSymlink ()](#apidoc.element.fs-promise.createSymlink)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>createSymlinkSync (srcpath, dstpath, type, callback)](#apidoc.element.fs-promise.createSymlinkSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>createWriteStream (path, options)](#apidoc.element.fs-promise.createWriteStream)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>emptyDir ()](#apidoc.element.fs-promise.emptyDir)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>emptyDirSync (dir)](#apidoc.element.fs-promise.emptyDirSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>emptydir ()](#apidoc.element.fs-promise.emptydir)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>emptydirSync (dir)](#apidoc.element.fs-promise.emptydirSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>ensureDir ()](#apidoc.element.fs-promise.ensureDir)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>ensureDirSync (p, opts, made)](#apidoc.element.fs-promise.ensureDirSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>ensureFile ()](#apidoc.element.fs-promise.ensureFile)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>ensureFileSync (file)](#apidoc.element.fs-promise.ensureFileSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>ensureLink ()](#apidoc.element.fs-promise.ensureLink)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>ensureLinkSync (srcpath, dstpath, callback)](#apidoc.element.fs-promise.ensureLinkSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>ensureSymlink ()](#apidoc.element.fs-promise.ensureSymlink)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>ensureSymlinkSync (srcpath, dstpath, type, callback)](#apidoc.element.fs-promise.ensureSymlinkSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>exists (filename, callback)](#apidoc.element.fs-promise.exists)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>existsSync (path)](#apidoc.element.fs-promise.existsSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>fchmod ()](#apidoc.element.fs-promise.fchmod)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>fchmodSync (target, mode)](#apidoc.element.fs-promise.fchmodSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>fchown ()](#apidoc.element.fs-promise.fchown)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>fchownSync (target, uid, gid)](#apidoc.element.fs-promise.fchownSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>fdatasync ()](#apidoc.element.fs-promise.fdatasync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>fdatasyncSync (fd)](#apidoc.element.fs-promise.fdatasyncSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>fstat ()](#apidoc.element.fs-promise.fstat)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>fstatSync (target)](#apidoc.element.fs-promise.fstatSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>fsync ()](#apidoc.element.fs-promise.fsync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>fsyncSync (fd)](#apidoc.element.fs-promise.fsyncSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>ftruncate ()](#apidoc.element.fs-promise.ftruncate)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>ftruncateSync (fd, len)](#apidoc.element.fs-promise.ftruncateSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>futimes ()](#apidoc.element.fs-promise.futimes)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>futimesSync (fd, atime, mtime)](#apidoc.element.fs-promise.futimesSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>gracefulify (fs)](#apidoc.element.fs-promise.gracefulify)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>lchmod (path, mode, cb)](#apidoc.element.fs-promise.lchmod)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>lchmodSync ()](#apidoc.element.fs-promise.lchmodSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>lchown ()](#apidoc.element.fs-promise.lchown)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>lchownSync ()](#apidoc.element.fs-promise.lchownSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>link ()](#apidoc.element.fs-promise.link)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>linkSync (existingPath, newPath)](#apidoc.element.fs-promise.linkSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>lstat ()](#apidoc.element.fs-promise.lstat)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>lstatSync (target)](#apidoc.element.fs-promise.lstatSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>lutimes (_a, _b, _c, cb)](#apidoc.element.fs-promise.lutimes)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>lutimesSync ()](#apidoc.element.fs-promise.lutimesSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>mkdir ()](#apidoc.element.fs-promise.mkdir)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>mkdirSync (path, mode)](#apidoc.element.fs-promise.mkdirSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>mkdirp ()](#apidoc.element.fs-promise.mkdirp)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>mkdirpSync (p, opts, made)](#apidoc.element.fs-promise.mkdirpSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>mkdirs ()](#apidoc.element.fs-promise.mkdirs)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>mkdirsSync (p, opts, made)](#apidoc.element.fs-promise.mkdirsSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>mkdtemp ()](#apidoc.element.fs-promise.mkdtemp)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>mkdtempSync (prefix, options)](#apidoc.element.fs-promise.mkdtempSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>move ()](#apidoc.element.fs-promise.move)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>moveSync (src, dest, options)](#apidoc.element.fs-promise.moveSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>open ()](#apidoc.element.fs-promise.open)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>openSync (path, flags, mode)](#apidoc.element.fs-promise.openSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>outputFile ()](#apidoc.element.fs-promise.outputFile)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>outputFileSync (file, data, encoding)](#apidoc.element.fs-promise.outputFileSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>outputJSON ()](#apidoc.element.fs-promise.outputJSON)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>outputJSONSync (file, data, options)](#apidoc.element.fs-promise.outputJSONSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>outputJson ()](#apidoc.element.fs-promise.outputJson)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>outputJsonSync (file, data, options)](#apidoc.element.fs-promise.outputJsonSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>read ()](#apidoc.element.fs-promise.read)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>readFile ()](#apidoc.element.fs-promise.readFile)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>readFileSync (path, options)](#apidoc.element.fs-promise.readFileSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>readJSON ()](#apidoc.element.fs-promise.readJSON)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>readJSONSync (file, options)](#apidoc.element.fs-promise.readJSONSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>readJson ()](#apidoc.element.fs-promise.readJson)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>readJsonSync (file, options)](#apidoc.element.fs-promise.readJsonSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>readSync (fd, buffer, offset, length, position)](#apidoc.element.fs-promise.readSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>readdir ()](#apidoc.element.fs-promise.readdir)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>readdirSync (path, options)](#apidoc.element.fs-promise.readdirSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>readlink ()](#apidoc.element.fs-promise.readlink)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>readlinkSync (path, options)](#apidoc.element.fs-promise.readlinkSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>realpath ()](#apidoc.element.fs-promise.realpath)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>realpathSync (p, options)](#apidoc.element.fs-promise.realpathSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>remove ()](#apidoc.element.fs-promise.remove)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>removeSync (dir)](#apidoc.element.fs-promise.removeSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>rename ()](#apidoc.element.fs-promise.rename)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>renameSync (oldPath, newPath)](#apidoc.element.fs-promise.renameSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>rmdir ()](#apidoc.element.fs-promise.rmdir)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>rmdirSync (path)](#apidoc.element.fs-promise.rmdirSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>stat ()](#apidoc.element.fs-promise.stat)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>statSync (target)](#apidoc.element.fs-promise.statSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>symlink ()](#apidoc.element.fs-promise.symlink)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>symlinkSync (target, path, type)](#apidoc.element.fs-promise.symlinkSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>truncate ()](#apidoc.element.fs-promise.truncate)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>truncateSync (path, len)](#apidoc.element.fs-promise.truncateSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>unlink ()](#apidoc.element.fs-promise.unlink)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>unlinkSync (path)](#apidoc.element.fs-promise.unlinkSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>unwatchFile (filename, listener)](#apidoc.element.fs-promise.unwatchFile)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>utimes ()](#apidoc.element.fs-promise.utimes)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>utimesSync (path, atime, mtime)](#apidoc.element.fs-promise.utimesSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>watch (filename, options, listener)](#apidoc.element.fs-promise.watch)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>watchFile (filename, options, listener)](#apidoc.element.fs-promise.watchFile)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>write ()](#apidoc.element.fs-promise.write)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>writeFile ()](#apidoc.element.fs-promise.writeFile)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>writeFileSync (path, data, options)](#apidoc.element.fs-promise.writeFileSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>writeJSON ()](#apidoc.element.fs-promise.writeJSON)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>writeJSONSync (file, obj, options)](#apidoc.element.fs-promise.writeJSONSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>writeJson ()](#apidoc.element.fs-promise.writeJson)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>writeJsonSync (file, obj, options)](#apidoc.element.fs-promise.writeJsonSync)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>writeSync (fd, buffer, offset, length, position)](#apidoc.element.fs-promise.writeSync)
1.  number <span class="apidocSignatureSpan">fs-promise.</span>F_OK
1.  number <span class="apidocSignatureSpan">fs-promise.</span>R_OK
1.  number <span class="apidocSignatureSpan">fs-promise.</span>W_OK
1.  number <span class="apidocSignatureSpan">fs-promise.</span>X_OK
1.  number <span class="apidocSignatureSpan">fs-promise.</span>spaces
1.  object <span class="apidocSignatureSpan">fs-promise.</span>ReadStream.prototype
1.  object <span class="apidocSignatureSpan">fs-promise.</span>Stats.prototype
1.  object <span class="apidocSignatureSpan">fs-promise.</span>WriteStream.prototype
1.  object <span class="apidocSignatureSpan">fs-promise.</span>constants
1.  object <span class="apidocSignatureSpan">fs-promise.</span>jsonfile

#### [module fs-promise.ReadStream](#apidoc.module.fs-promise.ReadStream)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>ReadStream (path, options)](#apidoc.element.fs-promise.ReadStream.ReadStream)

#### [module fs-promise.ReadStream.prototype](#apidoc.module.fs-promise.ReadStream.prototype)
1.  [function <span class="apidocSignatureSpan">fs-promise.ReadStream.prototype.</span>open ()](#apidoc.element.fs-promise.ReadStream.prototype.open)

#### [module fs-promise.Stats](#apidoc.module.fs-promise.Stats)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>Stats ( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec)](#apidoc.element.fs-promise.Stats.Stats)

#### [module fs-promise.Stats.prototype](#apidoc.module.fs-promise.Stats.prototype)
1.  [function <span class="apidocSignatureSpan">fs-promise.Stats.prototype.</span>_checkModeProperty (property)](#apidoc.element.fs-promise.Stats.prototype._checkModeProperty)
1.  [function <span class="apidocSignatureSpan">fs-promise.Stats.prototype.</span>isBlockDevice ()](#apidoc.element.fs-promise.Stats.prototype.isBlockDevice)
1.  [function <span class="apidocSignatureSpan">fs-promise.Stats.prototype.</span>isCharacterDevice ()](#apidoc.element.fs-promise.Stats.prototype.isCharacterDevice)
1.  [function <span class="apidocSignatureSpan">fs-promise.Stats.prototype.</span>isDirectory ()](#apidoc.element.fs-promise.Stats.prototype.isDirectory)
1.  [function <span class="apidocSignatureSpan">fs-promise.Stats.prototype.</span>isFIFO ()](#apidoc.element.fs-promise.Stats.prototype.isFIFO)
1.  [function <span class="apidocSignatureSpan">fs-promise.Stats.prototype.</span>isFile ()](#apidoc.element.fs-promise.Stats.prototype.isFile)
1.  [function <span class="apidocSignatureSpan">fs-promise.Stats.prototype.</span>isSocket ()](#apidoc.element.fs-promise.Stats.prototype.isSocket)
1.  [function <span class="apidocSignatureSpan">fs-promise.Stats.prototype.</span>isSymbolicLink ()](#apidoc.element.fs-promise.Stats.prototype.isSymbolicLink)

#### [module fs-promise.WriteStream](#apidoc.module.fs-promise.WriteStream)
1.  [function <span class="apidocSignatureSpan">fs-promise.</span>WriteStream (path, options)](#apidoc.element.fs-promise.WriteStream.WriteStream)

#### [module fs-promise.WriteStream.prototype](#apidoc.module.fs-promise.WriteStream.prototype)
1.  [function <span class="apidocSignatureSpan">fs-promise.WriteStream.prototype.</span>open ()](#apidoc.element.fs-promise.WriteStream.prototype.open)



# <a name="apidoc.module.fs-promise"></a>[module fs-promise](#apidoc.module.fs-promise)

#### <a name="apidoc.element.fs-promise.FileReadStream"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>FileReadStream (path, options)](#apidoc.element.fs-promise.FileReadStream)
- description and source-code
```javascript
function ReadStream(path, options) {
  if (this instanceof ReadStream)
    return fs$ReadStream.apply(this, arguments), this
  else
    return ReadStream.apply(Object.create(ReadStream.prototype), arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.FileWriteStream"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>FileWriteStream (path, options)](#apidoc.element.fs-promise.FileWriteStream)
- description and source-code
```javascript
function WriteStream(path, options) {
  if (this instanceof WriteStream)
    return fs$WriteStream.apply(this, arguments), this
  else
    return WriteStream.apply(Object.create(WriteStream.prototype), arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.ReadStream"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>ReadStream (path, options)](#apidoc.element.fs-promise.ReadStream)
- description and source-code
```javascript
function ReadStream(path, options) {
  if (this instanceof ReadStream)
    return fs$ReadStream.apply(this, arguments), this
  else
    return ReadStream.apply(Object.create(ReadStream.prototype), arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.Stats"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>Stats ( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec)](#apidoc.element.fs-promise.Stats)
- description and source-code
```javascript
function Stats( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec) {
  this.dev = dev;
  this.mode = mode;
  this.nlink = nlink;
  this.uid = uid;
  this.gid = gid;
  this.rdev = rdev;
  this.blksize = blksize;
  this.ino = ino;
  this.size = size;
  this.blocks = blocks;
  this.atime = new Date(atim_msec);
  this.mtime = new Date(mtim_msec);
  this.ctime = new Date(ctim_msec);
  this.birthtime = new Date(birthtim_msec);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.WriteStream"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>WriteStream (path, options)](#apidoc.element.fs-promise.WriteStream)
- description and source-code
```javascript
function WriteStream(path, options) {
  if (this instanceof WriteStream)
    return fs$WriteStream.apply(this, arguments), this
  else
    return WriteStream.apply(Object.create(WriteStream.prototype), arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise._toUnixTimestamp"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>_toUnixTimestamp (time)](#apidoc.element.fs-promise._toUnixTimestamp)
- description and source-code
```javascript
function toUnixTimestamp(time) {
  if (typeof time === 'string' && +time == time) {
    return +time;
  }
  if (typeof time === 'number') {
    if (!Number.isFinite(time) || time < 0) {
      return Date.now() / 1000;
    }
    return time;
  }
  if (util.isDate(time)) {
    // convert to 123.456 UNIX timestamp
    return time.getTime() / 1000;
  }
  throw new Error('Cannot parse time: ' + time);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.access"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>access ()](#apidoc.element.fs-promise.access)
- description and source-code
```javascript
access = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.accessSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>accessSync (path, mode)](#apidoc.element.fs-promise.accessSync)
- description and source-code
```javascript
accessSync = function (path, mode) {
  nullCheck(path);

  if (mode === undefined)
    mode = fs.F_OK;
  else
    mode = mode | 0;

  binding.access(pathModule._makeLong(path), mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.appendFile"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>appendFile ()](#apidoc.element.fs-promise.appendFile)
- description and source-code
```javascript
function appendFile() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.appendFileSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>appendFileSync (path, data, options)](#apidoc.element.fs-promise.appendFileSync)
- description and source-code
```javascript
appendFileSync = function (path, data, options) {
  if (!options) {
    options = { encoding: 'utf8', mode: 0o666, flag: 'a' };
  } else if (typeof options === 'string') {
    options = { encoding: options, mode: 0o666, flag: 'a' };
  } else if (typeof options !== 'object') {
    throwOptionsError(options);
  }

  if (!options.flag)
    options = util._extend({ flag: 'a' }, options);

  // force append behavior when using a supplied file descriptor
  if (isFd(path))
    options.flag = 'a';

  fs.writeFileSync(path, data, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.chmod"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>chmod ()](#apidoc.element.fs-promise.chmod)
- description and source-code
```javascript
chmod = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.chmodSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>chmodSync (target, mode)](#apidoc.element.fs-promise.chmodSync)
- description and source-code
```javascript
chmodSync = function (target, mode) {
  try {
    return orig.call(fs, target, mode)
  } catch (er) {
    if (!chownErOk(er)) throw er
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.chown"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>chown ()](#apidoc.element.fs-promise.chown)
- description and source-code
```javascript
chown = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.chownSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>chownSync (target, uid, gid)](#apidoc.element.fs-promise.chownSync)
- description and source-code
```javascript
chownSync = function (target, uid, gid) {
  try {
    return orig.call(fs, target, uid, gid)
  } catch (er) {
    if (!chownErOk(er)) throw er
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.close"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>close ()](#apidoc.element.fs-promise.close)
- description and source-code
```javascript
close = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.closeSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>closeSync (fd)](#apidoc.element.fs-promise.closeSync)
- description and source-code
```javascript
closeSync = function (fd) {
  // Note that graceful-fs also retries when fs.closeSync() fails.
  // Looks like a bug to me, although it's probably a harmless one.
  var rval = fs$closeSync.apply(fs, arguments)
  retry()
  return rval
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.copy"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>copy ()](#apidoc.element.fs-promise.copy)
- description and source-code
```javascript
function copy() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.copySync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>copySync (src, dest, options)](#apidoc.element.fs-promise.copySync)
- description and source-code
```javascript
function copySync(src, dest, options) {
  if (typeof options === 'function' || options instanceof RegExp) {
    options = {filter: options}
  }

  options = options || {}
  options.recursive = !!options.recursive

  // default to true for now
  options.clobber = 'clobber' in options ? !!options.clobber : true
  // overwrite falls back to clobber
  options.overwrite = 'overwrite' in options ? !!options.overwrite : options.clobber
  options.dereference = 'dereference' in options ? !!options.dereference : false
  options.preserveTimestamps = 'preserveTimestamps' in options ? !!options.preserveTimestamps : false

  options.filter = options.filter || function () { return true }

  // Warn about using preserveTimestamps on 32-bit node:
  if (options.preserveTimestamps && process.arch === 'ia32') {
    console.warn('fs-extra: Using the preserveTimestamps option in 32-bit node is not recommended;\n
    see https://github.com/jprichardson/node-fs-extra/issues/269')
  }

  const stats = (options.recursive && !options.dereference) ? fs.lstatSync(src) : fs.statSync(src)
  const destFolder = path.dirname(dest)
  const destFolderExists = fs.existsSync(destFolder)
  let performCopy = false

  if (options.filter instanceof RegExp) {
    console.warn('Warning: fs-extra: Passing a RegExp filter is deprecated, use a function')
    performCopy = options.filter.test(src)
  } else if (typeof options.filter === 'function') performCopy = options.filter(src, dest)

  if (stats.isFile() && performCopy) {
    if (!destFolderExists) mkdir.mkdirsSync(destFolder)
    copyFileSync(src, dest, {
      overwrite: options.overwrite,
      errorOnExist: options.errorOnExist,
      preserveTimestamps: options.preserveTimestamps
    })
  } else if (stats.isDirectory() && performCopy) {
    if (!fs.existsSync(dest)) mkdir.mkdirsSync(dest)
    const contents = fs.readdirSync(src)
    contents.forEach(content => {
      const opts = options
      opts.recursive = true
      copySync(path.join(src, content), path.join(dest, content), opts)
    })
  } else if (options.recursive && stats.isSymbolicLink() && performCopy) {
    const srcPath = fs.readlinkSync(src)
    fs.symlinkSync(srcPath, dest)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.createFile"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>createFile ()](#apidoc.element.fs-promise.createFile)
- description and source-code
```javascript
function createFile() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.createFileSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>createFileSync (file)](#apidoc.element.fs-promise.createFileSync)
- description and source-code
```javascript
function createFileSync(file) {
  if (fs.existsSync(file)) return

  const dir = path.dirname(file)
  if (!fs.existsSync(dir)) {
    mkdir.mkdirsSync(dir)
  }

  fs.writeFileSync(file, '')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.createLink"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>createLink ()](#apidoc.element.fs-promise.createLink)
- description and source-code
```javascript
function createLink() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.createLinkSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>createLinkSync (srcpath, dstpath, callback)](#apidoc.element.fs-promise.createLinkSync)
- description and source-code
```javascript
function createLinkSync(srcpath, dstpath, callback) {
  const destinationExists = fs.existsSync(dstpath)
  if (destinationExists) return undefined

  try {
    fs.lstatSync(srcpath)
  } catch (err) {
    err.message = err.message.replace('lstat', 'ensureLink')
    throw err
  }

  const dir = path.dirname(dstpath)
  const dirExists = fs.existsSync(dir)
  if (dirExists) return fs.linkSync(srcpath, dstpath)
  mkdir.mkdirsSync(dir)

  return fs.linkSync(srcpath, dstpath)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.createReadStream"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>createReadStream (path, options)](#apidoc.element.fs-promise.createReadStream)
- description and source-code
```javascript
function createReadStream(path, options) {
  return new ReadStream(path, options)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.createSymlink"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>createSymlink ()](#apidoc.element.fs-promise.createSymlink)
- description and source-code
```javascript
function createSymlink() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.createSymlinkSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>createSymlinkSync (srcpath, dstpath, type, callback)](#apidoc.element.fs-promise.createSymlinkSync)
- description and source-code
```javascript
function createSymlinkSync(srcpath, dstpath, type, callback) {
  callback = (typeof type === 'function') ? type : callback
  type = (typeof type === 'function') ? false : type

  const destinationExists = fs.existsSync(dstpath)
  if (destinationExists) return undefined

  const relative = symlinkPathsSync(srcpath, dstpath)
  srcpath = relative.toDst
  type = symlinkTypeSync(relative.toCwd, type)
  const dir = path.dirname(dstpath)
  const exists = fs.existsSync(dir)
  if (exists) return fs.symlinkSync(srcpath, dstpath, type)
  mkdirsSync(dir)
  return fs.symlinkSync(srcpath, dstpath, type)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.createWriteStream"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>createWriteStream (path, options)](#apidoc.element.fs-promise.createWriteStream)
- description and source-code
```javascript
function createWriteStream(path, options) {
  return new WriteStream(path, options)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.emptyDir"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>emptyDir ()](#apidoc.element.fs-promise.emptyDir)
- description and source-code
```javascript
function emptyDir() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.emptyDirSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>emptyDirSync (dir)](#apidoc.element.fs-promise.emptyDirSync)
- description and source-code
```javascript
function emptyDirSync(dir) {
  let items
  try {
    items = fs.readdirSync(dir)
  } catch (err) {
    return mkdir.mkdirsSync(dir)
  }

  items.forEach(item => {
    item = path.join(dir, item)
    remove.removeSync(item)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.emptydir"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>emptydir ()](#apidoc.element.fs-promise.emptydir)
- description and source-code
```javascript
function emptyDir() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.emptydirSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>emptydirSync (dir)](#apidoc.element.fs-promise.emptydirSync)
- description and source-code
```javascript
function emptyDirSync(dir) {
  let items
  try {
    items = fs.readdirSync(dir)
  } catch (err) {
    return mkdir.mkdirsSync(dir)
  }

  items.forEach(item => {
    item = path.join(dir, item)
    remove.removeSync(item)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.ensureDir"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>ensureDir ()](#apidoc.element.fs-promise.ensureDir)
- description and source-code
```javascript
function mkdirs() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.ensureDirSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>ensureDirSync (p, opts, made)](#apidoc.element.fs-promise.ensureDirSync)
- description and source-code
```javascript
function mkdirsSync(p, opts, made) {
  if (!opts || typeof opts !== 'object') {
    opts = { mode: opts }
  }

  let mode = opts.mode
  const xfs = opts.fs || fs

  if (process.platform === 'win32' && invalidWin32Path(p)) {
    const errInval = new Error(p + ' contains invalid WIN32 path characters.')
    errInval.code = 'EINVAL'
    throw errInval
  }

  if (mode === undefined) {
    mode = o777 & (~process.umask())
  }
  if (!made) made = null

  p = path.resolve(p)

  try {
    xfs.mkdirSync(p, mode)
    made = made || p
  } catch (err0) {
    switch (err0.code) {
      case 'ENOENT':
        if (path.dirname(p) === p) throw err0
        made = mkdirsSync(path.dirname(p), opts, made)
        mkdirsSync(p, opts, made)
        break

      // In the case of any other error, just see if there's a dir
      // there already.  If so, then hooray!  If not, then something
      // is borked.
      default:
        let stat
        try {
          stat = xfs.statSync(p)
        } catch (err1) {
          throw err0
        }
        if (!stat.isDirectory()) throw err0
        break
    }
  }

  return made
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.ensureFile"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>ensureFile ()](#apidoc.element.fs-promise.ensureFile)
- description and source-code
```javascript
function createFile() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.ensureFileSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>ensureFileSync (file)](#apidoc.element.fs-promise.ensureFileSync)
- description and source-code
```javascript
function createFileSync(file) {
  if (fs.existsSync(file)) return

  const dir = path.dirname(file)
  if (!fs.existsSync(dir)) {
    mkdir.mkdirsSync(dir)
  }

  fs.writeFileSync(file, '')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.ensureLink"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>ensureLink ()](#apidoc.element.fs-promise.ensureLink)
- description and source-code
```javascript
function createLink() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.ensureLinkSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>ensureLinkSync (srcpath, dstpath, callback)](#apidoc.element.fs-promise.ensureLinkSync)
- description and source-code
```javascript
function createLinkSync(srcpath, dstpath, callback) {
  const destinationExists = fs.existsSync(dstpath)
  if (destinationExists) return undefined

  try {
    fs.lstatSync(srcpath)
  } catch (err) {
    err.message = err.message.replace('lstat', 'ensureLink')
    throw err
  }

  const dir = path.dirname(dstpath)
  const dirExists = fs.existsSync(dir)
  if (dirExists) return fs.linkSync(srcpath, dstpath)
  mkdir.mkdirsSync(dir)

  return fs.linkSync(srcpath, dstpath)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.ensureSymlink"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>ensureSymlink ()](#apidoc.element.fs-promise.ensureSymlink)
- description and source-code
```javascript
function createSymlink() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.ensureSymlinkSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>ensureSymlinkSync (srcpath, dstpath, type, callback)](#apidoc.element.fs-promise.ensureSymlinkSync)
- description and source-code
```javascript
function createSymlinkSync(srcpath, dstpath, type, callback) {
  callback = (typeof type === 'function') ? type : callback
  type = (typeof type === 'function') ? false : type

  const destinationExists = fs.existsSync(dstpath)
  if (destinationExists) return undefined

  const relative = symlinkPathsSync(srcpath, dstpath)
  srcpath = relative.toDst
  type = symlinkTypeSync(relative.toCwd, type)
  const dir = path.dirname(dstpath)
  const exists = fs.existsSync(dir)
  if (exists) return fs.symlinkSync(srcpath, dstpath, type)
  mkdirsSync(dir)
  return fs.symlinkSync(srcpath, dstpath, type)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.exists"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>exists (filename, callback)](#apidoc.element.fs-promise.exists)
- description and source-code
```javascript
exists = function (filename, callback) {
  // callback
  if (typeof callback === 'function') {
    return fs.stat(filename, function (err) {
      callback(null, !err);
    })
  }
  // or promise
  return new Promise(function (resolve) {
    fs.stat(filename, function (err) {
      resolve(!err)
    })
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.existsSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>existsSync (path)](#apidoc.element.fs-promise.existsSync)
- description and source-code
```javascript
existsSync = function (path) {
  try {
    nullCheck(path);
    binding.stat(pathModule._makeLong(path), statValues);
    return true;
  } catch (e) {
    return false;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.fchmod"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>fchmod ()](#apidoc.element.fs-promise.fchmod)
- description and source-code
```javascript
fchmod = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.fchmodSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>fchmodSync (target, mode)](#apidoc.element.fs-promise.fchmodSync)
- description and source-code
```javascript
fchmodSync = function (target, mode) {
  try {
    return orig.call(fs, target, mode)
  } catch (er) {
    if (!chownErOk(er)) throw er
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.fchown"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>fchown ()](#apidoc.element.fs-promise.fchown)
- description and source-code
```javascript
fchown = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.fchownSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>fchownSync (target, uid, gid)](#apidoc.element.fs-promise.fchownSync)
- description and source-code
```javascript
fchownSync = function (target, uid, gid) {
  try {
    return orig.call(fs, target, uid, gid)
  } catch (er) {
    if (!chownErOk(er)) throw er
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.fdatasync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>fdatasync ()](#apidoc.element.fs-promise.fdatasync)
- description and source-code
```javascript
fdatasync = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.fdatasyncSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>fdatasyncSync (fd)](#apidoc.element.fs-promise.fdatasyncSync)
- description and source-code
```javascript
fdatasyncSync = function (fd) {
  return binding.fdatasync(fd);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.fstat"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>fstat ()](#apidoc.element.fs-promise.fstat)
- description and source-code
```javascript
fstat = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.fstatSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>fstatSync (target)](#apidoc.element.fs-promise.fstatSync)
- description and source-code
```javascript
fstatSync = function (target) {
  var stats = orig.call(fs, target)
  if (stats.uid < 0) stats.uid += 0x100000000
  if (stats.gid < 0) stats.gid += 0x100000000
  return stats;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.fsync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>fsync ()](#apidoc.element.fs-promise.fsync)
- description and source-code
```javascript
fsync = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.fsyncSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>fsyncSync (fd)](#apidoc.element.fs-promise.fsyncSync)
- description and source-code
```javascript
fsyncSync = function (fd) {
  return binding.fsync(fd);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.ftruncate"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>ftruncate ()](#apidoc.element.fs-promise.ftruncate)
- description and source-code
```javascript
ftruncate = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.ftruncateSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>ftruncateSync (fd, len)](#apidoc.element.fs-promise.ftruncateSync)
- description and source-code
```javascript
ftruncateSync = function (fd, len) {
  if (len === undefined) {
    len = 0;
  }
  return binding.ftruncate(fd, len);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.futimes"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>futimes ()](#apidoc.element.fs-promise.futimes)
- description and source-code
```javascript
futimes = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.futimesSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>futimesSync (fd, atime, mtime)](#apidoc.element.fs-promise.futimesSync)
- description and source-code
```javascript
futimesSync = function (fd, atime, mtime) {
  atime = toUnixTimestamp(atime);
  mtime = toUnixTimestamp(mtime);
  binding.futimes(fd, atime, mtime);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.gracefulify"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>gracefulify (fs)](#apidoc.element.fs-promise.gracefulify)
- description and source-code
```javascript
function patch(fs) {
  // Everything that references the open() function needs to be in here
  polyfills(fs)
  fs.gracefulify = patch
  fs.FileReadStream = ReadStream;  // Legacy name.
  fs.FileWriteStream = WriteStream;  // Legacy name.
  fs.createReadStream = createReadStream
  fs.createWriteStream = createWriteStream
  var fs$readFile = fs.readFile
  fs.readFile = readFile
  function readFile (path, options, cb) {
    if (typeof options === 'function')
      cb = options, options = null

    return go$readFile(path, options, cb)

    function go$readFile (path, options, cb) {
      return fs$readFile(path, options, function (err) {
        if (err && (err.code === 'EMFILE' || err.code === 'ENFILE'))
          enqueue([go$readFile, [path, options, cb]])
        else {
          if (typeof cb === 'function')
            cb.apply(this, arguments)
          retry()
        }
      })
    }
  }

  var fs$writeFile = fs.writeFile
  fs.writeFile = writeFile
  function writeFile (path, data, options, cb) {
    if (typeof options === 'function')
      cb = options, options = null

    return go$writeFile(path, data, options, cb)

    function go$writeFile (path, data, options, cb) {
      return fs$writeFile(path, data, options, function (err) {
        if (err && (err.code === 'EMFILE' || err.code === 'ENFILE'))
          enqueue([go$writeFile, [path, data, options, cb]])
        else {
          if (typeof cb === 'function')
            cb.apply(this, arguments)
          retry()
        }
      })
    }
  }

  var fs$appendFile = fs.appendFile
  if (fs$appendFile)
    fs.appendFile = appendFile
  function appendFile (path, data, options, cb) {
    if (typeof options === 'function')
      cb = options, options = null

    return go$appendFile(path, data, options, cb)

    function go$appendFile (path, data, options, cb) {
      return fs$appendFile(path, data, options, function (err) {
        if (err && (err.code === 'EMFILE' || err.code === 'ENFILE'))
          enqueue([go$appendFile, [path, data, options, cb]])
        else {
          if (typeof cb === 'function')
            cb.apply(this, arguments)
          retry()
        }
      })
    }
  }

  var fs$readdir = fs.readdir
  fs.readdir = readdir
  function readdir (path, options, cb) {
    var args = [path]
    if (typeof options !== 'function') {
      args.push(options)
    } else {
      cb = options
    }
    args.push(go$readdir$cb)

    return go$readdir(args)

    function go$readdir$cb (err, files) {
      if (files && files.sort)
        files.sort()

      if (err && (err.code === 'EMFILE' || err.code === 'ENFILE'))
        enqueue([go$readdir, [args]])
      else {
        if (typeof cb === 'function')
          cb.apply(this, arguments)
        retry()
      }
    }
  }

  function go$readdir (args) {
    return fs$readdir.apply(fs, args)
  }

  if (process.version.substr(0, 4) === 'v0.8') {
    var legStreams = legacy(fs)
    ReadStream = legStreams.ReadStream
    WriteStream = legStreams.WriteStream
  }

  var fs$ReadStream = fs.ReadStream
  ReadStream.prototype = Object.create(fs$ReadStream.prototype)
  ReadStream.prototype.open = ReadStream$open

  var fs$WriteStream = fs.WriteStream
  WriteStream.prototype = Object.create(fs$WriteStream.prototype)
  WriteStream.prototype.open = WriteStream$open

  fs.ReadStream = ReadStream
  fs.WriteStream = WriteStream

  function ReadStream (path, options) {
    if (this instanceof ReadStream)
      return fs$ReadStream.apply(this, arguments), this
    else
      return ReadStream.apply(Object.create(ReadStream.prototype), arguments)
  }

  function ReadStream$open () {
    var that = this
    open(that.path, that.flags, that.mode, function (err, fd) {
      if (err) {
        if (that.autoClose)
          that.destroy()

        that.emit('error', err)
      } else {
        that.fd = fd
        that.emit('open', fd)
        that.read()
      }
    })
  }

  function WriteStream (path, options) {
    if (this instanceof WriteStream)
      return fs$WriteStream.apply(this, arguments), this
    else
      return W ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.lchmod"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>lchmod (path, mode, cb)](#apidoc.element.fs-promise.lchmod)
- description and source-code
```javascript
lchmod = function (path, mode, cb) {
  if (cb) process.nextTick(cb)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.lchmodSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>lchmodSync ()](#apidoc.element.fs-promise.lchmodSync)
- description and source-code
```javascript
lchmodSync = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.lchown"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>lchown ()](#apidoc.element.fs-promise.lchown)
- description and source-code
```javascript
lchown = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.lchownSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>lchownSync ()](#apidoc.element.fs-promise.lchownSync)
- description and source-code
```javascript
lchownSync = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.link"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>link ()](#apidoc.element.fs-promise.link)
- description and source-code
```javascript
link = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.linkSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>linkSync (existingPath, newPath)](#apidoc.element.fs-promise.linkSync)
- description and source-code
```javascript
linkSync = function (existingPath, newPath) {
  nullCheck(existingPath);
  nullCheck(newPath);
  return binding.link(pathModule._makeLong(existingPath),
                      pathModule._makeLong(newPath));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.lstat"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>lstat ()](#apidoc.element.fs-promise.lstat)
- description and source-code
```javascript
lstat = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.lstatSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>lstatSync (target)](#apidoc.element.fs-promise.lstatSync)
- description and source-code
```javascript
lstatSync = function (target) {
  var stats = orig.call(fs, target)
  if (stats.uid < 0) stats.uid += 0x100000000
  if (stats.gid < 0) stats.gid += 0x100000000
  return stats;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.lutimes"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>lutimes (_a, _b, _c, cb)](#apidoc.element.fs-promise.lutimes)
- description and source-code
```javascript
lutimes = function (_a, _b, _c, cb) { if (cb) process.nextTick(cb) }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.lutimesSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>lutimesSync ()](#apidoc.element.fs-promise.lutimesSync)
- description and source-code
```javascript
lutimesSync = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.mkdir"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>mkdir ()](#apidoc.element.fs-promise.mkdir)
- description and source-code
```javascript
mkdir = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.mkdirSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>mkdirSync (path, mode)](#apidoc.element.fs-promise.mkdirSync)
- description and source-code
```javascript
mkdirSync = function (path, mode) {
  nullCheck(path);
  return binding.mkdir(pathModule._makeLong(path),
                       modeNum(mode, 0o777));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.mkdirp"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>mkdirp ()](#apidoc.element.fs-promise.mkdirp)
- description and source-code
```javascript
function mkdirs() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.mkdirpSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>mkdirpSync (p, opts, made)](#apidoc.element.fs-promise.mkdirpSync)
- description and source-code
```javascript
function mkdirsSync(p, opts, made) {
  if (!opts || typeof opts !== 'object') {
    opts = { mode: opts }
  }

  let mode = opts.mode
  const xfs = opts.fs || fs

  if (process.platform === 'win32' && invalidWin32Path(p)) {
    const errInval = new Error(p + ' contains invalid WIN32 path characters.')
    errInval.code = 'EINVAL'
    throw errInval
  }

  if (mode === undefined) {
    mode = o777 & (~process.umask())
  }
  if (!made) made = null

  p = path.resolve(p)

  try {
    xfs.mkdirSync(p, mode)
    made = made || p
  } catch (err0) {
    switch (err0.code) {
      case 'ENOENT':
        if (path.dirname(p) === p) throw err0
        made = mkdirsSync(path.dirname(p), opts, made)
        mkdirsSync(p, opts, made)
        break

      // In the case of any other error, just see if there's a dir
      // there already.  If so, then hooray!  If not, then something
      // is borked.
      default:
        let stat
        try {
          stat = xfs.statSync(p)
        } catch (err1) {
          throw err0
        }
        if (!stat.isDirectory()) throw err0
        break
    }
  }

  return made
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.mkdirs"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>mkdirs ()](#apidoc.element.fs-promise.mkdirs)
- description and source-code
```javascript
function mkdirs() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.mkdirsSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>mkdirsSync (p, opts, made)](#apidoc.element.fs-promise.mkdirsSync)
- description and source-code
```javascript
function mkdirsSync(p, opts, made) {
  if (!opts || typeof opts !== 'object') {
    opts = { mode: opts }
  }

  let mode = opts.mode
  const xfs = opts.fs || fs

  if (process.platform === 'win32' && invalidWin32Path(p)) {
    const errInval = new Error(p + ' contains invalid WIN32 path characters.')
    errInval.code = 'EINVAL'
    throw errInval
  }

  if (mode === undefined) {
    mode = o777 & (~process.umask())
  }
  if (!made) made = null

  p = path.resolve(p)

  try {
    xfs.mkdirSync(p, mode)
    made = made || p
  } catch (err0) {
    switch (err0.code) {
      case 'ENOENT':
        if (path.dirname(p) === p) throw err0
        made = mkdirsSync(path.dirname(p), opts, made)
        mkdirsSync(p, opts, made)
        break

      // In the case of any other error, just see if there's a dir
      // there already.  If so, then hooray!  If not, then something
      // is borked.
      default:
        let stat
        try {
          stat = xfs.statSync(p)
        } catch (err1) {
          throw err0
        }
        if (!stat.isDirectory()) throw err0
        break
    }
  }

  return made
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.mkdtemp"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>mkdtemp ()](#apidoc.element.fs-promise.mkdtemp)
- description and source-code
```javascript
mkdtemp = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.mkdtempSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>mkdtempSync (prefix, options)](#apidoc.element.fs-promise.mkdtempSync)
- description and source-code
```javascript
mkdtempSync = function (prefix, options) {
  if (!prefix || typeof prefix !== 'string')
    throw new TypeError('filename prefix is required');

  options = options || {};
  if (typeof options === 'string')
    options = {encoding: options};
  if (typeof options !== 'object')
    throw new TypeError('"options" must be a string or an object');
  nullCheck(prefix);

  return binding.mkdtemp(prefix + 'XXXXXX', options.encoding);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.move"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>move ()](#apidoc.element.fs-promise.move)
- description and source-code
```javascript
function move() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.moveSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>moveSync (src, dest, options)](#apidoc.element.fs-promise.moveSync)
- description and source-code
```javascript
function moveSync(src, dest, options) {
  options = options || {}
  const overwrite = options.overwrite || options.clobber || false

  src = path.resolve(src)
  dest = path.resolve(dest)

  if (src === dest) return

  if (isSrcSubdir(src, dest)) throw new Error('Cannot move '${src}' into itself '${dest}'.')

  mkdirpSync(path.dirname(dest))
  tryRenameSync()

  function tryRenameSync () {
    if (overwrite) {
      try {
        return fs.renameSync(src, dest)
      } catch (err) {
        if (err.code === 'ENOTEMPTY' || err.code === 'EEXIST' || err.code === 'EPERM') {
          removeSync(dest)
          options.overwrite = false // just overwriteed it, no need to do it again
          return moveSync(src, dest, options)
        }

        if (err.code !== 'EXDEV') throw err
        return moveSyncAcrossDevice(src, dest, overwrite)
      }
    } else {
      try {
        fs.linkSync(src, dest)
        return fs.unlinkSync(src)
      } catch (err) {
        if (err.code === 'EXDEV' || err.code === 'EISDIR' || err.code === 'EPERM' || err.code === 'ENOTSUP') {
          return moveSyncAcrossDevice(src, dest, overwrite)
        }
        throw err
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.open"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>open ()](#apidoc.element.fs-promise.open)
- description and source-code
```javascript
function open() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.openSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>openSync (path, flags, mode)](#apidoc.element.fs-promise.openSync)
- description and source-code
```javascript
openSync = function (path, flags, mode) {
  mode = modeNum(mode, 0o666);
  nullCheck(path);
  return binding.open(pathModule._makeLong(path), stringToFlags(flags), mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.outputFile"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>outputFile ()](#apidoc.element.fs-promise.outputFile)
- description and source-code
```javascript
function outputFile() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.outputFileSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>outputFileSync (file, data, encoding)](#apidoc.element.fs-promise.outputFileSync)
- description and source-code
```javascript
function outputFileSync(file, data, encoding) {
  const dir = path.dirname(file)
  if (fs.existsSync(dir)) {
    return fs.writeFileSync.apply(fs, arguments)
  }
  mkdir.mkdirsSync(dir)
  fs.writeFileSync.apply(fs, arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.outputJSON"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>outputJSON ()](#apidoc.element.fs-promise.outputJSON)
- description and source-code
```javascript
function outputJson() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.outputJSONSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>outputJSONSync (file, data, options)](#apidoc.element.fs-promise.outputJSONSync)
- description and source-code
```javascript
function outputJsonSync(file, data, options) {
  const dir = path.dirname(file)

  if (!fs.existsSync(dir)) {
    mkdir.mkdirsSync(dir)
  }

  jsonFile.writeJsonSync(file, data, options)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.outputJson"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>outputJson ()](#apidoc.element.fs-promise.outputJson)
- description and source-code
```javascript
function outputJson() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.outputJsonSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>outputJsonSync (file, data, options)](#apidoc.element.fs-promise.outputJsonSync)
- description and source-code
```javascript
function outputJsonSync(file, data, options) {
  const dir = path.dirname(file)

  if (!fs.existsSync(dir)) {
    mkdir.mkdirsSync(dir)
  }

  jsonFile.writeJsonSync(file, data, options)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.read"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>read ()](#apidoc.element.fs-promise.read)
- description and source-code
```javascript
read = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.readFile"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>readFile ()](#apidoc.element.fs-promise.readFile)
- description and source-code
```javascript
function readFile() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
...


'''javascript
var fsp = require('fs-promise');

fsp.writeFile('/tmp/hello1.txt', 'hello world')
  .then(function(){
    return fsp.readFile('/tmp/hello1.txt', {encoding:'utf8'});
  })
  .then(function(contents){});
'''

## Implementation

'fs-promise' is now a thin wrapper on top of ['mz/fs'][4] adding support for async functions from ['fs-extra'][2]. If you do not
 need the functions from 'fs-extra', consider using 'mz' directly.
...
```

#### <a name="apidoc.element.fs-promise.readFileSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>readFileSync (path, options)](#apidoc.element.fs-promise.readFileSync)
- description and source-code
```javascript
readFileSync = function (path, options) {
  if (!options) {
    options = { encoding: null, flag: 'r' };
  } else if (typeof options === 'string') {
    options = { encoding: options, flag: 'r' };
  } else if (typeof options !== 'object') {
    throwOptionsError(options);
  }

  var encoding = options.encoding;
  assertEncoding(encoding);

  var flag = options.flag || 'r';
  var isUserFd = isFd(path); // file descriptor ownership
  var fd = isUserFd ? path : fs.openSync(path, flag, 0o666);

  var st = tryStatSync(fd, isUserFd);
  var size = st.isFile() ? st.size : 0;
  var pos = 0;
  var buffer; // single buffer with file data
  var buffers; // list for when size is unknown

  if (size === 0) {
    buffers = [];
  } else {
    buffer = tryCreateBuffer(size, fd, isUserFd);
  }

  var bytesRead;

  if (size !== 0) {
    do {
      bytesRead = tryReadSync(fd, isUserFd, buffer, pos, size - pos);
      pos += bytesRead;
    } while (bytesRead !== 0 && pos < size);
  } else {
    do {
      // the kernel lies about many files.
      // Go ahead and try to read some bytes.
      buffer = Buffer.allocUnsafe(8192);
      bytesRead = tryReadSync(fd, isUserFd, buffer, 0, 8192);
      if (bytesRead !== 0) {
        buffers.push(buffer.slice(0, bytesRead));
      }
      pos += bytesRead;
    } while (bytesRead !== 0);
  }

  if (!isUserFd)
    fs.closeSync(fd);

  if (size === 0) {
    // data was collected into the buffers list.
    buffer = Buffer.concat(buffers, pos);
  } else if (pos < size) {
    buffer = buffer.slice(0, pos);
  }

  if (encoding) buffer = buffer.toString(encoding);
  return buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.readJSON"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>readJSON ()](#apidoc.element.fs-promise.readJSON)
- description and source-code
```javascript
function readFile() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.readJSONSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>readJSONSync (file, options)](#apidoc.element.fs-promise.readJSONSync)
- description and source-code
```javascript
function readFileSync(file, options) {
  options = options || {}
  if (typeof options === 'string') {
    options = {encoding: options}
  }

  var fs = options.fs || _fs

  var shouldThrow = true
  // DO NOT USE 'passParsingErrors' THE NAME WILL CHANGE!!!, use 'throws' instead
  if ('passParsingErrors' in options) {
    shouldThrow = options.passParsingErrors
  } else if ('throws' in options) {
    shouldThrow = options.throws
  }

  var content = fs.readFileSync(file, options)
  content = stripBom(content)

  try {
    return JSON.parse(content, options.reviver)
  } catch (err) {
    if (shouldThrow) {
      err.message = file + ': ' + err.message
      throw err
    } else {
      return null
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.readJson"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>readJson ()](#apidoc.element.fs-promise.readJson)
- description and source-code
```javascript
function readFile() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.readJsonSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>readJsonSync (file, options)](#apidoc.element.fs-promise.readJsonSync)
- description and source-code
```javascript
function readFileSync(file, options) {
  options = options || {}
  if (typeof options === 'string') {
    options = {encoding: options}
  }

  var fs = options.fs || _fs

  var shouldThrow = true
  // DO NOT USE 'passParsingErrors' THE NAME WILL CHANGE!!!, use 'throws' instead
  if ('passParsingErrors' in options) {
    shouldThrow = options.passParsingErrors
  } else if ('throws' in options) {
    shouldThrow = options.throws
  }

  var content = fs.readFileSync(file, options)
  content = stripBom(content)

  try {
    return JSON.parse(content, options.reviver)
  } catch (err) {
    if (shouldThrow) {
      err.message = file + ': ' + err.message
      throw err
    } else {
      return null
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.readSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>readSync (fd, buffer, offset, length, position)](#apidoc.element.fs-promise.readSync)
- description and source-code
```javascript
readSync = function (fd, buffer, offset, length, position) {
  var eagCounter = 0
  while (true) {
    try {
      return fs$readSync.call(fs, fd, buffer, offset, length, position)
    } catch (er) {
      if (er.code === 'EAGAIN' && eagCounter < 10) {
        eagCounter ++
        continue
      }
      throw er
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.readdir"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>readdir ()](#apidoc.element.fs-promise.readdir)
- description and source-code
```javascript
function readdir() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.readdirSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>readdirSync (path, options)](#apidoc.element.fs-promise.readdirSync)
- description and source-code
```javascript
readdirSync = function (path, options) {
  options = options || {};
  if (typeof options === 'string')
    options = {encoding: options};
  if (typeof options !== 'object')
    throw new TypeError('"options" must be a string or an object');
  nullCheck(path);
  return binding.readdir(pathModule._makeLong(path), options.encoding);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.readlink"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>readlink ()](#apidoc.element.fs-promise.readlink)
- description and source-code
```javascript
readlink = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.readlinkSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>readlinkSync (path, options)](#apidoc.element.fs-promise.readlinkSync)
- description and source-code
```javascript
readlinkSync = function (path, options) {
  options = options || {};
  if (typeof options === 'string')
    options = {encoding: options};
  if (typeof options !== 'object')
    throw new TypeError('"options" must be a string or an object');
  nullCheck(path);
  return binding.readlink(pathModule._makeLong(path), options.encoding);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.realpath"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>realpath ()](#apidoc.element.fs-promise.realpath)
- description and source-code
```javascript
function realpath() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.realpathSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>realpathSync (p, options)](#apidoc.element.fs-promise.realpathSync)
- description and source-code
```javascript
function realpathSync(p, options) {
  if (!options)
    options = {};
  else if (typeof options === 'string')
    options = {encoding: options};
  else if (typeof options !== 'object')
    throw new TypeError('"options" must be a string or an object');
  nullCheck(p);

  p = p.toString('utf8');
  p = pathModule.resolve(p);

  const seenLinks = {};
  const knownHard = {};
  const cache = options[realpathCacheKey];
  const original = p;

  const maybeCachedResult = cache && cache.get(p);
  if (maybeCachedResult) {
    return maybeCachedResult;
  }

  // current character position in p
  var pos;
  // the partial path so far, including a trailing slash if any
  var current;
  // the partial path without a trailing slash (except when pointing at a root)
  var base;
  // the partial path scanned in the previous round, with slash
  var previous;

  start();

  function start() {
    // Skip over roots
    var m = splitRootRe.exec(p);
    pos = m[0].length;
    current = m[0];
    base = m[0];
    previous = '';

    // On windows, check that the root exists. On unix there is no need.
    if (isWindows && !knownHard[base]) {
      fs.lstatSync(base);
      knownHard[base] = true;
    }
  }

  // walk down the path, swapping out linked pathparts for their real
  // values
  // NB: p.length changes.
  while (pos < p.length) {
    // find the next part
    nextPartRe.lastIndex = pos;
    var result = nextPartRe.exec(p);
    previous = current;
    current += result[0];
    base = previous + result[1];
    pos = nextPartRe.lastIndex;

    // continue if not a symlink
    if (knownHard[base] || (cache && cache.get(base) === base)) {
      continue;
    }

    var resolvedLink;
    const maybeCachedResolved = cache && cache.get(base);
    if (maybeCachedResolved) {
      resolvedLink = maybeCachedResolved;
    } else {
      var stat = fs.lstatSync(base);
      if (!stat.isSymbolicLink()) {
        knownHard[base] = true;
        if (cache) cache.set(base, base);
        continue;
      }

      // read the link if it wasn't read before
      // dev/ino always return 0 on windows, so skip the check.
      let linkTarget = null;
      let id;
      if (!isWindows) {
        id = '${stat.dev.toString(32)}:${stat.ino.toString(32)}';
        if (seenLinks.hasOwnProperty(id)) {
          linkTarget = seenLinks[id];
        }
      }
      if (linkTarget === null) {
        fs.statSync(base);
        linkTarget = fs.readlinkSync(base);
      }
      resolvedLink = pathModule.resolve(previous, linkTarget);

      if (cache) cache.set(base, resolvedLink);
      if (!isWindows) seenLinks[id] = linkTarget;
    }

    // resolve the link, then start over
    p = pathModule.resolve(resolvedLink, p.slice(pos));
    start();
  }

  if (cache) cache.set(original, p);
  return encodeRealpathResult(p, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.remove"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>remove ()](#apidoc.element.fs-promise.remove)
- description and source-code
```javascript
function remove() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.removeSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>removeSync (dir)](#apidoc.element.fs-promise.removeSync)
- description and source-code
```javascript
function removeSync(dir) {
  return rimraf.sync(dir, {disableGlob: true})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.rename"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>rename ()](#apidoc.element.fs-promise.rename)
- description and source-code
```javascript
rename = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.renameSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>renameSync (oldPath, newPath)](#apidoc.element.fs-promise.renameSync)
- description and source-code
```javascript
renameSync = function (oldPath, newPath) {
  nullCheck(oldPath);
  nullCheck(newPath);
  return binding.rename(pathModule._makeLong(oldPath),
                        pathModule._makeLong(newPath));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.rmdir"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>rmdir ()](#apidoc.element.fs-promise.rmdir)
- description and source-code
```javascript
rmdir = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.rmdirSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>rmdirSync (path)](#apidoc.element.fs-promise.rmdirSync)
- description and source-code
```javascript
rmdirSync = function (path) {
  nullCheck(path);
  return binding.rmdir(pathModule._makeLong(path));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.stat"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>stat ()](#apidoc.element.fs-promise.stat)
- description and source-code
```javascript
stat = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.statSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>statSync (target)](#apidoc.element.fs-promise.statSync)
- description and source-code
```javascript
statSync = function (target) {
  var stats = orig.call(fs, target)
  if (stats.uid < 0) stats.uid += 0x100000000
  if (stats.gid < 0) stats.gid += 0x100000000
  return stats;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.symlink"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>symlink ()](#apidoc.element.fs-promise.symlink)
- description and source-code
```javascript
symlink = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.symlinkSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>symlinkSync (target, path, type)](#apidoc.element.fs-promise.symlinkSync)
- description and source-code
```javascript
symlinkSync = function (target, path, type) {
  type = (typeof type === 'string' ? type : null);

  nullCheck(target);
  nullCheck(path);

  return binding.symlink(preprocessSymlinkDestination(target, type, path),
                         pathModule._makeLong(path),
                         type);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.truncate"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>truncate ()](#apidoc.element.fs-promise.truncate)
- description and source-code
```javascript
truncate = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.truncateSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>truncateSync (path, len)](#apidoc.element.fs-promise.truncateSync)
- description and source-code
```javascript
truncateSync = function (path, len) {
  if (typeof path === 'number') {
    // legacy
    return fs.ftruncateSync(path, len);
  }
  if (len === undefined) {
    len = 0;
  }
  // allow error to be thrown, but still close fd.
  var fd = fs.openSync(path, 'r+');
  var ret;

  try {
    ret = fs.ftruncateSync(fd, len);
  } finally {
    fs.closeSync(fd);
  }
  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.unlink"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>unlink ()](#apidoc.element.fs-promise.unlink)
- description and source-code
```javascript
unlink = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.unlinkSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>unlinkSync (path)](#apidoc.element.fs-promise.unlinkSync)
- description and source-code
```javascript
unlinkSync = function (path) {
  nullCheck(path);
  return binding.unlink(pathModule._makeLong(path));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.unwatchFile"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>unwatchFile (filename, listener)](#apidoc.element.fs-promise.unwatchFile)
- description and source-code
```javascript
unwatchFile = function (filename, listener) {
  nullCheck(filename);
  filename = pathModule.resolve(filename);
  var stat = statWatchers.get(filename);

  if (stat === undefined) return;

  if (typeof listener === 'function') {
    stat.removeListener('change', listener);
  } else {
    stat.removeAllListeners('change');
  }

  if (stat.listenerCount('change') === 0) {
    stat.stop();
    statWatchers.delete(filename);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.utimes"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>utimes ()](#apidoc.element.fs-promise.utimes)
- description and source-code
```javascript
utimes = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.utimesSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>utimesSync (path, atime, mtime)](#apidoc.element.fs-promise.utimesSync)
- description and source-code
```javascript
utimesSync = function (path, atime, mtime) {
  nullCheck(path);
  atime = toUnixTimestamp(atime);
  mtime = toUnixTimestamp(mtime);
  binding.utimes(pathModule._makeLong(path), atime, mtime);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.watch"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>watch (filename, options, listener)](#apidoc.element.fs-promise.watch)
- description and source-code
```javascript
watch = function (filename, options, listener) {
  nullCheck(filename);

  options = options || {};
  if (typeof options === 'function') {
    listener = options;
    options = {};
  } else if (typeof options === 'string') {
    options = {encoding: options};
  }
  if (typeof options !== 'object')
    throw new TypeError('"options" must be a string or an object');

  if (options.persistent === undefined) options.persistent = true;
  if (options.recursive === undefined) options.recursive = false;

  const watcher = new FSWatcher();
  watcher.start(filename,
                options.persistent,
                options.recursive,
                options.encoding);

  if (listener) {
    watcher.addListener('change', listener);
  }

  return watcher;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.watchFile"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>watchFile (filename, options, listener)](#apidoc.element.fs-promise.watchFile)
- description and source-code
```javascript
watchFile = function (filename, options, listener) {
  nullCheck(filename);
  filename = pathModule.resolve(filename);
  var stat;

  var defaults = {
    // Poll interval in milliseconds. 5007 is what libev used to use. It's
    // a little on the slow side but let's stick with it for now to keep
    // behavioral changes to a minimum.
    interval: 5007,
    persistent: true
  };

  if (options !== null && typeof options === 'object') {
    options = util._extend(defaults, options);
  } else {
    listener = options;
    options = defaults;
  }

  if (typeof listener !== 'function') {
    throw new Error('"watchFile()" requires a listener function');
  }

  stat = statWatchers.get(filename);

  if (stat === undefined) {
    stat = new StatWatcher();
    stat.start(filename, options.persistent, options.interval);
    statWatchers.set(filename, stat);
  }

  stat.addListener('change', listener);
  return stat;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.write"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>write ()](#apidoc.element.fs-promise.write)
- description and source-code
```javascript
write = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.writeFile"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>writeFile ()](#apidoc.element.fs-promise.writeFile)
- description and source-code
```javascript
function writeFile() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
...

[![Build Status](https://secure.travis-ci.org/kevinbeaty/fs-promise.svg)](http://travis-ci.org/kevinbeaty/fs-promise)


'''javascript
var fsp = require('fs-promise');

fsp.writeFile('/tmp/hello1.txt', 'hello world')
  .then(function(){
    return fsp.readFile('/tmp/hello1.txt', {encoding:'utf8'});
  })
  .then(function(contents){});
'''

## Implementation
...
```

#### <a name="apidoc.element.fs-promise.writeFileSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>writeFileSync (path, data, options)](#apidoc.element.fs-promise.writeFileSync)
- description and source-code
```javascript
writeFileSync = function (path, data, options) {
  if (!options) {
    options = { encoding: 'utf8', mode: 0o666, flag: 'w' };
  } else if (typeof options === 'string') {
    options = { encoding: options, mode: 0o666, flag: 'w' };
  } else if (typeof options !== 'object') {
    throwOptionsError(options);
  }

  assertEncoding(options.encoding);

  var flag = options.flag || 'w';
  var isUserFd = isFd(path); // file descriptor ownership
  var fd = isUserFd ? path : fs.openSync(path, flag, options.mode);

  if (!(data instanceof Buffer)) {
    data = Buffer.from('' + data, options.encoding || 'utf8');
  }
  var offset = 0;
  var length = data.length;
  var position = /a/.test(flag) ? null : 0;
  try {
    while (length > 0) {
      var written = fs.writeSync(fd, data, offset, length, position);
      offset += written;
      length -= written;
      if (position !== null) {
        position += written;
      }
    }
  } finally {
    if (!isUserFd) fs.closeSync(fd);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.writeJSON"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>writeJSON ()](#apidoc.element.fs-promise.writeJSON)
- description and source-code
```javascript
function writeFile() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.writeJSONSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>writeJSONSync (file, obj, options)](#apidoc.element.fs-promise.writeJSONSync)
- description and source-code
```javascript
function writeFileSync(file, obj, options) {
  options = options || {}
  var fs = options.fs || _fs

  var spaces = typeof options === 'object' && options !== null
    ? 'spaces' in options
    ? options.spaces : this.spaces
    : this.spaces

  var str = JSON.stringify(obj, options.replacer, spaces) + '\n'
  // not sure if fs.writeFileSync returns anything, but just in case
  return fs.writeFileSync(file, str, options)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.writeJson"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>writeJson ()](#apidoc.element.fs-promise.writeJson)
- description and source-code
```javascript
function writeFile() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.writeJsonSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>writeJsonSync (file, obj, options)](#apidoc.element.fs-promise.writeJsonSync)
- description and source-code
```javascript
function writeFileSync(file, obj, options) {
  options = options || {}
  var fs = options.fs || _fs

  var spaces = typeof options === 'object' && options !== null
    ? 'spaces' in options
    ? options.spaces : this.spaces
    : this.spaces

  var str = JSON.stringify(obj, options.replacer, spaces) + '\n'
  // not sure if fs.writeFileSync returns anything, but just in case
  return fs.writeFileSync(file, str, options)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.writeSync"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>writeSync (fd, buffer, offset, length, position)](#apidoc.element.fs-promise.writeSync)
- description and source-code
```javascript
writeSync = function (fd, buffer, offset, length, position) {
  if (buffer instanceof Buffer) {
    if (position === undefined)
      position = null;
    return binding.writeBuffer(fd, buffer, offset, length, position);
  }
  if (typeof buffer !== 'string')
    buffer += '';
  if (offset === undefined)
    offset = null;
  return binding.writeString(fd, buffer, offset, length, position);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fs-promise.ReadStream"></a>[module fs-promise.ReadStream](#apidoc.module.fs-promise.ReadStream)

#### <a name="apidoc.element.fs-promise.ReadStream.ReadStream"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>ReadStream (path, options)](#apidoc.element.fs-promise.ReadStream.ReadStream)
- description and source-code
```javascript
function ReadStream(path, options) {
  if (this instanceof ReadStream)
    return fs$ReadStream.apply(this, arguments), this
  else
    return ReadStream.apply(Object.create(ReadStream.prototype), arguments)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fs-promise.ReadStream.prototype"></a>[module fs-promise.ReadStream.prototype](#apidoc.module.fs-promise.ReadStream.prototype)

#### <a name="apidoc.element.fs-promise.ReadStream.prototype.open"></a>[function <span class="apidocSignatureSpan">fs-promise.ReadStream.prototype.</span>open ()](#apidoc.element.fs-promise.ReadStream.prototype.open)
- description and source-code
```javascript
function ReadStream$open() {
  var that = this
  open(that.path, that.flags, that.mode, function (err, fd) {
    if (err) {
      if (that.autoClose)
        that.destroy()

      that.emit('error', err)
    } else {
      that.fd = fd
      that.emit('open', fd)
      that.read()
    }
  })
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fs-promise.Stats"></a>[module fs-promise.Stats](#apidoc.module.fs-promise.Stats)

#### <a name="apidoc.element.fs-promise.Stats.Stats"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>Stats ( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec)](#apidoc.element.fs-promise.Stats.Stats)
- description and source-code
```javascript
function Stats( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec) {
  this.dev = dev;
  this.mode = mode;
  this.nlink = nlink;
  this.uid = uid;
  this.gid = gid;
  this.rdev = rdev;
  this.blksize = blksize;
  this.ino = ino;
  this.size = size;
  this.blocks = blocks;
  this.atime = new Date(atim_msec);
  this.mtime = new Date(mtim_msec);
  this.ctime = new Date(ctim_msec);
  this.birthtime = new Date(birthtim_msec);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fs-promise.Stats.prototype"></a>[module fs-promise.Stats.prototype](#apidoc.module.fs-promise.Stats.prototype)

#### <a name="apidoc.element.fs-promise.Stats.prototype._checkModeProperty"></a>[function <span class="apidocSignatureSpan">fs-promise.Stats.prototype.</span>_checkModeProperty (property)](#apidoc.element.fs-promise.Stats.prototype._checkModeProperty)
- description and source-code
```javascript
_checkModeProperty = function (property) {
  return ((this.mode & constants.S_IFMT) === property);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.Stats.prototype.isBlockDevice"></a>[function <span class="apidocSignatureSpan">fs-promise.Stats.prototype.</span>isBlockDevice ()](#apidoc.element.fs-promise.Stats.prototype.isBlockDevice)
- description and source-code
```javascript
isBlockDevice = function () {
  return this._checkModeProperty(constants.S_IFBLK);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.Stats.prototype.isCharacterDevice"></a>[function <span class="apidocSignatureSpan">fs-promise.Stats.prototype.</span>isCharacterDevice ()](#apidoc.element.fs-promise.Stats.prototype.isCharacterDevice)
- description and source-code
```javascript
isCharacterDevice = function () {
  return this._checkModeProperty(constants.S_IFCHR);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.Stats.prototype.isDirectory"></a>[function <span class="apidocSignatureSpan">fs-promise.Stats.prototype.</span>isDirectory ()](#apidoc.element.fs-promise.Stats.prototype.isDirectory)
- description and source-code
```javascript
isDirectory = function () {
  return this._checkModeProperty(constants.S_IFDIR);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.Stats.prototype.isFIFO"></a>[function <span class="apidocSignatureSpan">fs-promise.Stats.prototype.</span>isFIFO ()](#apidoc.element.fs-promise.Stats.prototype.isFIFO)
- description and source-code
```javascript
isFIFO = function () {
  return this._checkModeProperty(constants.S_IFIFO);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.Stats.prototype.isFile"></a>[function <span class="apidocSignatureSpan">fs-promise.Stats.prototype.</span>isFile ()](#apidoc.element.fs-promise.Stats.prototype.isFile)
- description and source-code
```javascript
isFile = function () {
  return this._checkModeProperty(constants.S_IFREG);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.Stats.prototype.isSocket"></a>[function <span class="apidocSignatureSpan">fs-promise.Stats.prototype.</span>isSocket ()](#apidoc.element.fs-promise.Stats.prototype.isSocket)
- description and source-code
```javascript
isSocket = function () {
  return this._checkModeProperty(constants.S_IFSOCK);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs-promise.Stats.prototype.isSymbolicLink"></a>[function <span class="apidocSignatureSpan">fs-promise.Stats.prototype.</span>isSymbolicLink ()](#apidoc.element.fs-promise.Stats.prototype.isSymbolicLink)
- description and source-code
```javascript
isSymbolicLink = function () {
  return this._checkModeProperty(constants.S_IFLNK);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fs-promise.WriteStream"></a>[module fs-promise.WriteStream](#apidoc.module.fs-promise.WriteStream)

#### <a name="apidoc.element.fs-promise.WriteStream.WriteStream"></a>[function <span class="apidocSignatureSpan">fs-promise.</span>WriteStream (path, options)](#apidoc.element.fs-promise.WriteStream.WriteStream)
- description and source-code
```javascript
function WriteStream(path, options) {
  if (this instanceof WriteStream)
    return fs$WriteStream.apply(this, arguments), this
  else
    return WriteStream.apply(Object.create(WriteStream.prototype), arguments)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fs-promise.WriteStream.prototype"></a>[module fs-promise.WriteStream.prototype](#apidoc.module.fs-promise.WriteStream.prototype)

#### <a name="apidoc.element.fs-promise.WriteStream.prototype.open"></a>[function <span class="apidocSignatureSpan">fs-promise.WriteStream.prototype.</span>open ()](#apidoc.element.fs-promise.WriteStream.prototype.open)
- description and source-code
```javascript
function WriteStream$open() {
  var that = this
  open(that.path, that.flags, that.mode, function (err, fd) {
    if (err) {
      that.destroy()
      that.emit('error', err)
    } else {
      that.fd = fd
      that.emit('open', fd)
    }
  })
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
