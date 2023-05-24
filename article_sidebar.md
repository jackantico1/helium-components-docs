# <ArticleSidebar/>

## Description
The `<CourseSyllabus/>` component shows the syllabus of the course, essentially the outline of the various sections, lessons, and topics that a course has

### Example code

```tsx
import { ArticleSidebar } from '@thoughtindustries/article-sidebar';

export function MyComponent() {
  // ...

  return (
    <ArticleSidebar
        id='adce-de45-5622-dasxs'
        showRating='true'
        showCustomFields='true'
        showSubmitRating='flase'/>
  );
}
```

## Props

| Name               | Required | Type         | Description               |
| ------------------ | -------- | -----------  | ------------------------- |
| id                 | Yes      | `ID`         | The ID of the article     |
| showRating         | Yes      | `Boolean`    | Show or hide the rating of the article      |
| showCustomFields   | Yes      | `Boolean`    | Show or hide the custom fields |
| showSubmitRating   | Yes      | `Boolean`    | Enable or disable learners to submit new ratings     |