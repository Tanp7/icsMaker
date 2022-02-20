# Info
通过教务网上的课表制作ICS文件，可导入到Google日历、Outlook日历及其他支持ICS文件的日历
# usage
## 你可以使用Git或者Git工具：
```zsh
git clone https://github.com/Tanp7/icsMaker  
```
## 使用方法
- 通过教务网上的课表数据手动输入xlsx文件  
- 运行excelReader.py  
- 运行main.py  
-  同目录会生成对应课表的ICS文件，导入日历即可。
#  FAQ



## 提示找不到xlrd？
可能是你没装xlrd
- macOS/Linux可以执行以下操作：
```zsh
pip install xlrd
```
- Windows可以选择用Pycharm安装

## 编译excelReader提示找不到文件？
classInfo.xlxs这个表格需要在同名文件夹内

## 编译main.py提示正在配置课堂信息后程序意外退出？
修改main.py中第153行
```python
 with open('conf_classInfo.json', 'r', encoding='UTF-8') as f:
 ```
 中的```UTF-8```改为```Unicode```.

## 还在改进中
如果觉得有用可以fork&star
