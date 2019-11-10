### vue通过axios设置ajax

+ 首先在脚本中引入axios
+ 可以使用vue-resources的写法，将vue.prototype.$http=axios,将axios绑定到vue的原型上
+ 之后使用this.$http.get()来调用ajax请求，在后面用.then()来定义回调函数
+ post方法调用都是类似的，只不过需要三个参数，第一个参数是url，第二个参数是查询参数，第三个参数设置提交样式