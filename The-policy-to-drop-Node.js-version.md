https://github.com/prettier/prettier/issues/13142#issuecomment-1483882351

This document may be moved to another location in the future, but for now I am writing it down here.

```
if (
  (VERSION reached EoL) && (
    (We need to use a new feature that is not available in VERSION) ||
    (It has been a year since VERSION reached EoL)
  )
) {
  drop(VERSION)
}
```