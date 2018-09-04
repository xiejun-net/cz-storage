## cz-storage
前端缓存

## 安装

```
yarn add cz-storage || npm i cz-storage
```
## 使用

```js
import LS from 'cz-storage'

let value = {name: 'xiejun'}
// 设值
// put （<key>, value, expiredTime）
// expiredTime 过期时间单位是天 1/8 === 3小时
LS.put('key', value, 1)

// 获取值
LS.get('key')

// 清楚所有缓存
LS.clear()

// 删除某个key
LS.remove('key')
```