# GreenTick docs

Customer and developer documentation for [GreenTick](https://greentick.ai), built with Mintlify.

## Preview

Install the CLI, then from this directory:

```bash
npm i -g mint
mint dev
```

Open `http://localhost:3000`.

## API reference

`openapi.json` is a snapshot of the public Developer API. Regenerate it from the backend when routes change:

```bash
node -e "const {buildOpenApiDocument}=require('./green-tick-backend/services/developer/openApiDocument'); require('fs').writeFileSync('./greentick-docs/openapi.json', JSON.stringify(buildOpenApiDocument('https://api.greentick.ai'), null, 2))"
```

Run that command from the repository root.

## Publishing

Connect the GitHub app from the [Mintlify dashboard](https://dashboard.mintlify.com) so pushes to the default branch deploy the site.
