---
sort: 3
---

# Code Blocks ёёё

`inline code`

[`inline code inside link`](./)

```
:root {
	@for $level from 1 through 12 {
		@if $level % 4 == 0 {
			--toc-#{$level}: #{darken($theme-white, 4 * 8.8%)};
		} @else {
			--toc-#{$level}: #{darken($theme-white, $level % 4 * 8.8%)};
		}
	}
}
```

**Highlight:**

``` scss
:root {
  @for $level from 1 through 12 {
    @if $level % 4 == 0 {
      --toc-#{$level}: #{darken($theme-white, 4 * 8.8%)};
    } @else {
      --toc-#{$level}: #{darken($theme-white, $level % 4 * 8.8%)};
    }
  }
}
```

``` note
This is note3
```

``` tip
It’s tip
```

``` warning
Strong prose may provoke extreme mental exertion. Reader discretion is strongly advised.
```

``` danger
Mad scientist at work!
```
