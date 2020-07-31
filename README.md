# @egoist/promise-quene

[![NPM version](https://badgen.net/npm/v/@egoist/promise-quene)](https://npmjs.com/package/@egoist/promise-quene) [![NPM downloads](https://badgen.net/npm/dm/@egoist/promise-quene)](https://npmjs.com/package/@egoist/promise-quene) [![CircleCI](https://badgen.net/circleci/github/egoist/promise-quene/master)](https://circleci.com/gh/egoist/promise-quene/tree/master) [![donate](https://badgen.net/badge/support%20me/donate/ff69b4)](https://github.com/sponsors/egoist)

## Install

```bash
yarn add @egoist/promise-quene
```

## Usage

```js
const { PromiseQueue } = require('@egoist/promise-quene')

const processor = async (jobId, resolution, format) => {
  // run job
}

const queue = new PromiseQueue(processor)

// Add a job
// First argument is an unique job id
queue.add('process-video-id-xxxx', '720p', 'mp4')

// Run added jobs
// Resolves a Set of processed job ids
await queue.run()
```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## Author

**@egoist/promise-quene** © [EGOIST](https://github.com/egoist), Released under the [MIT](./LICENSE) License.<br>
Authored and maintained by EGOIST with help from contributors ([list](https://github.com/egoist/@egoist/promise-quene/contributors)).

> [github.com/egoist](https://github.com/egoist) · GitHub [@EGOIST](https://github.com/egoist) · Twitter [@\_egoistlily](https://twitter.com/_egoistlily)