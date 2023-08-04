# Registration

## Description

The `Registration` component renders a form for learners to register for your site and gain access to the learner dashboard.

✨🎨 [View Component in Storybook](https://thoughtindustries.github.io/helium/?path=/story/packages-user-registration--registration-form) 🎨✨

## Props
| Name               | Required | Type                     | Description               |
| ------------------ | -------- | --------------------     | ------------------------- |
| redirectUrl        | No       | `String`                 | The URL to redirect the new learner once they sign up. For example, `/learn/dashboard`     |
| currentUser        | No       | `CurrentUser`            | The Current User, this prop relates to registration and redemption functionality of this component    |

## Example Code
```
import { Registration } from '@thoughtindustries/user'

export function MyComponent() {
  // ...

  return (
    <Registration
        redirectUrl='/learn/dashboard'/>
  );
}
```