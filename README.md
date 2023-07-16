---
license: mit
title: '文献调研神器'
python_version: 3.10.10
---


# 文献调研神器

这个项目旨在轻松快捷的调研相关文献! 具体包含如下功能:
* 自动搜索相关文献, 提供真实有出处的引用.
* 自动生成LaTeX格式，markdown格式的调研结果.


# 部署方法
1. 克隆此仓库：
```angular2html
git clone https://github.com/red-tie/auto-survey
```
2. 安装依赖：
```angular2html
pip install -r requirements.txt
```
3. 将`main.py`中`your key` 替换成有效的open key
```angular2html
openai.api_key = "your key"
```
4. 将`main.py`中的`target_title`替换成自己的标题
```angular2html
target_title = "Reinforcement Learning for Robot Control"
```
5. 运行`main.py`
```angular2html
python main.py
```
所得到的结果结果会保存在 outputs 目录的对应文件夹下，文件夹以运行main.py的时间为名。 用户可以在能运行tex文件的地方直接运行main.tex
得到相应的pdf文件， 或者直接查看survey.md文件即可. 



# 参考与学习
代码主要参考了如下优秀项目：
https://github.com/kaixindelele/ChatPaper
https://github.com/CCCBora/auto-draft