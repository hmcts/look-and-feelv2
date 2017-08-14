# Look and Feel

GOV.UK look and feel as a single easy import (at least that's the goal).

## Usage

To use look-and-feel first add it to your `package.json`:

    > yarn add @hmcts/look-and-feel

Then configure it in your `app.js`:

    const express = require('express');
    const app = express();
    ...
    const lookAndFeel = require('@hmcts/look-and-feel');
    lookAndFeel.configure(app);
    ...

## Documentation

All documentation is stored in the [docs] folder.

## Development

We use the [Dockerfile] and [docker-compose.yml] to create a development
container used for running tests, etc.

To start the container run:

```
make
```

Once complete you will be dropped in to a shell where you can run `yarn`.

[Dockerfile]:https://github.com/hmcts/nodejs-one-per-page/blob/master/Dockerfile
[docker-compose.yml]:https://github.com/hmcts/nodejs-one-per-page/blob/master/docker-compose.yml