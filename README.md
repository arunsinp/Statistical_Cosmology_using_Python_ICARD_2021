```diff
- # Cosmology with Python: From Beginner to Advanced in red
```
colorize <- function(x, color) {
  if (knitr::is_latex_output()) {
    sprintf("\\textcolor{%s}{%s}", color, x)
  } else if (knitr::is_html_output()) {
    sprintf("<span style='color: %s;'>%s</span>", color,
      x)
  } else x
}

`r colorize("Cosmology with Python: From Beginner to Advanced","red")`
