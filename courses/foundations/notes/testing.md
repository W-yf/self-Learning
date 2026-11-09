# Testing：测试的作用与边界

参考：[MIT 6.031 Spring 2022 — Reading 3: Testing](https://web.mit.edu/6.031/www/sp22/classes/03-testing/)、[MIT 6.005 Spring 2016 — Reading 3: Testing / Validation](https://ocw.mit.edu/ans7870/6/6.005/s16/classes/03-testing/#validation)。

## 核心知识

- 测试通过选择输入、执行程序并检查结果来发现问题。
- 一组测试通过，只表明这些用例的检查项符合预期，通常不能据此推断程序对所有合法输入都正确。
- 如果测试正确表达了约定，一个不符合预期的结果就足以说明实现存在错误。
- 未测试某个输入，不等于程序在该输入上一定出错。

## Test-first programming

- 模块是可以和系统其他部分分开设计、实现、测试和推理的一部分；当前先以函数为例。
- spec 说明参数类型及约束、返回值类型，以及返回值与输入之间的关系。实现提供行为，client 调用模块，两者都受 spec 约束。
- 测试用例由具体输入和 spec 要求的预期行为组成；测试套件是一组测试用例。
- Test-first 的顺序是先写 spec，再根据 spec 写测试，最后写实现。预期结果来自 spec，因此不需要先知道实现采用什么算法。

## Systematic testing

- correct 评价测试套件本身：测试必须是 spec 的合法 client，并接受所有符合 spec 的合法实现。错误实现不在“必须通过”的范围内。
- thorough 表示测试能够发现实际实现中可能出现的、尤其是程序员容易犯的错误；不等于用例更多，也不保证找出所有 bug。
- small 表示用较少的测试用例保持测试快速、易更新和可频繁运行。small 要与 thorough 平衡，不能随意删除负责发现重要错误的用例。

## 个人理解与例子

几个测试通过，不足以说明函数在所有情况下都正确。还需要考虑其他输入，例如两个数相等的情况。

按功能逐个采用 Spec → Test → Implement，可以更早发现问题。测试失败时，尚未验证的代码和最近改动范围较小，因此排查更集中。

下面是一个用于说明问题的错误实现，约定是返回两个整数中较大的值：

```cpp
int larger(int a, int b) {
    if (a > b) {
        return a;
    }
    return 0;
}
```

它能通过 `(2, 1)`、`(5, 3)`、`(9, 4)` 这三个用例，但 `larger(1, 1)` 返回 `0`，约定要求返回 `1`。这个输入暴露了原测试未发现的错误。

对于约定“当 `value < low` 时返回 `low`”的 `clamp(value, low, high)`，即使实现尚未编写，也可以从 spec 得到：

```cpp
assert(clamp(0, 1, 2) == 1);
```
