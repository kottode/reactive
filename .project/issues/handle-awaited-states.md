---
id: 7
assignee: FrameMuse
labels: enhancement
~github: pinely-international/reactive#10
---

```tsx

          {module.$.default()}
          {module.toAwaited(module => module.default())}
          {State.asyncIterableOf(module.toAwaited(module => module.default()))}
```
