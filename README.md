测试程序执行时间
可测试一个或多个函数的执行次数、平均耗时、总耗时，并排序


## 使用

```javascript
yarn add --dev perfomance-js // or npm install --save-dev perfomance-js 
import p from 'performance-js'
```

## 参数

> p(fns[,num])

- 参数 fns：类型：函数 或 由函数组成的数组
- 参数 num：执行次数，默认为 1

## 例子

1. 一个函数例子

    ```javascript
    p(f1, 100)
    function f1(){
        console.log('f1...')
    }
    ```
    ![效果图](https://user-images.githubusercontent.com/26001948/50371161-2d313400-05f0-11e9-8443-dfff8240d017.jpg)

2. 多个函数例子

    ```javascript
    p([f1, f2], 1000)
    function f1(){
        console.log('f1...')
    }

    function f2(){
        console.log('f2...')
    }
    ```
    ![效果图](https://user-images.githubusercontent.com/26001948/50371147-eba08900-05ef-11e9-9b62-fd5a3b52b1fa.jpg)