## Steps to reproduce the Issue
1. Install `casbin` from `npm`;
2. Import anything from `casbin` to any component that has a `.stories` file;
3. Run the storybook;

That's it. The issue should appear.
```
ERROR in ./node_modules/casbin/lib/esm/util/util.js
Module not found: Error: Can't resolve 'fs' in '/Users/armr/Documents/repro_casbin/node_modules/casbin/lib/esm/util'
 @ ./node_modules/casbin/lib/esm/util/util.js 14:0-25 74:8-19 85:8-20
 @ ./node_modules/casbin/lib/esm/util/index.js
 @ ./node_modules/casbin/lib/esm/index.js
 @ ./src/stories/Button.tsx
 @ ./src/stories/Button.stories.tsx
 @ ./src sync ^\.(?:(?:^|\/|(?:(?:(?!(?:^|\/)\.).)*?)\/)(?!\.)(?=.)[^/]*?\.stories\.(js|jsx|ts|tsx))$
 @ ./generated-stories-entry.js
 @ multi ./node_modules/@pmmmwh/react-refresh-webpack-plugin/client/ReactRefreshEntry.js ./node_modules/@storybook/core-client/dist/esm/globals/polyfills.js ./node_modules/@storybook/core-client/dist/esm/globals/globals.js (webpack)-hot-middleware/client.js?reload=true&quiet=false&noInfo=undefined ./node_modules/@pmmmwh/react-refresh-webpack-plugin/client/ErrorOverlayEntry.js ./storybook-init-framework-entry.js ./node_modules/@storybook/addon-docs/dist/esm/frameworks/common/config.js-generated-config-entry.js ./node_modules/@storybook/addon-docs/dist/esm/frameworks/react/config.js-generated-config-entry.js ./node_modules/@storybook/addon-links/dist/esm/preset/addDecorator.js-generated-config-entry.js ./node_modules/@storybook/addon-actions/dist/esm/preset/addDecorator.js-generated-config-entry.js ./node_modules/@storybook/addon-actions/dist/esm/preset/addArgs.js-generated-config-entry.js ./node_modules/@storybook/addon-backgrounds/dist/esm/preset/addDecorator.js-generated-config-entry.js ./node_modules/@storybook/addon-backgrounds/dist/esm/preset/addParameter.js-generated-config-entry.js ./node_modules/@storybook/addon-measure/dist/esm/preset/addDecorator.js-generated-config-entry.js ./node_modules/@storybook/addon-outline/dist/esm/preset/addDecorator.js-generated-config-entry.js ./.storybook/preview.js-generated-config-entry.js ./generated-stories-entry.js
```
