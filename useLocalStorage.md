# Local Storage in Angular

## Step 1: Save Data to Local Storage

### Save a String

```typescript
localStorage.setItem('username', 'Huy');
```

### Save a Number

```typescript
const id = 1;
localStorage.setItem('id', id.toString());
```

### Save an Object

```typescript
const user = {
  id: 1,
  name: 'Huy',
  email: 'huy@gmail.com'
};

localStorage.setItem('user', JSON.stringify(user));
```

---

## Step 2: Get Data from Local Storage

### Get a String

```typescript
const username = localStorage.getItem('username');
```

### Get a Number

```typescript
const id = Number(localStorage.getItem('id'));
```

### Get an Object

```typescript
const userData = localStorage.getItem('user');

if (userData) {
  const user = JSON.parse(userData);
}
```

---

## Step 3: Remove Data from Local Storage

### Remove One Item

```typescript
localStorage.removeItem('user');
```

### Remove All Items

```typescript
localStorage.clear();
```

---

# Formula

## Save

```typescript
localStorage.setItem('key', value);
```

## Get

```typescript
localStorage.getItem('key');
```

## Remove

```typescript
localStorage.removeItem('key');
```

## Clear All

```typescript
localStorage.clear();
```
