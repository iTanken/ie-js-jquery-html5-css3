# ie-js-jquery-html5-css3

🌏 用于 `IE6/7/8/9` 页面兼容性的优化脚本。

## 相关内容

[低版本浏览器（IE6+）页面兼容性问题相关处理](https://zixizixi.cn/low-version-browser-page-compatibility)

## 使用方法

```html
  <script>
    if (navigator.userAgent.indexOf('MSIE') > -1 || navigator.userAgent.indexOf('rv:11') > -1) {
      document.write('<script src="./shim-2.6.9.min.js"><\/script>');
    }
  </script>
  <script src="./jquery-1.12.4.min.js"></script>
  <!--[if (gte IE 6)&(lte IE 8)]>
    <script src="./jquery-ie678.min.js"></script>
  <![endif]-->
  <!--[if IE 9]>
    <script src="./jquery-ie9.min.js"></script>
  <![endif]-->
  <!--[if (gte IE 6)&(lte IE 9)]>
    <script>
      $(function() {
        $(".example_css3_class").each(function() {
          PIE.attach(this);
        });
      });
    </script>
  <![endif]-->
```

## 开源协议

[MIT License](https://opensource.org/licenses/MIT)

## 鸣谢

* [core-js](https://github.com/zloirock/core-js)
* [jquery](https://github.com/jquery/jquery)
* [html5shiv](https://github.com/aFarkas/html5shiv)
* [css3-mediaqueries-js](https://github.com/iTanken/css3-mediaqueries-js)
* [selectivizr](https://github.com/keithclark/selectivizr)
* [css3pie](https://github.com/lojjic/PIE)
