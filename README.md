# pintos 实验说明

## 实验总体设计

实验来自[CS 140: Operating Systems (Spring 2020)](http://web.stanford.edu/~ouster/cgi-bin/cs140-spring20/index.php)，包含以下若干个Projects：

- [x] [Problem Set 0: Synchronization](http://web.stanford.edu/~ouster/cgi-bin/cs140-spring20/problemSet0.php) 单人，必做，10 月 10 日 22：00 前提交
- [x] [Project 1: Threads](http://web.stanford.edu/~ouster/cgi-bin/cs140-spring20/pintosProjects.php) 组队，必做，11 月 7 日 22：00 前提交
- [x] [Project 2: User Programs](http://web.stanford.edu/~ouster/cgi-bin/cs140-spring20/pintosProjects.php) 组队，必做，11 月 28 日 22：00 前提交
- [ ] [Project 3: Virtual Memory](http://web.stanford.edu/~ouster/cgi-bin/cs140-spring20/pintosProjects.php) 组队，选做，12 月 5 日 22：00 前提交
- [ ] [Project 4: File Systems](http://web.stanford.edu/~ouster/cgi-bin/cs140-spring20/pintosProjects.php) 没要求

### Problem Set 0: Synchronization

Note: this problem set should be done individually, not in teams. The teams will apply to the four Pintos projects. For this problem set it is OK to discuss general strategy with other people, and it's OK to give and receive help tracking down problems, but you must write your own code.

### Project 1: Threads

See the Pintos documentation for details on this project:

- [Assignment](http://web.stanford.edu/~ouster/cgi-bin/cs140-spring20/pintos/pintos_2.html)
- [Frequently asked questions](http://web.stanford.edu/~ouster/cgi-bin/cs140-spring20/pintos/pintos_2.html#Project%201%20FAQ)
- [Template for design document](http://web.stanford.edu/~ouster/cgi-bin/cs140-spring20/pintos/threads.tmpl)

Additional notes and modifications for Project 1:

- A common mistake students make throughout the Pintos projects is to use `malloc` carelessly. If you call `malloc`, you must check the result to make sure the system did not run out of memory (and you must do something reasonable if memory does run out). In addition, you must be sure that any memory you allocate is eventually freed.

### Projects 2: User Programs

See the Pintos documentation for details on this project:

- [Assignment](http://web.stanford.edu/~ouster/cgi-bin/cs140-spring20/pintos/pintos_3.html)
- [Frequently asked questions](http://web.stanford.edu/~ouster/cgi-bin/cs140-spring20/pintos/pintos_3.html#Project%202%20FAQ)
- [Template for design document](http://web.stanford.edu/~ouster/cgi-bin/cs140-spring20/pintos/userprog.tmpl)

### Project 3: Virtual Memory

See the Pintos documentation for details on this project:

- [Assignment](http://web.stanford.edu/~ouster/cgi-bin/cs140-spring20/pintos/pintos_4.html)
- [Frequently asked questions](http://web.stanford.edu/~ouster/cgi-bin/cs140-spring20/pintos/pintos_4.html#Project%203%20FAQ)
- [Template for design document](http://web.stanford.edu/~ouster/cgi-bin/cs140-spring20/pintos/vm.tmpl)

## 提交方式和要求

- 

## 评分标准

