# Gravity Forms styling
Styling for the Gravity Forms plugin.

## Install
```sh
bower install trendwerk/gravity-forms-styling#~0.1.0 --save
```

## Usage
To use the gravity forms styling you need to `@include` the mixin in your stylesheet:

```scss
@include gravity-forms-styling();
```

You can extend the base styles to support Gravity Forms features like datepicker, using `datepicker: true` for example. See API reference below for all options.

### API
```scss
@include gravity-forms-styling((
  'datepicker': false,
  'datepicker-primary-color': #337ab7,
  'error-bordered': false,
  'error-color': #ce4844,
  'field-width': 70%,
  'file-upload': false,
  'horizontal-layout': 641px,
  'label-width': 30%,
));
```

#### Datepicker
Specify if datepicker styles should be included.

#### Datepicker: primary color
The primary color that's used in datepicker styling. Only applicable if `datepicker` is set to `true`.

#### Error: bordered
Specify if the main error should have a border. When set to `false`, the background color is set to `error-color` and the text color is set to white.

#### Error: color
The color that's used for error messages and highlighting fields with errors.

#### Field width
The default width of fields.

#### File upload
Specify if file upload styles should be included.

#### Horizontal layout
On smaller screens, labels and fields are positioned vertically (below each other). With this parameter you can specify from which screen width labels and fields should be positioned horizontally (next to each other).

#### Label width
The default width of labels.
