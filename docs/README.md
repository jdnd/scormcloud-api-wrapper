# scormcloud-api-wrapper

[![npm](https://img.shields.io/npm/v/office-document-properties.svg?style=flat)](https://www.npmjs.com/package/scormcloud-api-wrapper)
[![MIT license](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://github.com/swestmoreland/scormcloud-api-wrapper/blob/master/LICENSE)
[![GitHub](https://img.shields.io/github/stars/swestmoreland/scormcloud-api-wrapper.svg?style=social&logo=github&label=Stars)](https://github.com/swestmoreland/scormcloud-api-wrapper/)
[![Twitter](https://img.shields.io/twitter/follow/swestmoreland.svg?style=social&logo=twitter&label=Follow)](https://twitter.com/intent/follow?screen_name=swestmoreland)

Node.js client for the [SCORM Cloud API](https://cloud.scorm.com/docs/index.html).

## Installation {#installation}

To install via npm:

```sh
npm install scormcloud-api-wrapper --save
```

## Usage {#usage}

```js
// Import the module.
var SCORMCloud = require('scormcloud-api-wrapper');

// Create an instance with your API credentials.
var api = new SCORMCloud('appid', 'secretKey');

// See API documentation for additional examples.
api.getCourseList(function (error, result) {
  console.log(result);
  /*
  [
    {
      id: '810348d9-318e-48d5-b352-a1f6eb3a92cd',
      title: 'Example Course',
      registrations: 1,
      size: 3023399,
      tags: ['example', 'course'],
      learningStandard: 'scorm_12',
      createDate: '2017-11-10T16:30:00.000+0000'
    },
    ...
  ]
  */
});
```

For more information, see [Getting started with the Node.js client for the SCORM Cloud API](https://stevenwestmoreland.com/2017/11/nodejs-client-for-scormcloud-api.html).
