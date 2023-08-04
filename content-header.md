---
sidebar_position: 3
---
# Content Header

## Description

The `Content Header` component is used to display the `title`, `description`, and `image` of a Course or Learning Path. All content types, except learning paths, can also display `rating` and `ratingsCount` information.

✨🎨 [View Component in Storybook](https://thoughtindustries.github.io/helium/?path=/story/packages-content-header--base) 🎨✨

## Props

| Name        | Required | Type                 | Description                                                      |
| ----------- | -------- | -------------------- | ---------------------------------------------------------------- |
| contentKind | Yes      | <code>string</code>  | The contentKind of the Content, e.g., `learningPath`, `course`.  |
| slug        | Yes      | <code>slug</code>    | The slug of the content that should be displayed.                |
| showStars   | No       | <code>boolean</code> | Controls whether a course's rating is displayed, shown in stars. |
| showImage   | No       | <code>boolean</code> | Controls whether a piece of content's Detail Image is displayed. |

## Example code

```tsx
import { ContentHeader } from '@thoughtindustries/content';

export function MyComponent() {
  // ...

  return (
    <ContentHeader
      contentKind={contentKind}
      slug={courseSlug}
      showStars={true}
      showImage={true}
    />
  );
}
```