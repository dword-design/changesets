# @changesets/config

> Utilities for reading and parsing Changeset's config

```tsx
import { parse, read, ValidationError } from "@changesets/config";

let config = await read(process.cwd(), workspaces);

let config = parse({ commit: true }, workspaces);

try {
  return parse({ commit: true }, workspaces);
} catch (err) {
  if (err instanceof ValidationError) {
    let message = err.message;
  } else {
    throw err;
  }
}
```
