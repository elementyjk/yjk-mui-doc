# Calender 日历
----
### 基础用法
日历用于选择年月日，提供相应的点击事件
``` html
<ym-calender :sundayStart="true" :agoDayHide='Math.ceil(new Date().getTime() / 1000 - 86000)' :markDate="[ '2019-08-03' ]" :markDateMore="[ { date: '2019-08-06' } ]" :choseDay="choseDay"></ym-calender>
<ym-calender :sundayStart="false" :agoDayHide='Math.ceil(new Date().getTime() / 1000 - 86000)' :markDate="[ '2019-08-03' ]" :markDateMore="[ { date: '2019-08-06' } ]" :choseDay="choseDay"></ym-calender>
```

### 属性
| 参数      | 说明    | 类型      | 可选值       | 格式       | 默认值   |
|---------- |-------- |---------- |------------- |----------- |-------- |
| sundayStart     | 以星期日开头   | Boolen  | false true  | true |
| markDate     | 标记日期   | Array  | - | yyyy-MM-dd | - |
| agoDayHide     | 禁用某日期之前   | Number  | - | 00000000001 | - |
| futureDayHide     | 禁用某日期之后   | Number  | - | 16000000001 | - |
| calendarLang     | 星期   | Array  | - | - | ['日', '一', '二', '三', '四', '五', '六'] |