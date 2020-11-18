# git_collect_sub
个人收集的有用项目，使用git submodule方式，引用已有项目。
## submodule的使用
参考：[Git 子模块submodule的使用](https://blog.csdn.net/h4x0r_007/article/details/108167592)
- 首次拉取
  ```
  git clone https://github.com/h4x0r139/git_collect_sub.git
  git submodule init
  git submodule update
  ```
- 更新
  ```
  git pull
  git submodule foreach git submodule update
  ```

**常见问题**

- git 拉取`errno 54`问题
  [解决参考](https://blog.csdn.net/qq_42347755/article/details/90347988)：使用`ssh clone`
  ```
  error: RPC failed; curl 56 LibreSSL SSL_read: SSL_ERROR_SYSCALL, errno 54
  fatal: the remote end hung up unexpectedly
  fatal: early EOF
  fatal: index-pack failed
  ```
- git 拉取`errno 56`问题
errno 56，有大文件或者提交缓存方面的问题：增大缓存配置，比如下面就是配置提交缓存为 500M。
  ```
  git config http.postBuffer 524288000
  git config https.postBuffer 524288000
  ```  

## 引用的项目列表
- [CyC2018/CS-Notes](https://github.com/CyC2018/CS-Notes)：技术面试必备基础知识、Leetcode、计算机操作系统、计算机网络、系统设计、Java、Python、C++
- [fucking-algorithm](https://github.com/labuladong/fucking-algorithm)，[电子书](https://labuladong.gitbook.io/algo/)：68k，刷算法思路，数据结构、动态规划、算法思维、高频面试题
- [LeetCodeAnimation](https://github.com/MisterBooo/LeetCodeAnimation)：60k，动画演示leetcode算法
- [hello-algorithm](https://github.com/geekxh/hello-algorithm)：19.7k，小浩算法图解，后端

## TODO


### Android 面试
- [Android 高级开发整理的面试题以及答案](https://github.com/jinguangyue/Android-Advanced-Interview)
Java 算法实现
https://github.com/TheAlgorithms/Java
https://github.com/h4x0r139/Java
Algorithms, 4th Edition 算法4精华笔记，通俗理解，算法收集与强化
https://github.com/MeandNi/Algorithms4-Common

算法图解：https://github.com/zhanwen/AlgorithmDiagram
牛客网-剑指offer：https://github.com/DmrfCoder/AlgorithmAndDataStructure
cache
https://github.com/Tencent/MMKV

### LeetCode

- [azl397985856/leetcode](https://github.com/azl397985856/leetcode)：37.5k，力扣加加
- [yuanguangxin/LeetCode](https://github.com/yuanguangxin/LeetCode)：LeetCode题目分类与面试问题整理：
- [LeetCodeGraphically](https://github.com/lefex/LeetCodeGraphically)：图解 LeetCode 算法：
- [afatcoder/LeetcodeTop](https://github.com/afatcoder/LeetcodeTop)：4.2k，汇总各大互联网公司（阿里，百度，字节，快手）容易考察的高频leetcode题