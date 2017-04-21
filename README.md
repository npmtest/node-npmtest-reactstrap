# npmtest-reactstrap

#### basic test coverage for  [reactstrap (v4.5.0)](https://github.com/reactstrap/reactstrap#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-reactstrap.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-reactstrap) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-reactstrap.svg)](https://travis-ci.org/npmtest/node-npmtest-reactstrap)

#### React Bootstrap 4 components

[![NPM](https://nodei.co/npm/reactstrap.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/reactstrap)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-reactstrap/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-reactstrap/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-reactstrap/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-reactstrap/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-reactstrap/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-reactstrap/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-reactstrap/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-reactstrap/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-reactstrap/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-reactstrap/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-reactstrap/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-reactstrap/build/test-report.html](https://npmtest.github.io/node-npmtest-reactstrap/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-reactstrap/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-reactstrap/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-reactstrap/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-reactstrap/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-reactstrap/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-reactstrap/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-reactstrap/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-reactstrap/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "reactstrap",
    "version": "4.5.0",
    "description": "React Bootstrap 4 components",
    "main": "dist/reactstrap.min.js",
    "jsnext:main": "dist/reactstrap.es.js",
    "module": "dist/reactstrap.es.js",
    "scripts": {
        "report-coverage": "coveralls < ./coverage/lcov.info",
        "test": "BABEL_ENV=test react-scripts test --env=jsdom",
        "cover": "npm test -- --coverage",
        "start": "BABEL_ENV=webpack webpack-dev-server --config ./webpack.dev.config.js --watch",
        "build-docs": "cross-env WEBPACK_BUILD=production webpack --config ./webpack.dev.config.js --progress --colors",
        "build": "cross-env NODE_ENV=production rollup -c",
        "prebuild": "BABEL_ENV=dist-dir babel src --out-dir lib --ignore src/__tests__/",
        "create-release": "npm test && sh ./scripts/release",
        "publish-release": "npm test && sh ./scripts/publish",
        "lint": "eslint src"
    },
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/reactstrap/reactstrap.git"
    },
    "files": [
        "LICENSE",
        "README.md",
        "CHANGELOG.md",
        "lib",
        "dist"
    ],
    "keywords": [
        "reactstrap",
        "bootstrap",
        "react",
        "component",
        "components",
        "react-component",
        "ui"
    ],
    "contributors": [
        "Eddy Hernandez <edward.d.hernandez@gmail.com> (https://github.com/eddywashere)",
        "Evan Sharp <evan@lostonia.com> (https://github.com/TheSharpieOne)",
        "Chris Burrell <chrisburrell@gmail.com> (https://github.com/cbfx)",
        "Li Jinyao (https://github.com/LiJinyao)",
        "Matthew King (https://github.com/mking-clari)",
        "Ajai <ajainarayanan@gmail.com> (https://github.com/ajainarayanan)",
        "Paulus Schoutsen <paulus@paulusschoutsen.nl> (https://github.com/balloob)",
        "Ronny Haase (https://github.com/ronnyhaase)",
        "Ali Sheehan-Dare <alisd23@live.co.uk> (https://github.com/alisd23)",
        "Amila Welihinda (https://github.com/amilajack)",
        "David Edmondson (https://github.com/threehams)",
        "Aaron Panchal (https://github.com/aaronpanch)",
        "André Pena <andrerpena@gmail.com> (https://github.com/andrerpena)",
        "Ben Herila (https://github.com/bherila)",
        "Binoy <me@binoy.io> (https://github.com/binoy14)",
        "Chad Wintzer (https://github.com/arbitrarytech)",
        "Code Review Videos (https://github.com/codereviewvideos)",
        "Cory Deppen (https://github.com/corydeppen)",
        "Daniel Huisman <daniel@huisman.me> (https://github.com/DanielHuisman)",
        "Gary Thomas (https://github.com/gthomas-appfolio)",
        "Hosmel Quintana <hosmelq@gmail.com> (https://github.com/hosmelq)",
        "Jamie Albinson <jcalbinson@gmail.com> (https://github.com/jalbinson)",
        "Jason Sturges <jason@jasonsturges.com> (https://github.com/jasonsturges)",
        "Jean-Elie Barjonet (https://github.com/jebarjonet)",
        "Jeff Francisco (https://github.com/j-francisco)",
        "Jim Liu <junminliu@gmail.com> (https://github.com/JimLiu)",
        "Joe (https://github.com/joemcadams)",
        "Joe Woynillowicz (https://github.com/CoderJoeIO)",
        "Jon Jaques <jaquers@gmail.com> (https://github.com/jonjaques)",
        "Luc Vauvillier (https://github.com/lvauvillier)",
        "Melissa Siu <melissa.siu@gmail.com> (https://github.com/mesiu)",
        "Natthakit Susanthitanon (https://github.com/nsmag)",
        "Rich Hong <hong.rich@gmail.com> (https://github.com/hongrich)",
        "Skoranga (https://github.com/skoranga)",
        "Thijs Vogels (https://github.com/tvogels)",
        "Tyler Johnson <tyler@tylerjohnson.me> (https://github.com/tyler-johnson)",
        "alan blount <alan@zeroasterisk.com> (https://github.com/zeroasterisk)",
        "edgji (https://github.com/edgji)",
        "nlrowe (https://github.com/nlrowe)",
        "npm-to-cdn-bot (by Forbes Lindesay) (https://github.com/npmcdn-to-unpkg-bot)",
        "polmauri (https://github.com/polmauri)"
    ],
    "license": "MIT",
    "bugs": {
        "url": "https://github.com/reactstrap/reactstrap/issues"
    },
    "homepage": "https://github.com/reactstrap/reactstrap#readme",
    "dependencies": {
        "classnames": "^2.2.3",
        "lodash.isfunction": "^3.0.8",
        "lodash.isobject": "^3.0.2",
        "lodash.omit": "^4.4.1",
        "lodash.tonumber": "^4.0.3",
        "reactstrap-tether": "1.3.4"
    },
    "peerDependencies": {
        "react": "^0.14.0 || ^15.0.0",
        "react-addons-css-transition-group": "^0.14.0 || ^15.0.0",
        "react-addons-transition-group": "^0.14.0 || ^15.0.0",
        "react-dom": "^0.14.0 || ^15.0.0"
    },
    "devDependencies": {
        "babel-cli": "^6.14.0",
        "babel-loader": "^6.2.2",
        "babel-plugin-transform-object-rest-spread": "^6.23.0",
        "babel-preset-es2015-rollup": "^3.0.0",
        "babel-preset-react": "^6.11.1",
        "babel-preset-react-app": "^0.2.1",
        "bootstrap": "^4.0.0-alpha.6",
        "clean-webpack-plugin": "^0.1.8",
        "conventional-changelog-cli": "^1.1.1",
        "conventional-recommended-bump": "^0.3.0",
        "copy-webpack-plugin": "^3.0.1",
        "coveralls": "^2.11.12",
        "cross-env": "^2.0.0",
        "css-loader": "^0.25.0",
        "ejs": "^2.5.1",
        "enzyme": "^2.4.1",
        "eslint": "^3.2.2",
        "eslint-config-airbnb": "^10.0.0",
        "eslint-plugin-import": "^1.12.0",
        "eslint-plugin-jsx-a11y": "^2.0.1",
        "eslint-plugin-react": "^6.0.0",
        "eslint-plugin-standard": "^2.0.0",
        "extract-text-webpack-plugin": "^1.0.1",
        "history": "^3.0.0",
        "holderjs": "^2.9.3",
        "json-loader": "^0.5.4",
        "raw-loader": "^0.5.1",
        "react": "^15.3.0",
        "react-addons-css-transition-group": "^15.3.2",
        "react-addons-test-utils": "^15.3.0",
        "react-addons-transition-group": "^15.3.0",
        "react-dom": "^15.3.0",
        "react-helmet": "^3.0.1",
        "react-prism": "4.0.0",
        "react-router": "^2.6.1",
        "react-scripts": "^0.7.0",
        "rollup": "^0.41.5",
        "rollup-plugin-babel": "^2.7.1",
        "rollup-plugin-babili": "^2.0.0",
        "rollup-plugin-commonjs": "^8.0.2",
        "rollup-plugin-node-resolve": "^2.0.0",
        "static-site-generator-webpack-plugin": "^2.0.1",
        "style-loader": "^0.13.1",
        "webpack": "^1.12.13",
        "webpack-dev-server": "^1.14.1"
    },
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
