# Bootstrap

## Components

- ### _Base Classes_

  Bootstrap group as many shared properties as possible inot a base class, like `.btn`, and then group individual styles for each variant into modifier classe, like `.btn-primary` or `btn-success`.

- ### _Modifiers_

  Seeing how Bootstrap's components are built with a base class approach. The bulk of the styling is contained to a base class, while style variations are confined to modifier classe.

- ### _Root variables_
  Here are the variables included that can be accessed anywhere Bootstrap's CSS is loaded:

```
:root {
  --bs-blue: #0d6efd;
  --bs-indigo: #6610f2;
  --bs-purple: #6f42c1;
  --bs-pink: #d63384;
  --bs-red: #dc3545;
  --bs-orange: #fd7e14;
  --bs-yellow: #ffc107;
  --bs-green: #198754;
  --bs-teal: #20c997;
  --bs-cyan: #0dcaf0;
  --bs-white: #fff;
  --bs-gray: #6c757d;
  --bs-gray-dark: #343a40;
  --bs-primary: #0d6efd;
  --bs-secondary: #6c757d;
  --bs-success: #198754;
  --bs-info: #0dcaf0;
  --bs-warning: #ffc107;
  --bs-danger: #dc3545;
  --bs-light: #f8f9fa;
  --bs-dark: #212529;
  --bs-font-sans-serif: system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", "Liberation Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
  --bs-font-monospace: SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;
  --bs-gradient: linear-gradient(180deg, rgba(255, 255, 255, 0.15), rgba(255, 255, 255, 0));
}
```

---

## Layout

- ### _Breakpoints_
  Bootstrap includes six default breakpoints, sometimes referred to as _grid tiers_, for building **respoonsively**, these brekpoints can be custumized if when using the source Sass files.

| Breakpoint        | class Inflx | Dimensions |
| ----------------- | ----------- | ---------- |
| X-Small           | none        | <576px     |
| Small             | sm          | >=566px    |
| Medium            | md          | >=768px    |
| Large             | lg          | >=992px    |
| Extra Large       | xl          | >= 1200px  |
| Extra extra large | xxl         | >= 1440px  |

- ### _Containers_

  Containers are the most basic layout element in Bootstrap, and are required when uding the default grid system. They are used mostly to contain, pad and _sometimes_ center the content within them.

- ### _HTML Classes_
  - Navigation:
    - navbar: The wrapping for the navegation;
    - navbar-expand {-sm|-md|-lg|-xl}: Responsive collapsing;

## Must use files from Bootstrap

bootstrap.css

> this one has all the css styling and classes

bootstrap.css.map
bootstrap.min.css

> this is the one that should be linked on the index.html file
