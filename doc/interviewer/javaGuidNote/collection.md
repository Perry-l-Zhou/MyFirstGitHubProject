# Collection

## List：有序，可重复

### ArrayList：Object数组
支持高效随机访问，适用于频繁查找操作，线程不安全，结尾预留容量空间占用内存
### Vector：Object数组
线程安全。
### LinkedList：双向链表，使用场景极少，作者都不用
不支持高效随机访问，增删复杂度受下标位置影响，线程不安全，每个元素占用更多空间
## Set：无序，不可重复

### HashSet：基于HashMap实现

### LinkedHashSet：HashSet子类，基于LinkedHashMap实现

### TreeSet：红黑树（自平衡排序二叉树）

## Queue：有序，可重复，先进先出

### PriorityQueue：Object数组

### ArrayQueue：Object数组+双指针

# Map：键值对存储数据，k无序，不可重复；v无序，可重复

## HashMap
JDK1.8之前是数组+链表，数组为主体，链表为解决hash冲突存在。JDK1.8之后链表长度大于阈值8则判断数组长度小于64，则扩容，否则转红黑树。
## LinkedHashMap
继承自HashMap，底层是数组、链表、红黑树组成。增加双向链表以保证顺序。
## Hashtable
数组+链表组成，数组为主体，链表为解决hash冲突存在
## TreeMap
自平衡的排序二叉树--红黑树

# 双向链表
链表有pre和next，首尾不连接
# 双向循环链表
链表有pre和next，首尾连接