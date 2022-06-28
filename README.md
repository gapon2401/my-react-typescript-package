# my-react-typescript-package

[![NPM version][npm-image]][npm-url]
[![Build][github-build]][github-build-url]
![npm-typescript]
[![License][github-license]][github-license-url]

This repo is the example of the article ["How to create and publish React Typescript npm package with demo and automated build"](https://medium.com/@igaponov/how-to-create-and-publish-react-typescript-npm-package-with-demo-and-automated-build-80c40ec28aca).

You can clone it and step by step create your own NPM package and publish it.

It is simple React counter.

[**Live Demo**](https://gapon2401.github.io/my-react-typescript-package/)

## Installation:

```bash
npm install my-react-typescript-package --save-dev
```

or

```bash
yarn add -D my-react-typescript-package
```

## Usage :

Add `MyCounter` to your component:

```js
import React from 'react'
import ReactDOM from 'react-dom/client'
import { MyCounter } from 'my-react-typescript-package'

const root = ReactDOM.createRoot(document.getElementById('root') as HTMLElement)
root.render(
    <React.StrictMode>
        <div>
            <h2>Default counter</h2>
            <MyCounter />
        </div>
        <hr />
        <div>
            <h2>Counter with predefined value</h2>
            <MyCounter value={5} />
        </div>
    </React.StrictMode>,
)

```

[npm-url]: https://www.npmjs.com/package/my-react-typescript-package
[npm-image]: https://img.shields.io/npm/v/my-react-typescript-package
[github-license]: https://img.shields.io/github/license/gapon2401/my-react-typescript-package
[github-license-url]: https://github.com/gapon2401/my-react-typescript-package/blob/master/LICENSE
[github-build]: https://github.com/gapon2401/my-react-typescript-package/actions/workflows/publish.yml/badge.svg
[github-build-url]: https://github.com/gapon2401/my-react-typescript-package/actions/workflows/publish.yml
[npm-typescript]: https://img.shields.io/npm/types/my-react-typescript-package