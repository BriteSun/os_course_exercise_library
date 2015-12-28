# 操作系统练习题库

## 简介
这里包括从互联网上搜集的操作系统课程相关习题和答案，包括部分考研试题，版权属于各出题单位或个人。

其他题目和答案采用 Creative Commons Attribution/Share-Alike (CC-BY-SA) License。

MOOC OS习题集可采用gitbook的方式展现，可用于操作系统课程考试、练习、在线交互式答题。

**注意:** 
- 原来的目录1～15不再维护
- json 格式的题目数据以目录`data/json`下为准
- md 格式的题目数据以目录`data/md`下为准


## 练习题格式说明帮助
### 练习题例子
#### 单选题例子
```
1
下列四个操作系统中，是多用户分时操作系统的为（　） 。
- ( ) A.　CP/M 
- ( ) B.　MS-DOS 
- (x) C. UNIX 
- ( ) D.　VxWorks

> 知识点：操作系统概述。
> 出处：清华大学研究生入学考试测试练习2015
> 难度：1
> C　CP/M, MS-DOS都是单用户操作系统，VxWorks是实时操作系统，UNIX是多用户分时操作系统
```
#### 多选题例子
```
2
文件的逻辑结构有（　　　　　）类型
- [ ] A.顺序式 
- [x] B.流式 
- [ ] C.链接式 
- [x] D.记录式 
- [ ] E.索引式

> 知识点：文件系统。
> 出处：网络
> 难度：1
> BD 逻辑结构是指一个文件在用户面前所呈现的形式，有两种形式：①记录式文件(有结构式文件)，②字符流式文件（无结构式文件）,也称流式文件。
```
#### 填空题例子
```
5
产生死锁的原因<input type="text" width="10">。
- [x]  

> 知识点：死锁。
> 出处：网络
> 难度：1
> 产生死锁的原因主要是：
>（1） 因为系统资源不足。
>（2） 进程运行推进的顺序不合适。
>（3） 资源分配不当等。
> 如果系统资源充足，进程的资源请求都能够得到满足，死锁出现的可能性就很低，否则
> 就会因争夺有限的资源而陷入死锁。其次，进程运行推进顺序与速度不同，也可能产生死锁。
```
#### 问答题例子
```
4
何为页表和快表？它们各起什么作用？
- [x]  

> 知识点：物理内存管理实验。
> 出处：网络
> 难度：1
> 页表指出逻辑地址中的页号与所占主存块号的对应关系。 作用：页式存储管理在用动态重定位方式装入作业时，要利用页表做地址转换工作。
> 快表就是存放在高速缓冲存储器的部分页表。它起页表相同的作用。
> 由于采用页表做地址转换，读写内存数据时CPU要访问两次主存。有了快表，有时只要访问一次高速缓冲存储器，一次主存，这样可加速查找并提高指令执行速度。
```

### 格式说明
 * 整个练习题由五部分组成
 * “题目类型”说明::　位置：第一行；　内容：用数字1-5表示，1表示单选题，2表示多选题，3是判断题，4是问答题，5是填空题；
 * “题干”说明:: 位置：第二行；　内容：文字描述，叙述题目内容
 *  “选项”说明::　位置：第三行开始到　“> ”起始的行结束；内容：需要学生填写或选择的信息
   *  选项格式说明：
     1. 单选题格式：　"- ( )"开始，里面有x代表是正确选项，没有x则不是正确选项，注意，需要与答案和解释中的描述一致
     1. 多选题格式：　"- [ ]"开始，里面有x代表是正确选项，没有x则不是正确选项，注意，需要与答案和解释中的描述一致
     1. 填空题格式：　“- [x]  ”开始，在需要填空的地址插入`<input type="text" width="10">`代码
     1. 问答题格式：　“- [x]  ”开始

   * “知识点”说明::　位置：出现的以“> 知识点：”起始的行。注意：选项和注释之间有一个空行；内容：表示该题属于哪个知识点，[例子](https://github.com/chyyuu/os_course_exercise_library/edit/master/1/1.md)
     * 知识点列表
         1. 操作系统概述
         1. 实验环境准备实验
         1. 中断、异常与系统调用
         1. OS启动和中断处理实验
         1. 物理内存管理：连续内存分配
         1. 物理内存管理：非连续内存分配
         1. 物理内存管理实验
         1. 虚拟存储：缺页中断
         1. 虚拟存储：置换算法
         1. 虚拟内存管理实验
         1. 进程状态与控制
         1. 线程管理实验
         1. 进程管理实验
         1. 处理机调度
         1. 处理机调度实验
         1. 同步互斥
         1. 同步互斥：信号量
         1. 同步互斥：管程
         1. 同步互斥实验：信号量
         1. 同步互斥实验：条件变量
         1. 进程间通信
         1. 死锁
         1. 进程间通信实验
         1. 死锁实验
         1. 文件系统
         1. 文件系统实验
         1. I/O子系统
         1. I/O子系统实验
       
   * “出处”说明:: 出现以“> 出处：”起始的行。内容：表示该题从哪里找的，[例子](https://github.com/chyyuu/os_course_exercise_library/edit/master/1/1.md)
   * “难度”说明:: 出现以“> 难度：”起始的行。内容：用1-5表示，数值大难度越高，[例子](https://github.com/chyyuu/os_course_exercise_library/edit/master/1/1.md)
   * “答案和解释”说明:: 第四次出现的以“> ”起始的n行；内容：n(n大于等于0)个英文大写字母是选择题的答案，接着是空格，空格后面的是具体的解释，[例子](https://github.com/chyyuu/os_course_exercise_library/edit/master/1/1.md)




