# Configuring-Persian-font (IRANSans)

**To change the font family of the whole application use the `styled-components` provider**

1. first create a `fonts` folder inside assets of src and copy your fonts there

2. second create a `css` folder and create `fontiran.css` and `style.css` files 

fontiran.css

```js
/**
*
*	Name:			IRAN Sans-Serif Font
*	Version:		5.0
*	Author:			Moslem Ebrahimi (moslemebrahimi.com)
*	Created on:		Dec 25, 2012
*	Updated on:		Sep 01, 2017
*	Website:		             http://fontiran.com
*	Copyright:		Commercial/Proprietary Software
--------------------------------------------------------------------------------------
فونت های ایران سن سریف یک نرم افزار مالکیتی محسوب می شود. جهت آگاهی از قوانین استفاده از این فونت ها لطفا به وب سایت (فونت ایران دات کام) مراجعه نمایید
--------------------------------------------------------------------------------------
IRAN Sans-serif fonts are considered a proprietary software. To gain information about the laws regarding the use of these fonts, please visit www.fontiran.com 
--------------------------------------------------------------------------------------
This set of fonts are used in this project under the license: (.....)
--------------------------------------------------------------------------------------
*	
**/
@font-face {
  font-family: IRANSans;
  font-style: normal;
  font-weight: 900;
  src: url('../fonts/eot/IRANSansWeb(FaNum)_Black.eot');
  src: url('../fonts/eot/IRANSansWeb(FaNum)_Black.eot?#iefix')
      format('embedded-opentype'),
    /* IE6-8 */ url('../fonts/woff2/IRANSansWeb(FaNum)_Black.woff2')
      format('woff2'),
    /* FF39+,Chrome36+, Opera24+*/
      url('../fonts/woff/IRANSansWeb(FaNum)_Black.woff') format('woff'),
    /* FF3.6+, IE9, Chrome6+, Saf5.1+*/
      url('../fonts/ttf/IRANSansWeb(FaNum)_Black.ttf') format('truetype');
}
@font-face {
  font-family: IRANSans;
  font-style: normal;
  font-weight: bold;
  src: url('../fonts/eot/IRANSansWeb(FaNum)_Bold.eot');
  src: url('../fonts/eot/IRANSansWeb(FaNum)_Bold.eot?#iefix')
      format('embedded-opentype'),
    /* IE6-8 */ url('../fonts/woff2/IRANSansWeb(FaNum)_Bold.woff2')
      format('woff2'),
    /* FF39+,Chrome36+, Opera24+*/
      url('../fonts/woff/IRANSansWeb(FaNum)_Bold.woff') format('woff'),
    /* FF3.6+, IE9, Chrome6+, Saf5.1+*/
      url('../fonts/ttf/IRANSansWeb(FaNum)_Bold.ttf') format('truetype');
}
@font-face {
  font-family: IRANSans;
  font-style: normal;
  font-weight: 500;
  src: url('../fonts/eot/IRANSansWeb(FaNum)_Medium.eot');
  src: url('../fonts/eot/IRANSansWeb(FaNum)_Medium.eot?#iefix')
      format('embedded-opentype'),
    /* IE6-8 */ url('../fonts/woff2/IRANSansWeb(FaNum)_Medium.woff2')
      format('woff2'),
    /* FF39+,Chrome36+, Opera24+*/
      url('../fonts/woff/IRANSansWeb(FaNum)_Medium.woff') format('woff'),
    /* FF3.6+, IE9, Chrome6+, Saf5.1+*/
      url('../fonts/ttf/IRANSansWeb(FaNum)_Medium.ttf') format('truetype');
}
@font-face {
  font-family: IRANSans;
  font-style: normal;
  font-weight: 300;
  src: url('../fonts/eot/IRANSansWeb(FaNum)_Light.eot');
  src: url('../fonts/eot/IRANSansWeb(FaNum)_Light.eot?#iefix')
      format('embedded-opentype'),
    /* IE6-8 */ url('../fonts/woff2/IRANSansWeb(FaNum)_Light.woff2')
      format('woff2'),
    /* FF39+,Chrome36+, Opera24+*/
      url('../fonts/woff/IRANSansWeb(FaNum)_Light.woff') format('woff'),
    /* FF3.6+, IE9, Chrome6+, Saf5.1+*/
      url('../fonts/ttf/IRANSansWeb(FaNum)_Light.ttf') format('truetype');
}
@font-face {
  font-family: IRANSans;
  font-style: normal;
  font-weight: 200;
  src: url('../fonts/eot/IRANSansWeb(FaNum)_UltraLight.eot');
  src: url('../fonts/eot/IRANSansWeb(FaNum)_UltraLight.eot?#iefix')
      format('embedded-opentype'),
    /* IE6-8 */ url('../fonts/woff2/IRANSansWeb(FaNum)_UltraLight.woff2')
      format('woff2'),
    /* FF39+,Chrome36+, Opera24+*/
      url('../fonts/woff/IRANSansWeb(FaNum)_UltraLight.woff') format('woff'),
    /* FF3.6+, IE9, Chrome6+, Saf5.1+*/
      url('../fonts/ttf/IRANSansWeb(FaNum)_UltraLight.ttf') format('truetype');
}
@font-face {
  font-family: IRANSans;
  font-style: normal;
  font-weight: normal;
  src: url('../fonts/eot/IRANSansWeb(FaNum).eot');
  src: url('../fonts/eot/IRANSansWeb(FaNum).eot?#iefix')
      format('embedded-opentype'),
    /* IE6-8 */ url('../fonts/woff2/IRANSansWeb(FaNum).woff2') format('woff2'),
    /* FF39+,Chrome36+, Opera24+*/ url('../fonts/woff/IRANSansWeb(FaNum).woff')
      format('woff'),
    /* FF3.6+, IE9, Chrome6+, Saf5.1+*/
      url('../fonts/ttf/IRANSansWeb(FaNum).ttf') format('truetype');
}
```

style.css
```js
@import url(fontiran.css); /* لینک فایلی که وظیفه بارگذاری فونت ها را برعهده دارد */
body {
  font-family: IRANSans !important;
  font-weight: 300;
}
h1,
h2,
h3,
h4,
h5,
h6,
input,
textarea {
  font-family: IRANSans !important;
}
::-webkit-scrollbar {
  width: 7px;
}

/* Track */
::-webkit-scrollbar-track {
  border-radius: 4px;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: #afb6d055;
  border-radius: 10px;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #afb6d0;
}

```

3. third create a `themeProvider.js` file (which we use styled components here)

```js
import { createGlobalStyle } from 'styled-components'

export const ThemeProvider = createGlobalStyle`
  * {
    @import url('../assets/css/fontiran.css');
    font-family: IRANSans !important;
    direction: rtl;
    text-align: right;
    cursor: default;
  }
`
```

4. and lastly in `index.js` file

```js
import React from 'react'
import ReactDOM from 'react-dom'
import './index.css'
import './assets/css/fontiran.css'
import App from './App'
import * as serviceWorker from './serviceWorker'
import { ConfigProvider } from 'antd'
import fa_IR from 'antd/es/locale/fa_IR'
import { ThemeProvider } from './theme/themeProvider'

ReactDOM.render(
  <React.StrictMode>
    <ConfigProvider locale={fa_IR}>
      <ThemeProvider />
      <App />
    </ConfigProvider>
  </React.StrictMode>,
  document.getElementById('root')
)

// If you want your app to work offline and load faster, you can change
// unregister() to register() below. Note this comes with some pitfalls.
// Learn more about service workers: https://bit.ly/CRA-PWA
serviceWorker.unregister()
```
