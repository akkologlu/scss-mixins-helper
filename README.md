# SCSS-MIXINS-HELPER

This is a lightweight SCSS package that provides a collection of reusable mixins for common styling tasks.

## Installation

Install SCSS-MIXINS-HELPER with npm

```bash
  npm install scss-mixins
```

or

```bash
  yarn add scss-mixins
```

## Usage

Import the mixins into your SCSS file:

```scss
@import "/node_modules/scss-mixins-helper/src/mixins.scss";
```

Then, you can use the mixins like any other SCSS function:

```scss
.primary-button {
  @include button(#007bff, #fff);
}

.secondary-button {
  @include button(#ddd, #333);
}
```

### Flexbox Mixin:

```scss
.flex-row {
  @include flex-box(row, space-between, center);
}

.flex-column {
  @include flex-box(column, center, flex-start);
}
```

### Styled Text Mixin:

```scss
.heading {
  @include styled-text(24px, bold, #333);
}

.paragraph {
  @include styled-text(16px, normal, #666);
}
```

### Cover Background Mixin:

```scss
.hero {
  @include cover-background;
  background-image: url("path/to/your/image.jpg");
}
```

### Absolute Position Mixin:

```scss
.fixed-top-right {
  @include absolute(fixed, 20px, 20px, auto, auto);
}

.absolute-center {
  @include absolute(absolute, 50%, 50%, -50%, -50%);
  transform: translate(-50%, -50%);
}
```

These are just a few examples of how to use the mixins in this package. Refer to the source code for a complete list of available mixins and their options.

## Contributing

We welcome contributions to this package! Please refer to my GitHub repository: https://github.com/akkologlu/scss-mixins-helper for contribution guidelines or open issues/pull requests to discuss improvements.

## License

This package is licensed under the MIT License. See the [MIT](https://choosealicense.com/licenses/mit/) file for details.
