# Manifold Icons

Manifold’s icon system

## Setup

```bash
npm install
```

## Usage

```bash
npm i @manifoldco/icons
```

```jsx
import { arrow_right } from '@manifoldco/icons';

const Icon = () => (
  <svg
    viewBox="0 0 1024 1024"
    xmlns="http://www.w3.org/2000/svg"
    xmlnsX="http://www.w3.org/1999/xlink"
  >
    <path d={arrow_right} />
  </svg>
);
```

_Note: the `viewBox="0 0 1024 1024"` is the most important part!_

## Publishing to npm

You must be logged into npm and have access to the `@manifoldco` team to publish.

```bash
npm run deploy
```

Other repos use Git tagging, but this is a little different. We’re using
@pika/pack’s npm publish script, which is a command prompt UI. For that reason,
publishing happens locally.

If testing something, then release it as a **prerelease** rather than a patch
version. Patch versions get pushed everywhere, so treat them as production!
