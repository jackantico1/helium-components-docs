---
sidebar_position: 5
---

# Login

## Description

The `Login` component renders a form for learners to enter email address and password to sign in, as well as a link to retrieve password in case the learner forgets their password. Once learner signs in successfully, learner will be redirected to the dashboard page.

✨🎨 [View Component in Storybook](https://thoughtindustries.github.io/helium/?path=/story/packages-user-login--login-form) 🎨✨

## Props
None

## Example code

```tsx
import { Login } from '@thoughtindustries/user';

export function MyComponent() {
  // ...

  return (
    <Login />
  );
}
```