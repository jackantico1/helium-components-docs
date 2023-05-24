# <CourseSyllabus/>

## Description
The `<CourseSyllabus/>` component shows the syllabus of the course, essentially the outline of the various sections, lessons, and topics that a course has

### Example code

```tsx
import { CourseSyllabus } from '@thoughtindustries/course-syllabus';

export function MyComponent() {
  // ...

  return (
    <CourseSyllabus
        slug=''
        contentKind='Course'
        tabsView='true'/>
  );
}
```

## Props

| Name               | Required | Type         | Description               |
| ------------------ | -------- | -----------  | ------------------------- |
| slug               | Yes      | `Slug`       | The slug of the course                  |
| preview            | Yes      | `String`     | The type of the Contnet, either a `LearningPath` or a `Course`      |
| condense           | Yes      | `Boolean`    | If true accordion is expanded to show full outline, if false accordion is shows a part of the outline    |
| visibilityDepth    | Yes      | `Section`, `Lesson`, or `Topic`    | If the prop is “section” it shows just the sections of the outline, if prop is “lesson” it shows the lesson and the sections, and if prop is “topic” shows all three of the outline.    |