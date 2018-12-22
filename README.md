可测试一个或多个函数的执行次数、平均耗时、总耗时，并排序


## 使用

```javascript
yarn add --dev perfomance-js // or npm install --save-dev perfomance-js 
import p from 'performance-js'
```

## 参数
参数一： 一个函数名，或一个由函数组成的数组
参数二：执行次数，默认为 1

## 例子

1. 一个函数例子

    ```javascript
    p(f1, 100)
    function f1(){
        console.log('f1...')
    }
    ```

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