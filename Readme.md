# promise-map

[![npm version](https://img.shields.io/npm/v/promise-utils.svg?style=flat-square)](https://www.npmjs.org/package/promise-utils)
![build status](https://img.shields.io/github/workflow/status/shfshanyue/promise-map/test?style=flat-square)
[![install size](https://packagephobia.now.sh/badge?p=promise-utils)](https://packagephobia.now.sh/result?p=promise-utils)
[![npm downloads](https://img.shields.io/npm/dw/promise-utils.svg?style=flat-square)](http://npm-stat.com/charts.html?package=promise-utils)

## Install

``` bash
$ npm install promise-utils
```

## Usage

``` ts
import { map, filter, retry, sleep } from 'promise-utils'


await filter([Promise.resolve(1), 2, 3, 4], (x: number) => Boolean(x % 2))

await map([Promise.resolve(1), 2, 3, 4], (x: number) => x + 1)

await sleep(300)

await retry(() => Promise.resolve(3), { times: 3 })
```

## API

### filter(input, filterer, [options])

### map(input, mapper, [options])

### retry(input, [options])

### sleep(ms)
