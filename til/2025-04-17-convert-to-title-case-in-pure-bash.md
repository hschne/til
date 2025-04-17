---
title: Convert to Title Case in Pure Bash
date: 2025-04-17
tags:
---

# Convert to Title Case in Pure Bash

You can convert a string to title case in pure bash.

```bash
to_title_case() {
  set ${*,,}
  echo ${*^}

}
to_title_case 'Something new and UNEXPECTED'
# Something New And Unexpected
```

You can also create fancier version that ignores articles and conjunctions.

```bash
to_title_case() {
  set ${*,,}
  set ${*^}
  echo -n "$1 "
  shift 1
  for f in ${*}; do
    case $f in A | The | Is | Of | And | Or | But | About | To | In | By)
      echo -n "${f,,} "
      ;;
    *) echo -n "$f " ;;
    esac
  done
  echo
}

to_title_case 'Something new and UNEXPECTED'
# Something New and Unexpected
```

[Source](https://stackoverflow.com/a/42943426)
