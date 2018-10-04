# Happy-ya
The first repository
http://codeforces.com/submissions/Petr/page/22
膜拜日本大神代码

现阶段对输入输出掌握不够精准，其次，最一般的代码题都是沿用c的思想，不需要强行套用hashmap

同大余数问题 饥饿的小易先往后放放

争取养着每天做两三道算法的习惯
LeetCode  2018年10月3日星期三16点22分
从今天开始记录leetcode经验，真是时间长了就忘记了。 
map.put(nums[i], map.getOrDefault(nums[i], 0) + 1);//用getOrDefault(如果有就这么填, 如果没有的话 填默认值) 
hashmap的计数使用方法，特别常用，因为套用了hash表速度快。
solution284 Find the Duplicate Number hashmap过一遍查重ok
solution62 Unique Paths 典型DP 用二维数组做 就ok
if(i==0||j==0)  grid[i][j] = 1;                  
else
grid[i][j] = grid[i][j-1] + grid[i-1][j] ;       
solution48 Rotate Image 整体思路和按圈打印数组类似 在一套（或者多套）循环中换位置
for(int j =i;j<n-i-1;j++){                        
 int temp =matrix[i][j];                          
matrix[i][j] = matrix[n-j-1][i];                 
matrix[n-j-1][i] = matrix[n-i-1][n-j-1];        
matrix[n-i-1][n-j-1] = matrix[j][n-i-1] ;       
matrix[j][n-i-1] = temp;                             
solution46 Permutations 全排列 算法能看懂想不出来 难度系数较大放在包里以后直接调用



LeetCode  2018年10月4日星期四17点54分
solution49 Group Anagrams  类似字典功能 物以类聚思想
Map<String, List> ans = new HashMap<String, List>();//字符串Key 对应 List存Value
将给定的单词String 分门别类 先char[] ca = s.toCharArray(); 临时char[]储存收录的词String
sort()一下 如果不相同 就另建一个新的Array[] 储存放在Value里 

solution289 Game of Life 类似岛屿island of water 都是通过搜索来寻求满足条件的来更新matrix[][]
