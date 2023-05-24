# <RelatedContent/>

## Description
The `<RelatedContent/>` component shows content related to a specific piece of content This information is set in the Thought Industries admin interface and can be seen under `Catalog Settings > Detail Page` in the admin experience.

### Example code

```tsx
import { RelatedContent } from '@thoughtindustries/related-content';

export function MyComponent() {
  // ...

  return (
    <RelatedContent
        slug=''
        contentKind='Course'
        tabsView='true'/>
  );
}
```

## Props

| Name          | Required | Type         | Description               |
| ------------- | -------- | -----------  | ------------------------- |
| slug          | Yes      | `Slug`       | The slug of the content                  |
| numberOfItems   | Yes      | `Int`     | The number of related pieces of content to show, a number between 1 - 6    |