# 第一章|万物皆数 | 《数学要素》
# 使用软件：
jupyterlab (建议使用chrome打开）
# 重点快捷键
ctrl + shift + _: 在光标所在的地方分块  
esc + M: 变成markdown格式  
esc + Y：变成代码环境  
space twice（敲击两次空格）：Jupyterlab中markdown中的分段  
ctrl + enter: 执行  
esc + b：在当前cell下方生成一个新的cell  
esc + a：在当前cell上方生成一个新的cell  
# 写作公式
This is a symbol, $A$  
$$a + b = 2$$
# 绘图
（请直接去jupyterlab中试用）  
# 注释
CTRL + /： comment
# 学习步骤
![Example Image](images/example.png)

# 一些个人问题
## Q：现在，我还有个问题，我本地安装的python是3.10版本，但我通过anaconda使用python时，显示的版本是3.9
## 这意味着你可能有多个 Python 版本安装在你的系统上，并且它们可能来自不同的来源（例如，一个来自官方 Python 安装包，另一个来自 Anaconda）。

### 检查当前 Python 版本
你可以在终端或命令提示符中运行以下命令来查看当前使用的 Python 版本：
```python
python --version
```
如果你在使用 Anaconda 环境，可以运行：
```python
conda list python
```
这将显示当前激活的 Anaconda 环境中安装的 Python 版本。

### 解决方案
1. 更新 Anaconda 环境中的 Python 版本
你可以更新 Anaconda 环境中的 Python 版本，使其与系统中的 Python 版本一致。以下是步骤：

激活你的 Anaconda 环境（如果还没有激活）：
```python
conda activate myenv  # 请将myenv替换为你的环境名称
```
更新 Python 版本：
```python
conda install python=3.10
```
2. 创建一个新的 Anaconda 环境
如果你想要一个干净的环境，可以创建一个新的 Anaconda 环境并指定所需的 Python 版本：
```python
conda create --name myenv python=3.10
```
然后激活新的环境：
```python
conda activate myenv
```
3. 指定 Python 解释器
如果你在使用集成开发环境（IDE）如 VSCode、PyCharm 等，你可以指定使用的 Python 解释器。

在 VSCode 中：

打开命令面板（F1 或 Ctrl+Shift+P）。
输入并选择 Python: Select Interpreter。
选择你想要使用的 Python 3.10 解释器路径。
在 PyCharm 中：

打开 Settings/Preferences。
导航到 Project: <project name> -> Python Interpreter。
点击齿轮图标并选择 Add，然后选择 Existing environment，选择 Python 3.10 的解释器路径。
确保路径正确
有时，路径设置可能会导致使用错误的 Python 版本。你可以检查并确保路径正确：
```python
which python  # 在Linux/MacOS上
where python  # 在Windows上
```
这将显示当前终端中使用的 Python 解释器的路径。确保它指向你期望的 Python 版本。

### 总结
更新 Anaconda 环境中的 Python 版本：使用 conda install python=3.10。
创建新的 Anaconda 环境：使用 conda create --name myenv python=3.10 并激活新环境。
在 IDE 中指定 Python 解释器：确保你的 IDE 使用正确的 Python 解释器路径。
检查路径设置：使用 which python 或 where python 确保路径正确。
通过这些步骤，你可以确保在 Anaconda 环境中使用期望的 Python 版本。




