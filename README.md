# algorithm

javascript 算法训练营

## 训练形式

训练形式以 issues 的形式提交代码

我会为每个题目创建一个 issues，在没个 issuess 下提交自己的代码即可

## 代码提交标准

主函数+leetcode 运行结果截图

## 示例

```js
var twoSum = function (nums, target) {
  const len = nums.length;
  let obj = {};
  obj[nums[0]] = 0;
  for (let i = 1; i < len; i++) {
    const targetNum = target - nums[i];
    if (obj[targetNum] || obj[targetNum] === 0) {
      return [obj[targetNum], i];
    } else {
      obj[nums[i]] = i;
    }
  }
};
```

备注：哈希表解决方案

运行结果截图：

![image.png](https://raw.githubusercontent.com/melody-core/algorithm/main/image/image.png)
