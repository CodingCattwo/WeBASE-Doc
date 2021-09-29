
# 实训2 实现转账合约

## 题目描述

<!-- 这里写题目描述 -->

编写一个HelloWorld合约，合约包含一个string变量、一个get方法和一个set方法。
- 构造函数初始化该变量为"Hello world!"
- 提供get方法获取变量string的值（调用get方法不产生区块）
- 提供set方法设置string的值（产生区块）

**示例1：**
```
通过合约IDE部署合约
```

**示例2：**
```
部署合约后，直接调用get方法，获得string的返回值为"Hello world!"
```

**示例3：**
```
调用set方法，设置string为"123"，获得交易回执，回执状态为0x0(成功)

调用get方法，获取string的值，显示为"123"
```


## 解法

<!-- 这里可写通用的实现逻辑 -->

伪代码

```ts
pragma solidity >=0.4.25 <0.6.11;
contract HelloWorld {
    string a;
    constructor;
    getter;
    setter;
}
```

<!-- tabs:start -->

### **Solidity**

<!-- 这里可写当前语言的特殊实现逻辑 -->

```ts
pragma solidity >=0.4.25 <0.6.11;

contract HelloWorld {
    string name;

    constructor() public {
        name = "Hello, World!";
    }

    function get() public view returns (string memory) {
        return name;
    }

    function set(string memory n) public {
        name = n;
    }
}
```

### **...**

```

```

<!-- tabs:end -->




