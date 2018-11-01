# autocompile-less

Compile LESS file on save.

---

Add the parameters on the first line of the LESS file.

```
out          (string) path of CSS file to create
sourcemap    (bool)   create sourcemap file
compress     (bool)   compress CSS file
main         (string) path to your main LESS file to be compiled
autoprefixer (string) autoprefixer parameterers
```
Check [this](https://github.com/browserslist/browserslist#best-practices) for a how-to on autoprefixer parameters.

## Example
less/styles.less
```scss
// out: ../css/styles.css, sourcemap: true, compress: true, autoprefixer: defaults

@import "my/components/select.less";
```

less/my/components/select.less
```scss
// main: ../../styles.less

.select {
  height: 100px;
  width: 100px;
}
```
