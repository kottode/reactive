---
id: 1
status: done
assignee: FrameMuse
~github: pinely-international/reactive#3
---

## Problem

```tsx
const name = new State<string | null>(null)

<input when={{ change: select(name, event => event.currentTarget.value) }} />
```

## Proposal

```tsx
const name = new StateEvent<Event>(new Event)

<input when={{ change: name.from(event => event.currentTarget.value) }} />
```
