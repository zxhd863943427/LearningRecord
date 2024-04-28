‍

#### 4-11

从今天起正式记录rcore日程。

##### 事件

安装了fireDBG调试器，为下一步的开发做准备。

完成题目：

* thread
* 智能指针

##### 问题

* [ ] 多线程并发的Arc智能指针与所有权机制不太理解`arc1.rs`​，难道线程的生命周期比调用的主进程还长？

  貌似理解了，确实不能使用借用创建`Arc`​，不然主线程结束就被回收了。
* [ ] 如何修改`Arc`​智能智能指向的结构体？

  看了下，这应该是不允许的行为，必须套一个`Mutex`​，跟Rc一样，参考见：[std/sync/struct.Arc](https://rustwiki.org/zh-CN/std/sync/struct.Arc.html)

##### 预期计划

‍

#### 4-12

##### 事件

今天在看rust的宏，感觉好复杂……

习题倒好做，了解一下细节都能做。

感觉`clippy`​真的好强啊……

##### 问题

* [ ] rust宏，难

##### 预期计划

* [ ] 把rust小册看完
* [ ] 手动实现rust小册中的宏

#### 4-13

##### 事件

继续做rustlings，目前进度105。

唉，算法基础还是太薄弱了，还得查资料。这是个不错的算法百科的[oi-wiki](https://oi-wiki.org/)。

##### 问题

* [X] test5里面的unsafe代码为什么要`&mut t as *mut u32 as usize`​这样的顺序转换类型？

  这似乎是rust不安全特性里的解引用裸指针的方法，参考：[解引用裸指针](https://kaisery.github.io/trpl-zh-cn/ch19-01-unsafe-rust.html?highlight=*mut#%E8%A7%A3%E5%BC%95%E7%94%A8%E8%A3%B8%E6%8C%87%E9%92%88)​

##### 预期计划

‍

#### 4-16

##### 事件

今天继续看rust quiz，感觉让自己变成大脑编译器了。

[quiz 19](https://dtolnay.github.io/rust-quiz/10) `let _ = s`​居然不会移动所有权？之后还能用s？奇妙。

##### 问题

* [ ] [quiz 10](https://dtolnay.github.io/rust-quiz/10)有点看不懂。

##### 预期计划

‍

#### 4-24

##### 事件

深读Rust 程序设计语言中的面向对象特性。

##### 问题

‍

##### 预期计划

‍
