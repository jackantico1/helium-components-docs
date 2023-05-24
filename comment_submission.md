# <CommentSubmission/>

## Description
The `<CommentSubmission/>` component allows users to submit comments to disscussion boards and comment threads.

### Example code

```tsx
import { CommentSubmission } from '@thoughtindustries/comment-submission';

export function MyComponent() {
  // ...

  return (
    <CommentSubmission
        slug=''
        contentKind='Course'
        tabsView='true'/>
  );
}
```

## Props [Need to do]

| Name          | Required | Type         | Description               |
| ------------- | -------- | -----------  | ------------------------- |
| slug          | Yes      | `Slug`       | The slug of the content                  |
| contentKind   | Yes      | `String`     | The type of the Contnet, either a `LearningPath` or a `Course`    |
| tabsView      | Yes      | `Boolean`    | If the content tabs should appear with a tabs view or as long piece of continues content    |