# My Linux Configuration

## vim configuration

**特点：**

- 有cursor在当前行和当前列的光标
- 不生成备份、swap等文件
- 缩进
  - 换行自动缩进
  - 非python文件，一个tab代表两个空格
- 最下面有状态栏（显示当前模式、光标位置、编码格式等信息）
- 退出文件会询问是否报错
- 打开文件时，光标会停留在上次退出文件的位置
- 搜索高亮，可通过`-hl +hl`改
- 支持NERDTree / Tagbar / CtrlP(ag)
- python
  - 每个缩进有提示符对齐
  - 换行等操作自动PEP8缩进
  - 打开`.py`文件，pylint自动检查语法编码格式错误(按PEP8，忽略缺少文档字符串警告)，并在下方显示
- 等等


**快捷：**

```
+nu 显示行号
-nu 不显示行号
+hl 搜索词高亮
-hl 搜索词不高亮
,w 保存
,q 退出
,x 保存退出
,s 搜索当前光标所在word的python文档字符串
,S 搜索python字符串文档
,go 寻找python中当前word的定义处(比如跳转到某个类定义处)
,gf 寻找word在代码中相关的地方, 再选择跳转
,gd 寻找并跳转word定义或声明的地方
<F2> F2按键, 运行当前打开的python
<F3> F3按键, #注释代码. 在v模式下,可多行注释
<F4> F4按键, 打开下方快速搜索文件CtrlP(在CtrlP中F5是刷新列表)
<F5> F5按键, 打开左边目录树 NERDTree
<F6> F6按键, 打开右边 类/方法/函数显示 Tagbar
<F7> F7按键, pylint检查python代码(忽略C0111警告,缺少文档字符串)
<F8> F8按键, 尝试自动修复python代码,保持PEP8编码规范
<F9> F9按键, 关闭synastix或python-mode的语法检查quickfix窗口
```

pymode插件自带命令:
- `[[` 跳到上一个类或函数
- `]]` 跳到下一个类或函数
- `[M` 跳到上一个类或者方法
- `]M` 跳到下一个类或者方法
- `aC` 选择一个类， `daC yaC caC vaC`
- `iC`  选择一个inner类，同上
- `aM` 选择一个函数或者方法，同上


