# HTML STORYBOOK SETUP

it's not easy to find documentation (up-to-date Documentation) and examples for Storybook with HTML requirements. This setup will allow you to work with atomic approach (Atoms/Molecules/Organisms/Templates/Pages) using js files and stories. Thanks to Storyout you will be able to export your components as HTML code. You can use Controls and actions.


node version I'm using for this project : node/16.10.0 \
npm version : 7.18.1 \
yarn version : 1.22.10 \
Storybook version : 6.1.21

## Project and Storybook Setup

please run :

### `yarn install` or `npm install`
to install the project with dependencies
### `yarn storybook`
to lunch Storybook.

## Addons

### `storyout`
-> this addon will display an HTML tab next to controls with the output

#### how to render html in your story

```javascript
import { withSource, html } from 'storybook-addon-storyout';

const render = html();

export default {
  title: 'Button',
  decorators: [withSource],
  parameters: {
    source: { render },
  },
};
```

#### source
https://storybook.js.org/addons/storybook-addon-storyout

### `a11y`
-> this addon will display an Accessibility tab with accessibility rules and violations.

#### source
https://storybook.js.org/addons/@storybook/addon-a11y