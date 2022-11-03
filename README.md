# LearningOS_Record
Record my daily process when learning os-comp2022-winter



# Daily Record

## Week 1(2022-10-17 -- 10-24)

> 大致浏览了一下rust学习路线,感觉看[简单英语学rust](https://kumakichi.github.io/easy_rust_chs/Chapter_20.html)这本书挺适合我的,后续讲按照这本书来学习, 同时辅助[贵系小学期的slides](https://lab.cs.tsinghua.edu.cn/rust/).

1. 先了解了一下rust的基本语法,比如变量命名,函数等,完成了rustlings的variable, functions, if以及对应的quiz.
2. 学习rust的生命周期和所有权.完成了rustlings的move_semantics, primitive_type and part of struct.

some notes :
1. 所有权转移其实转移的是对内存的所有权, 但是mut/immut还是取决于变量的定义.

## Week 2(2022-10-25 -- 11-01)

这周完成了rustling的小练习, 初步对rust有了一定的了解, 因为之前对riscv的指令集有一定的了解,所以打算直接去看rcore,中间碰到什么问题再去翻手册.

## Week 3(2022-11-02 -- 11-09)

目前浏览了rcore的部分代码, 看完了前两章(也就是在裸机上实现hello world以及实现批处理系统)
1. 第一章做的主要是移除rust std-lib的支持,仅仅使用core-lib来实现print hello-world
2. 第二章主要是实现批处理系统, 此时的批处理系统是只能一个app一个app的装载, 即所有app都装载到同一个地址,一个结束了才能下一个.主要的实现是trap的实现.

然后目前正在看第三章,相比于第二章, 它主要增加了对一次性将全部app load进来的支持,也就是将不同的app load到不同的地址.同时也实现了yield.
前两章没有什么练习需要实现,第三章是实现一个打印task information的小练习, 希望这周能完成.
