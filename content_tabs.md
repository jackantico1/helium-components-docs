# <ContentTabs/>

## Description
The `<ContentTabs/>` component shows information about a content's tabs such as information about the syllabus, the instructors, testimonials, or other products related to the content. This information is pulled from the actual content itself and can be seen under `Catalog Settings > Detail Page` in the admin experience.

### Example code

```tsx
import { ContentTabs } from '@thoughtindustries/content-tabs';

export function MyComponent() {
  // ...

  return (
    <ContentTabs
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
| contentKind   | Yes      | `String`     | The type of the Contnet, either a `LearningPath` or a `Course`    |
| tabsView      | Yes      | `Boolean`    | If the content tabs should appear with a tabs view or as long piece of continues content    |