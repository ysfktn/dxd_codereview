```sh
review@crdao:~/casperholdersfront (main)$ sudo docker build --build-arg mode=mainnet .

Sending build context to Docker daemon  23.46MB

Step 1/11 : FROM node:lts as build-stage
 ---> 5f9d246cdc07
Step 2/11 : ARG mode
 ---> Using cache
 ---> eb993b445cc2
Step 3/11 : WORKDIR /app
 ---> Using cache
 ---> 254710633e15
Step 4/11 : COPY package*.json ./
 ---> Using cache
 ---> e5a09ffa6dd0
Step 5/11 : RUN yarn install
 ---> Running in 46703ef6edf5
yarn install v1.22.18
info No lockfile found.
[1/4] Resolving packages...
[91mwarning @cypress/code-coverage > nyc > istanbul-lib-processinfo > uuid@3.4.0: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
[0m[91mwarning @vue/cli-plugin-babel > webpack > watchpack > watchpack-chokidar2 > chokidar@2.1.8: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
[0m[91mwarning @vue/cli-plugin-babel > webpack > micromatch > snapdragon > source-map-resolve@0.5.3: See https://github.com/lydell/source-map-resolve#deprecated
[0m[91mwarning @vue/cli-plugin-babel > webpack > watchpack > watchpack-chokidar2 > chokidar > fsevents@1.2.13: fsevents 1 will break on node v14+ and could be using insecure binaries. Upgrade to fsevents 2.
[0m[91mwarning @vue/cli-plugin-babel > webpack > micromatch > snapdragon > source-map-resolve > resolve-url@0.2.1: https://github.com/lydell/resolve-url#deprecated
[0m[91mwarning @vue/cli-plugin-babel > webpack > micromatch > snapdragon > source-map-resolve > urix@0.1.0: Please see https://github.com/lydell/urix#deprecated
[0m[91mwarning @vue/cli-plugin-babel > webpack > micromatch > snapdragon > source-map-resolve > source-map-url@0.4.1: See https://github.com/lydell/source-map-url#deprecated
[0m[91mwarning @vue/cli-plugin-babel > @vue/cli-shared-utils > request@2.88.2: request has been deprecated, see https://github.com/request/request/issues/3142
[0m[91mwarning @vue/cli-plugin-babel > @vue/cli-shared-utils > request > uuid@3.4.0: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
[0m[91mwarning @vue/cli-plugin-babel > @vue/cli-shared-utils > @hapi/joi@15.1.1: Switch to 'npm install joi'
[0m[91mwarning @vue/cli-plugin-babel > webpack > node-libs-browser > url > querystring@0.2.0: The querystring API is considered Legacy. new code should use the URLSearchParams API instead.
[0m[91mwarning @vue/cli-plugin-babel > @vue/cli-shared-utils > request > har-validator@5.1.5: this library is no longer supported
[0m[91mwarning @vue/cli-plugin-babel > @vue/cli-shared-utils > @hapi/joi > @hapi/hoek@8.5.1: This version has been deprecated and is no longer supported or maintained
[0m[91mwarning @vue/cli-plugin-babel > @vue/cli-shared-utils > @hapi/joi > @hapi/topo@3.1.6: This version has been deprecated and is no longer supported or maintained
[0m[91mwarning @vue/cli-plugin-babel > @vue/cli-shared-utils > @hapi/joi > @hapi/topo > @hapi/hoek@8.5.1: This version has been deprecated and is no longer supported or maintained
[0m[91mwarning @vue/cli-plugin-babel > @vue/cli-shared-utils > @hapi/joi > @hapi/bourne@1.3.2: This version has been deprecated and is no longer supported or maintained
[0m[91mwarning @vue/cli-plugin-babel > @vue/cli-shared-utils > @hapi/joi > @hapi/address@2.1.4: Moved to 'npm install @sideway/address'
[0m[91mwarning @vue/cli-plugin-e2e-cypress > cypress > debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
[0m[91mwarning @vue/cli-plugin-e2e-cypress > cypress > request@2.88.0: request has been deprecated, see https://github.com/request/request/issues/3142
[0m[91mwarning @vue/cli-plugin-e2e-cypress > cypress > request > har-validator@5.1.5: this library is no longer supported
[0m[91mwarning @vue/cli-plugin-e2e-cypress > cypress > request > uuid@3.4.0: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
[0m[91mwarning @vue/cli-plugin-e2e-cypress > cypress > extract-zip > mkdirp@0.5.1: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
[0m[91mwarning @vue/cli-plugin-eslint > eslint-loader@2.2.1: This loader has been deprecated. Please use eslint-webpack-plugin
[0m[91mwarning @vue/cli-plugin-pwa > workbox-webpack-plugin > workbox-build > @hapi/joi@15.1.1: Switch to 'npm install joi'
[0m[91mwarning @vue/cli-plugin-pwa > workbox-webpack-plugin > workbox-build > strip-comments > babel-plugin-transform-object-rest-spread > babel-runtime > core-js@2.6.12: core-js@<3.4 is no longer maintained and not recommended for usage due to the number of issues. Because of the V8 engine whims, feature detection in old core-js versions could cause a slowdown up to 100x even if nothing is polyfilled. Please, upgrade your dependencies to the actual version of core-js.
[0m[91mwarning @vue/cli-service > html-webpack-plugin@3.2.0: 3.x is no longer supported
[0m[91mwarning @vue/cli-service > webpack-dev-server > chokidar@2.1.8: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
[0m[91mwarning @vue/cli-service > copy-webpack-plugin > webpack-log > uuid@3.4.0: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
[0m[91mwarning @vue/cli-service > @intervolga/optimize-cssnano-plugin > cssnano-preset-default > postcss-svgo > svgo@1.3.2: This SVGO version is no longer supported. Upgrade to v2.x.x.
[0m[91mwarning babel-eslint@10.1.0: babel-eslint is now @babel/eslint-parser. This package will no longer receive updates.
[0m[2/4] Fetching packages...
[3/4] Linking dependencies...
[91mwarning "@casperholders/core > casper-js-sdk > eslint-plugin-prettier@3.4.1" has unmet peer dependency "prettier@>=1.13.0".
[0m[91mwarning " > @toruslabs/casper-embed@1.2.0" has unmet peer dependency "@babel/runtime@7.x".
warning "@toruslabs/casper-embed > @toruslabs/base-controllers@1.6.18" has unmet peer dependency "@babel/runtime@7.x".
[0m[91mwarning "@toruslabs/casper-embed > @toruslabs/openlogin-jrpc@1.7.3" has unmet peer dependency "@babel/runtime@7.x".
[0m[91mwarning "@toruslabs/casper-embed > @toruslabs/http-helpers@2.2.0" has unmet peer dependency "@babel/runtime@7.x".
[0m[91mwarning "@toruslabs/casper-embed > @toruslabs/openlogin-jrpc > @toruslabs/openlogin-utils@1.7.0" has unmet peer dependency "@babel/runtime@7.x".
[0m[91mwarning "@cypress/code-coverage > @cypress/webpack-preprocessor@5.11.1" has unmet peer dependency "@babel/core@^7.0.1".
warning "@cypress/code-coverage > @cypress/webpack-preprocessor@5.11.1" has unmet peer dependency "@babel/preset-env@^7.0.0".
[0m[91mwarning "@cypress/code-coverage > @cypress/webpack-preprocessor@5.11.1" has unmet peer dependency "babel-loader@^8.0.2".
[0m[91mwarning "@cypress/code-coverage > @cypress/webpack-preprocessor@5.11.1" has unmet peer dependency "webpack@^4 || ^5".
[0m[91mwarning " > @vue/eslint-config-airbnb@5.3.0" has unmet peer dependency "eslint-plugin-import@^2.18.2".
[0m[91mwarning "@vue/eslint-config-airbnb > eslint-import-resolver-webpack@0.13.2" has unmet peer dependency "webpack@>=1.11.0".
[0m[91mwarning " > sass-loader@10.2.1" has unmet peer dependency "webpack@^4.36.0 || ^5.0.0".
warning " > vue-cli-plugin-vuetify@2.5.0" has unmet peer dependency "webpack@^4.0.0 || ^5.0.0".
warning "vue-cli-plugin-vuetify > null-loader@4.0.1" has unmet peer dependency "webpack@^4.0.0 || ^5.0.0".
[0m[91mwarning " > vuetify-loader@1.7.3" has unmet peer dependency "webpack@^4.0.0 || ^5.0.0".
[0m[91mwarning "vuetify-loader > file-loader@6.2.0" has unmet peer dependency "webpack@^4.0.0 || ^5.0.0".
[0m[4/4] Building fresh packages...
success Saved lockfile.
Done in 428.38s.
Removing intermediate container 46703ef6edf5
 ---> 5bfef526b62d
Step 6/11 : COPY ./ .
 ---> def3ec8b54ef
Step 7/11 : RUN yarn build-${mode}
 ---> Running in 25af0aadacf5
yarn run v1.22.18
$ vue-cli-service build --mode mainnet

[91m-  Building for mainnet...
[0m WARNING  Compiled with 20 warnings4:20:50 AM

Module Warning (from ./node_modules/eslint-loader/index.js):

/app/src/components/layout/Connect.vue
  569:9  warning  Unexpected console statement  no-console
  611:9  warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


Module Warning (from ./node_modules/eslint-loader/index.js):

/app/src/components/operations/OperationResult.vue
  329:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/app/src/components/operations/Validators.vue
  241:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/app/src/views/account/AccountInfo.vue
  239:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/app/src/views/account/Balance.vue
  292:11  warning  Unexpected console statement  no-console
  313:9   warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


Module Warning (from ./node_modules/eslint-loader/index.js):

/app/src/views/account/Security.vue
  617:11  warning  Unexpected console statement  no-console
  691:9   warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


Module Warning (from ./node_modules/eslint-loader/index.js):

/app/src/views/account/Transfer.vue
  275:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/app/src/views/developers/SmartContract.vue
  189:9  warning  Unexpected console statement  no-console
  245:9  warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


Module Warning (from ./node_modules/eslint-loader/index.js):

/app/src/views/multisig/MultiSig.vue
  458:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/app/src/views/staking/Delegate.vue
  233:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/app/src/views/staking/Undelegate.vue
  198:9  warning  Unexpected console statement  no-console
  230:9  warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


Module Warning (from ./node_modules/eslint-loader/index.js):

/app/src/views/validators/AddBid.vue
  261:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/app/src/views/validators/WithdrawBid.vue
  253:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


You may use special comments to disable some warnings.
Use // eslint-disable-next-line to ignore the next line.
Use /* eslint-disable */ to ignore all warnings in a file.
 warning  in ./src/helpers/genericSendDeploy.js

Module Warning (from ./node_modules/thread-loader/dist/cjs.js):

/app/src/helpers/genericSendDeploy.js
  63:9  warning  Unexpected console statement  no-console
  82:5  warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


 @ ./node_modules/cache-loader/dist/cjs.js??ref--13-0!./node_modules/thread-loader/dist/cjs.js!./node_modules/babel-loader/lib!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options!./src/views/account/AccountInfo.vue?vue&type=script&lang=js& 1197:0-60 1448:23-40
 @ ./src/views/account/AccountInfo.vue?vue&type=script&lang=js&
 @ ./src/views/account/AccountInfo.vue
 @ ./src/router/index.js
 @ ./src/main.js
 @ multi ./src/main.js

 warning  in ./src/store/index.js

Module Warning (from ./node_modules/thread-loader/dist/cjs.js):

/app/src/store/index.js
  275:7  warning  Unexpected console statement  no-console
  360:9  warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


 @ ./src/main.js 104:0-28 113:9-14
 @ multi ./src/main.js

 warning  

chunk account-view~addbid-view~balance-view~settings-view~smartcontract-view~stake-view~transfer-view~unst~52c4e50f [mini-css-extract-plugin]
Conflicting order. Following module has been added:
 * css ./node_modules/css-loader/dist/cjs.js??ref--10-oneOf-3-1!./node_modules/postcss-loader/src??ref--10-oneOf-3-2!./node_modules/sass-loader/dist/cjs.js??ref--10-oneOf-3-3!./node_modules/vuetify/src/components/VInput/VInput.sass
despite it was not able to fulfill desired ordering with these modules:
 * css ./node_modules/css-loader/dist/cjs.js??ref--10-oneOf-3-1!./node_modules/postcss-loader/src??ref--10-oneOf-3-2!./node_modules/sass-loader/dist/cjs.js??ref--10-oneOf-3-3!./node_modules/vuetify/src/components/VTextField/VTextField.sass
   - couldn't fulfill desired order of chunk group(s) balance-view, transfer-view, account-view, stake-view, unstake-view, addbid-view, withdrawbid-view, smartcontract-view
   - while fulfilling desired order of chunk group(s) settings-view

 warning  

chunk account-view~addbid-view~balance-view~settings-view~smartcontract-view~stake-view~transfer-view~unst~52c4e50f [mini-css-extract-plugin]
Conflicting order. Following module has been added:
 * css ./node_modules/css-loader/dist/cjs.js??ref--10-oneOf-3-1!./node_modules/postcss-loader/src??ref--10-oneOf-3-2!./node_modules/sass-loader/dist/cjs.js??ref--10-oneOf-3-3!./node_modules/vuetify/src/components/VLabel/VLabel.sass
despite it was not able to fulfill desired ordering with these modules:
 * css ./node_modules/css-loader/dist/cjs.js??ref--10-oneOf-3-1!./node_modules/postcss-loader/src??ref--10-oneOf-3-2!./node_modules/sass-loader/dist/cjs.js??ref--10-oneOf-3-3!./node_modules/vuetify/src/components/VTextField/VTextField.sass
   - couldn't fulfill desired order of chunk group(s) balance-view, transfer-view, account-view, stake-view, unstake-view, addbid-view, withdrawbid-view, smartcontract-view
   - while fulfilling desired order of chunk group(s) settings-view

 warning  

chunk account-view~addbid-view~balance-view~settings-view~smartcontract-view~stake-view~transfer-view~unst~52c4e50f [mini-css-extract-plugin]
Conflicting order. Following module has been added:
 * css ./node_modules/css-loader/dist/cjs.js??ref--10-oneOf-3-1!./node_modules/postcss-loader/src??ref--10-oneOf-3-2!./node_modules/sass-loader/dist/cjs.js??ref--10-oneOf-3-3!./node_modules/vuetify/src/components/VMessages/VMessages.sass
despite it was not able to fulfill desired ordering with these modules:
 * css ./node_modules/css-loader/dist/cjs.js??ref--10-oneOf-3-1!./node_modules/postcss-loader/src??ref--10-oneOf-3-2!./node_modules/sass-loader/dist/cjs.js??ref--10-oneOf-3-3!./node_modules/vuetify/src/components/VTextField/VTextField.sass
   - couldn't fulfill desired order of chunk group(s) balance-view, transfer-view, account-view, stake-view, unstake-view, addbid-view, withdrawbid-view, smartcontract-view
   - while fulfilling desired order of chunk group(s) settings-view

 warning  

asset size limit: The following asset(s) exceed the recommended size limit (244 KiB).
This can impact web performance.
Assets: 
  js/balance-view.57b4233d.js (561 KiB)
  css/chunk-vendors.56303a1f.css (366 KiB)
  js/chunk-vendors.399cf0c2.js (2.34 MiB)

 warning  

entrypoint size limit: The following entrypoint(s) combined asset size exceeds the recommended limit (244 KiB). This can impact web performance.
Entrypoints:
  app (2.88 MiB)
      css/chunk-vendors.56303a1f.css
      js/chunk-vendors.399cf0c2.js
      css/app.6b1608e7.css
      js/app.937536cc.js


  File                                      Size             Gzipped

  dist/js/chunk-vendors.399cf0c2.js         2391.05 KiB      720.99 KiB
  dist/js/balance-view.57b4233d.js          560.55 KiB       145.49 KiB
  dist/js/balance-view~home-view~stake-v    202.68 KiB       67.12 KiB
  iew.05533b5b.js
  dist/js/app.937536cc.js                   187.11 KiB       39.30 KiB
  dist/js/stake-view.a2cbc54f.js            114.28 KiB       26.72 KiB
  dist/js/account-view~addbid-view~balan    100.37 KiB       21.71 KiB
  ce-view~smartcontract-view~stake-view~
  transfer-view~unstake-view~withd~486a3
  9ec.dafa1101.js
  dist/js/home-view.da14fe7a.js             75.38 KiB        18.04 KiB
  dist/js/contact-view.aad1d872.js          69.79 KiB        10.67 KiB
  dist/js/unstake-view.c89c278a.js          56.47 KiB        12.34 KiB
  dist/js/addbid-view.24ba1ed5.js           32.10 KiB        8.90 KiB
  dist/js/settings-view.f9b07048.js         28.85 KiB        7.15 KiB
  dist/js/balance-view~unstake-view.c5fc    26.68 KiB        7.54 KiB
  e867.js
  dist/js/transfer-view.408f2ecc.js         26.10 KiB        6.74 KiB
  dist/js/account-view~addbid-view~balan    24.79 KiB        6.94 KiB
  ce-view~settings-view~smartcontract-vi
  ew~stake-view~transfer-view~unst~52c4e
  50f.cee28df7.js
  dist/js/smartcontract-view.48beeaec.js    24.26 KiB        6.86 KiB
  dist/js/account-view.cc2d6d2e.js          21.22 KiB        5.78 KiB
  dist/js/withdrawbid-view.1121b9fb.js      20.53 KiB        5.41 KiB
  dist/js/addbid-view~smartcontract-view    18.66 KiB        4.24 KiB
  ~stake-view~transfer-view~unstake-view
  ~withdrawbid-view.c670b9c4.js
  dist/js/faq-view.c5101591.js              6.51 KiB         1.98 KiB
  dist/precache-manifest.7b31571e96bbb62    4.56 KiB         1.26 KiB
  9b1985f60a975aac4.js
  dist/service-worker.js                    1.02 KiB         0.47 KiB
  dist/css/chunk-vendors.56303a1f.css       365.79 KiB       44.19 KiB
  dist/css/account-view~addbid-view~bala    22.82 KiB        3.11 KiB
  nce-view~settings-view~smartcontract-v
  iew~stake-view~transfer-view~unst~52c4
  e50f.ed7a7d4f.css
  dist/css/balance-view.ab7462e1.css        11.53 KiB        1.85 KiB
  dist/css/account-view~addbid-view~bala    9.49 KiB         1.95 KiB
  nce-view~smartcontract-view~stake-view
  ~transfer-view~unstake-view~withd~486a
  39ec.1311a611.css
  dist/css/addbid-view.2d728a8a.css         6.27 KiB         1.22 KiB
  dist/css/stake-view.14e63fa2.css          5.52 KiB         1.25 KiB
  dist/css/balance-view~unstake-view.8bf    5.27 KiB         1.15 KiB
  3f273.css
  dist/css/settings-view.cf6fe5fe.css       3.83 KiB         0.96 KiB
  dist/css/home-view.dc456265.css           3.21 KiB         0.75 KiB
  dist/css/app.6b1608e7.css                 1.41 KiB         0.66 KiB
  dist/css/smartcontract-view.76a811a3.c    1.36 KiB         0.38 KiB
  ss
  dist/css/unstake-view.f20af4b7.css        0.06 KiB         0.08 KiB

  Images and other types of assets omitted.

 DONE  Build complete. The dist directory is ready to be deployed.
 INFO  Check out deployment instructions at https://cli.vuejs.org/guide/deployment.html
      
Done in 133.16s.
Removing intermediate container 25af0aadacf5
 ---> 32f35a1f9805
Step 8/11 : FROM nginx as production-stage
 ---> de2543b9436b
Step 9/11 : RUN mkdir /app
 ---> Using cache
 ---> df80ed06ffcb
Step 10/11 : COPY --from=build-stage /app/dist /app
 ---> 10b3c22ffb62
Step 11/11 : COPY nginx.conf /etc/nginx/nginx.conf
 ---> f907c09846c8
Successfully built f907c09846c8
```