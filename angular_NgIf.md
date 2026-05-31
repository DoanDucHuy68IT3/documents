# 🅰️ Document Angular

### Step 1: Import library

```typescript
import { NgIf } from '@angular/common';
```

### Step 2: Declare in imports

```typescript
imports: [NgIf], // 👈 Must declare here for standalone components
```

### Step 3: Use in HTML

#### Formula 1

```html
<div *ngIf="user">
```

**Meaning:** If `user` is not `null`.

#### Formula 2

```html
<div *ngIf="user; else noUser">
```

**Meaning:** Use `if else`.

```html
<ng-template #noUser>
  <p>There's not information user</p>
</ng-template>
```
