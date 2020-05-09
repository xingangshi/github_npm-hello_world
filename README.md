## github_npm-hello_world
> Just a simple demo for  nmp package by using github npm registry. [Github Packages](https://github.com/features/packages)

### Installation
> Before installing, make sure you has been authented with [Github Pakage](https://github.com/features/packages) or using a `.npmrc` file.
>
> You can see [Configuring npm for use with GitHub Packages](https://help.github.com/en/packages/using-github-packages-with-your-projects-ecosystem/configuring-npm-for-use-with-github-packages#authenticating-to-github-package-registry).

#### Install
1.
```shell
npm install @xingangshi/github_npm-hello_world
```

IF you get the following errors, please use the mehod-3 to install the package.

1.1 Maybe error 1:

```shell
$ npm install @xingangshi/github_npm-hello_world@1.0.2
npm ERR! code E404
npm ERR! 404 Not Found - GET https://registry.npmjs.org/@xingangshi%2fgithub_npm-hello_world - Not found
npm ERR! 404
npm ERR! 404  '@xingangshi/github_npm-hello_world@1.0.4' is not in the npm registry.
npm ERR! 404 You should bug the author to publish it (or use the name yourself!)
npm ERR! 404
npm ERR! 404 Note that you can also install from a
npm ERR! 404 tarball, folder, http url, or git url.

npm ERR! A complete log of this run can be found in:
npm ERR!     C:\Users\S1635\AppData\Roaming\npm-cache\_logs\2020-05-09T06_08_20_754Z-debug.log
```
1.2 Maybe error 2:
```
[panshi@localhost panshi]$ npm install @xingangshi/github_npm-hello_world
npm ERR! Linux 2.6.32-642.3.1.el6.x86_64
npm ERR! argv "/usr/bin/node" "/usr/bin/npm" "install" "@xingangshi/github_npm-hello_world"
npm ERR! node v6.3.0
npm ERR! npm  v3.10.3
npm ERR! code E404

npm ERR! 404 Not found : github
npm ERR! 404
npm ERR! 404  'github' is not in the npm registry.
npm ERR! 404 You should bug the author to publish it (or use the name yourself!)
npm ERR! 404
npm ERR! 404 Note that you can also install from a
npm ERR! 404 tarball, folder, http url, or git url.

npm ERR! Please include the following file with any support request:
npm ERR!     /home/panshi/npm-debug.log
```

2.
```js
"dependencies": {
    "@xingangshi/github_npm-hello_world": "1.0.2"
  }
```
3.

```shell
npm i https://github.com/xingangshi/github_npm-hello_world
npm install
```

### Usage
1. Terminal
```shell
$ node
> const hello_world_pkg = require("@xingangshi/github_npm-hello_world");
undefined
> hello_world_pkg.hello_world();
Hello world from Github npm package
undefined
>
```

2. Js code

Just like file of [`test_pakage.js`](https://github.com/xingangshi/github_npm-hello_world/blob/master/test_pakage.js):

```js
const hello_world_pkg = require("@xingangshi/github_npm-hello_world");
hello_world_pkg.hello_world();
```
