# <Bookmark/>

## Description
The `<Bookmark/>` component allows users to bookmark pieces of content, edit their existing bookmark folders, and create new bookmark folders.

### Example code

```tsx
import { Bookmark } from '@thoughtindustries/bookmark';

export function MyComponent() {
  // ...

  return (
    <Bookmark id='adce-de45-5622-dasxs'/>
  );
}
```

## Props

| Name               | Required | Type         | Description               |
| ------------------ | -------- | -----------  | ------------------------- |
| id                 | Yes      | `ID`         | The ID of the content     |