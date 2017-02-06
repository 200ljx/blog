> ui-router加载模板文件后解析编译内部script引入文件

使用angular装饰器装饰 uiViewDirective 指令，加入ui-router-require-polyfill.js
<a href="https://github.com/kuitos/angular-utils/blob/1.3.1/polyfills/ui-router-require-polyfill.js" target="_blank">参考</a>

> 正则表达式匹配页面中的script标签src信息

上述ui-router-require-polyfill.js中有一个获取script标签的正则表达式，如下

`/<script\s+((?!type=('|")text\/ng-template('|")).)*>.*<\/script>/gi`

此正则表达式在ie8中只会匹配到最后一个script，需改成如下即可：

`/<script\b[^<]*(?:(?!<\/script>)<[^<]*)*<\/script>/gi`

> angular中使用调用jquery插件

设置自定义angular指令（如下），在对应html标签上添加指令属性即可

```
.directive('myDatepicker', function() {
            return {
                // Restrict it to be an attribute in this case
                restrict: 'A',
                // responsible for registering DOM listeners as well as updating the DOM
                link: function (scope, element, attrs) {
                    $(element).datepicker();
                }
            }
        })
```

> 未完待续。。。