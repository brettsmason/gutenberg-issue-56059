# @wordpress/create-block issue #56059

This is an example repository that showcases the issue with using @wordpress/create-block within a npm workspaces environment.

## Steps to reproduce

- Run `npm install` from the root of the repository
- Run `npm run create-block` from the root of the repository
- Answer the questions to the create-block script

The block should be scaffolded within the `src` directory of the `example-dynamic` plugin, however you'll see its in the root of the `example-dynamic` plugin instead.

The same issue can be seen if you run `npx @wordpress/create-block@latest --no-plugin` from within `web/app/plugins/example-dynamic/src`.
