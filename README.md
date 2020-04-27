# Configuring-Persian-font

```
Add the files of font of Vazir, into the src folder
```

add these codes to App.css:

```
.App {
  text-align: center;
  font-family: 'Vazir', sans-serif;
}

@font-face {
  font-family: Vazir;
  src: url('Vazir.eot');
  src: url('Vazir.eot?#iefix') format('embedded-opentype'),
       url('Vazir.woff2') format('woff2'),
       url('Vazir.woff') format('woff'),
       url('Vazir.ttf') format('truetype');
  font-weight: normal;
  font-style: normal;
}
@font-face {
  font-family: Vazir;
  src: url('Vazir-Bold.eot');
  src: url('Vazir-Bold.eot?#iefix') format('embedded-opentype'),
       url('Vazir-Bold.woff2') format('woff2'),
       url('Vazir-Bold.woff') format('woff'),
       url('Vazir-Bold.ttf') format('truetype');
  font-weight: bold;
  font-style: normal;
}
@font-face {
  font-family: Vazir;
  src: url('Vazir-Black.eot');
  src: url('Vazir-Black.eot?#iefix') format('embedded-opentype'),
       url('Vazir-Black.woff2') format('woff2'),
       url('Vazir-Black.woff') format('woff'),
       url('Vazir-Black.ttf') format('truetype');
  font-weight: 900;
  font-style: normal;
}
@font-face {
  font-family: Vazir;
  src: url('Vazir-Medium.eot');
  src: url('Vazir-Medium.eot?#iefix') format('embedded-opentype'),
       url('Vazir-Medium.woff2') format('woff2'),
       url('Vazir-Medium.woff') format('woff'),
       url('Vazir-Medium.ttf') format('truetype');
  font-weight: 500;
  font-style: normal;
}
@font-face {
  font-family: Vazir;
  src: url('Vazir-Light.eot');
  src: url('Vazir-Light.eot?#iefix') format('embedded-opentype'),
       url('Vazir-Light.woff2') format('woff2'),
       url('Vazir-Light.woff') format('woff'),
       url('Vazir-Light.ttf') format('truetype');
  font-weight: 300;
  font-style: normal;
}
@font-face {
  font-family: Vazir;
  src: url('Vazir-Thin.eot');
  src: url('Vazir-Thin.eot?#iefix') format('embedded-opentype'),
       url('Vazir-Thin.woff2') format('woff2'),
       url('Vazir-Thin.woff') format('woff'),
       url('Vazir-Thin.ttf') format('truetype');
  font-weight: 100;
  font-style: normal;
}
```
