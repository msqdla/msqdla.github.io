[TOC]

#### Python 001

##### iterdir()函数——**罗列文件夹的内容**

1 from pathlib import Path # 导入pathlib模块中的Path对象
2 p = Path('F:\\python\\第1章\\工作信息表1') # 指定一个文件夹的路径
3 p1 = p.iterdir() # 获取指定文件夹中所有文件和子文件夹的路径
4 for i in p1: # 遍历获取结果
5       print(i) # 输出获取的路径

 ---

1 from pathlib import Path # 导入pathlib模块中的Path对象
2 p = Path('F:\\python\\第1章\\工作信息表2') # 指定一个文件夹的路径
3 workbook = p.glob('*.xlsx') # 获取指定文件夹中所有工作簿的路径
4 for i in workbook: # 遍历获取结果
5     print(i) # 逐个输出工作簿的路径

 ---
