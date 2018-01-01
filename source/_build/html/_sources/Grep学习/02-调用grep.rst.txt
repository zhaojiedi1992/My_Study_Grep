02 调用grep
===============================================

调用grep的用法： 

.. code-block:: text

    grep options pattern input_file_names

2.1 命令行选项
------------------------------------------------

--help                      获取帮助
-V                          获取版本
--version                   获取版本
-e                          指定模式，可以多次使用
--regexp                    指定模式，可以多次使用
-f                          模式从文件来
-file                       模式从文件来
-i                          忽略大小写
-y                          忽略大小写
--ignore-case               忽略大小写
-v                          反向匹配
--invert-match              反向匹配
-w                          单词匹配
--word-regexp               单词匹配
-x                          整行匹配
--line-regexp               整行匹配
-c                          显示匹配的个数
--count                     显示匹配的个数
--color                     给匹配到的结果上色

-m                          最大的匹配个数
--max-count                 最大的匹配个数
-o                          只显示匹配的行
--only-matching             只显示匹配的行
-q                          静默模式
--quiet                     静默模式
--silent                    静默模式
-b                          显示偏移字节数
--btype-offset              显示偏移字节数
-H                          显示文件名
--with-filename             显示文件名
-n                          显示行号
--line-number               显示行号
-A                          匹配行后面几行显示
--after-content             匹配行后面几行显示
-B                          匹配行前面几行显示
--before-context            匹配行前面几行显示
-C                          匹配前后几行显示
--context                   匹配行前后几行显示

-d                          如果输入文件是目录，使用指定的action去处理，有read,skip,recurse,
--directories               如果输入文件是目录，使用指定的action去处理，有read,skip,recurse,
-r                          输入文件是目录，递归
--recursive                 输入文件是目录，递归
-R                          递归，且追踪符号链接

2.2 环境变量
-------------------------------------------------

grep是受到一些环境变量影响的。

2.3 退出码

如果退出码是0表示有匹配到的，1代表没有行选中，2代表有错误发生。
