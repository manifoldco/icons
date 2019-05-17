# Manifold Icons

Manifold’s icon system

## Setup

```bash
npm i
cp .manifold.yml.example .manifold.yml
```

This will work out-of-box, but edit `.manifold.yml` if necessary (separate
file allows changes without accidentally committing and breaking things for
others).

## Usage

```bash
npm i @manifoldco/icons
```

```ts
import { arrow_right } from '@manifoldco/icons';
```

## Publishing to npm

```bash
npm run publish
```

_Note: this is **different** from `npm publish`!_

Other repos use Git tagging, but this is a little different. We’re using
@pika/pack’s npm publish script, which is a command prompt UI. For that reason,
publishing happens locally.

If testing something, then release it as a **prerelease** rather than a patch
version. Patch versions get pushed everywhere, so treat them as production!
