```js filename="Button.stories.js|jsx|ts|tsx" renderer="common" language="js"
import { Button } from './Button';

export default {
  /* 👇 The title prop is optional.
  * See https://storybook.js.org/docs/react/configure/overview#configure-story-loading
  * to learn how to generate automatic titles
  */
  title: 'Button',
  component: Button,
  argTypes: {
    label: {
      description: 'Overwritten description',
      table: {
        type: {
          summary: 'Something short',
          detail: 'Something really really long',
        },
      },
      control: {
        type: null,
      },
    },
  },
};
```