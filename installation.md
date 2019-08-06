# 安装
> 全局引入 -- 在 webpack 入口文件 main.js 中如下配置：

``` bash
# 安装
npm install yjk-mui --save

# 引入CSS文件
1. 直接引用  
import 'yjk-mui/package/yjkmui.min.css'
2. 引入CSS未压缩文件  
import 'yjk-mui/package/yjkmui.css'

# 引入JS
import ymui from 'yjk-mui'

# 注入到VUE
Vue.use(ymui)
```

> 按需引入 -- 在 入口文件 main.js 或 组件内 中如下配置：

```` bash
# 全局引入 main.js引入
import Button from 'yjk-mui/package/comps/components/button'
Vue.prototype.$button = Button

# 单个引入
import yButton from 'yjk-mui/package/comps/components/button'
import yCalender from 'yjk-mui/package/comps/components/calender'
...

components: {
  yButton,
  yCalender
  ...
}
````
