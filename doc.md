
## **1. Grid & Column Shortcodes**

### **Basic Usage**
Use `grid` to define a row and `col` to define columns.

```html
{{< grid >}}
  {{< col cols="6" >}} Column 1 {{< /col >}}
  {{< col cols="6" >}} Column 2 {{< /col >}}
{{< /grid >}}
```

### **Custom Column Width**
Set `cols` to define column size (default is 6/12).

```html
{{< grid >}}
  {{< col cols="8" >}} Larger column {{< /col >}}
  {{< col cols="4" >}} Smaller column {{< /col >}}
{{< /grid >}}
```

### **Markdown & Images**
Enable Markdown inside a column with `isMarkdown="true"`.

```html
{{< col cols="8" isMarkdown="true" >}}
  ### Title
  Some markdown content.
{{< /col >}}
```

To add images:
```html
{{< col cols="6" >}}
  {{< image src="images/example.png" >}}
{{< /col >}}
```

---

## **2. R Code Example**
Wrap R code inside fenced blocks:

```r
ggplot(mtcars, aes(wt, mpg)) +
geom_point(size = 3, aes(colour = factor(cyl))) +
theme(legend.position = "none")
```

---


