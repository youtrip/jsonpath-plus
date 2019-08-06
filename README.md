# jsonpath-plus
Fork of pip jsonpath (https://pypi.python.org/pypi/jsonpath/)，A Improved version, Base PIP jsonpath v0.82.

##说明(Chinese)：
jsonpath-plus是基于PIP jsonpath v0.82的改进加强版本。之前的版本在读取节点不规则的json结构时，导致输出的list不一致，这对下一步处理数据产生了干扰，特别是把数据传入Pandas tocsv或者tosql都会大概率出现失败。本版本在核心文件上增加了判断，如果某个节点缺失，将默认输出空字符串或者空字典确保输出的list长度一致。

这个改进版本人已经正常使用半年，运行非常好，有需要推荐使用这个版本替换PIP的jsonpath。

### Readme (English)
Jsonpath-plus is an improved and enhanced version of PIP jsonpath v0.82. Previous versions of Pandas tocsv or tosql were used to read irregular json structures of nodes, resulting in inconsistent output lists, which interfered with the next step of data processing. This version adds a judgment to the core file that if a node is missing, an empty string or dictionary will be output by default to ensure that the list output is of the same length.