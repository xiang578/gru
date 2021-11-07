## [[2021 September]]

1. [5847. 找到所有的农场组](https://leetcode-cn.com/problems/find-all-groups-of-farmland/) 暴力，一个格子是不是起点可以通过判断上边格子和左边格子得知。
2. [5848. 树上的操作](https://leetcode-cn.com/problems/operations-on-tree/) 模拟，先想清楚然后再写
3. [5849. 好子集的数目](https://leetcode-cn.com/problems/the-number-of-good-subsets/) 枚举所有合法组合的个数
4. [5866. 数组的最大公因数排序 - 力扣（LeetCode） (leetcode-cn.com)](https://leetcode-cn.com/problems/gcd-sort-of-an-array/) 并查集 + [[素数筛]]，有相同因子的数会在同一个集合中。
5. [5865. 访问完所有房间的第一天 - 力扣（LeetCode） (leetcode-cn.com)](https://leetcode-cn.com/problems/first-day-where-you-have-been-in-all-the-rooms/) 漏看一个条件，实际上是傻逼题，还是错了好几次，1e9 相加会爆 int 以及返回答案前也需要取模。
6. [1977. 划分数字的方案数 - 力扣（LeetCode） (leetcode-cn.com)](https://leetcode-cn.com/problems/number-of-ways-to-separate-numbers/) 挺复杂的，写了好几个小时，看题解才过…… n=3500，暗示是 $O(n^2)$ 的算法
	1. 设以 nums[i...j] 为结尾的方案数是 $dp_{i,j}$
	2. 可以发现 $dp_{i,j}=\sum_{k=2*i-j-1}^{i-1}dp[k][i-1], dp_{i,j+1}=dp_{i,j} + dp_{2*i-j-2,i-1}$，维护一个前缀和。
	3. 比较 nums[i...j] 和 nums[2*i-j-1...i-1]  大小，可以先预处理出以 i 和 j 开始的字符串的最大相同长度 lcp[i][j]。
7. [LCP 42. 玩具套圈 - 力扣（LeetCode） (leetcode-cn.com)](https://leetcode-cn.com/problems/vFjcfV/)：r 比较小，可以暴力枚举，被抬一手还是没有写出来。。。需要注意细节。不要提交 debug。
8. [LCP 43. 十字路口的交通 - 力扣（LeetCode） (leetcode-cn.com)](https://leetcode-cn.com/problems/Y1VbOX/)
9. [36. 有效的数独 - 力扣（LeetCode） (leetcode-cn.com)](https://leetcode-cn.com/problems/valid-sudoku/)：判断数独当前局面是否合法。
	1. [37. 解数独 - 力扣（LeetCode） (leetcode-cn.com)](https://leetcode-cn.com/problems/sudoku-solver/)：求解数独，上一题的进阶。

## [[2021 August]]

1. 210815 [[5832 构造元素不等于两相邻元素平均值的数组]] 排序 + 贪心
2. 210816 [[526 优美的排列]] DP + 状态压缩
3. 210817 [[1969 数组元素的最小非零乘积]] 快速幂
4. 210818 [[552 学生出勤记录 II]] DP
5. 210829  [5856. 完成任务的最少工作时间段](https://leetcode-cn.com/problems/minimum-number-of-work-sessions-to-finish-the-tasks/)：DP + 子集合枚举
6.  210829 [5857. 不同的好子序列数目](https://leetcode-cn.com/problems/number-of-unique-good-subsequences/)：不重复的 01 子序列个数，DP
7.  210829 [940. 不同的子序列 II](https://leetcode-cn.com/problems/distinct-subsequences-ii/)：和 5857 类似，字符串包含小写字母
