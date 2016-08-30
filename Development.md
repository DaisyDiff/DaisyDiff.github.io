---
layout: default
---

# Installing
 * Clone (or download) from our GitHub [repository](https://github.com/DaisyDiff/DaisyDiff).
 * `mvn install`

# NetBeans

## Maven and NetBeans
When you use [NetBeans](https://netbeans.org/downloads/), install its Maven plugin (in Tools > Plugins). NetBeans (8.0.1) doesn't let you configure Maven much. However, edit your `~/.m2/settings.xml`. Maven embedded in NetBeans honours it.

## Testing
Menu Run > Test Project.

## Regenerating `expected.html`
Edit `pom.xml`. Uncomment `<CREATE_EXPECTED_RESULTS>true</CREATE_EXPECTED_RESULTS>`. Run tests. Then run:

```
cd target/test-classes
# You must have test files two or three folders below. Otherwise add a variation of the following command.
for f in testdata/*/*/expected.html; do cp "$f" "../../src/test/resources/$f"; done
for f in testdata/*/*/*/expected.html; do cp "$f" "../../src/test/resources/$f"; done
```