```md renderer="angular" language="mdx"
{/* Badge.stories.mdx */}

import { Canvas, Meta, Story } from '@storybook/addon-docs';

import { Badge } from './badge.component';

<Meta title="Badge" component={Badge} />

export const Template = (args) => ({ props: args });

<Canvas>
  <Story 
    name="warning"
    args={{ 
      status: 'warning', 
      label: 'Warning',
    }}>
    {Template.bind({})}
  </Story>
  <Story 
    name="neutral"
    args={{ 
      status: 'neutral', 
      label: 'Neutral',
     }}>
    {Template.bind({})}
  </Story>
  <Story 
    name="error"
    args={{ 
      status: 'error', 
      label: 'Error',
    }}>
    {Template.bind({})}
  </Story>
</Canvas>
```

```md renderer="react" language="mdx"
{/* Badge.stories.mdx */}

import { Canvas, Meta, Story } from '@storybook/addon-docs';

import { Badge } from './Badge';

<Meta title="MDX/Badge" component={Badge} />

export const Template = (args) => <Badge {...args } />;

<Canvas>
  <Story 
    name="warning"
    args={{
      status: 'warning', 
      label: 'Warning',
    }}>
    {Template.bind({})}
  </Story>
  <Story 
    name="neutral"
    args={{
      status: 'neutral', 
      label: 'Neutral',
    }}>
    {Template.bind({})}
  </Story>
  <Story 
    name="error"
    args={{
      status: 'error', 
      label: 'Error',
    }}>
    {Template.bind({})}
  </Story>
</Canvas>
```

```md renderer="svelte" language="mdx"
{/* Badge.stories.mdx */}

import { Canvas, Meta, Story } from '@storybook/addon-docs';

import Badge from './Badge.svelte';

<Meta title="MDX/Badge" component={Badge} />

export const Template = (args) => ({
  Component: Badge,
  props: args,
});

<Canvas>
  <Story 
    name="warning"
    args={{
      status: 'warning',
      label: 'Warning',
    }}>
    {Template.bind({})}
  </Story>
  <Story 
    name="neutral"
    args={{
      status: 'neutral',
      label: 'Neutral',
    }}>
    {Template.bind({})}
  </Story>
  <Story 
    name="error"
    args={{
      status: 'error',
      label: 'Error',
    }}>
    {Template.bind({})}
  </Story>
</Canvas>
```

```md renderer="vue" language="mdx" tabTitle="mdx-2"
{/* Badge.stories.mdx */}

import { Canvas, Meta, Story } from '@storybook/addon-docs';

import Badge from './Badge.vue';

<Meta title="MDX/Badge" component={Badge} />

export const Template = (args, { argTypes }) => ({
  props: Object.keys(argTypes),
  components: { Badge },
  template: '<Badge v-bind="$props" />',
});

<Canvas>
  <Story 
    name="warning"
    args={{
      status: 'warning', 
      label: 'Warning',
    }}>
    {Template.bind({})}
  </Story>
  <Story 
    name="neutral"
    args={{
      status: 'neutral', 
      label: 'Neutral',
    }}>
    {Template.bind({})}
  </Story>
  <Story 
    name="error"
    args={{
      status: 'error', 
      label: 'Error',
    }}>
    {Template.bind({})}
  </Story>
</Canvas>
```
```md renderer="vue" language="mdx" tabTitle="mdx-3"
{/* Badge.stories.mdx */}

import { Canvas, Meta, Story } from '@storybook/addon-docs';

import Badge from './Badge.vue';

<Meta title="MDX/Badge" component={Badge} />

export const Template = (args) => ({
  components: { Badge },
  setup() {
    return { args };
  },
  template: '<Badge v-bind="args" />',
});

<Canvas>
  <Story 
    name="warning"
    args={{
      status: 'warning',
      label: 'Warning',
    }}>
    {Template.bind({})}
  </Story>
  <Story 
    name="neutral"
    args={{
      status: 'neutral',
      label: 'Neutral',
    }}>
    {Template.bind({})}
  </Story>
  <Story 
    name="error"
    args={{
      status: 'error',
      label: 'Error',
    }}>
    {Template.bind({})}
  </Story>
</Canvas>
```