# Vim 
## 基础知识
vim 分为两种模式，即Command（命令）模式，以及edit（编辑）模式，其相互转换模式分别为i 和esc键
其中配置vim配置文件为vimrc 可通过`~/.vimrc`进入命令，对其进行全局的配置，也可以通过在github上进行搜索其中相关的配置，当然也可以通过一些插件管理
### 常用的一些命令
|命令|作用 |
|:---|:---:|
|`syntax on`|高亮|
|`set number`|显示行号|
|HJKL|命令模式上的左上下右|
|W|命令模式中向左移动，以单词为一个单位|
|B|命令模式中向右移动，以单词为一个单位|
|PageUp / Ctrl +b|向上翻页|
|PageDown / Ctrl +f|向下翻页|
|数字+gg|跳转指定行|
|`/`|命令模式的查找，后面跟着查找的单词，N为下一个，`shift +n`为上一个|
|CC|剪切掉当前行|
|C+数字+C|连续剪切从当前往下的行|
|U|undo 即为恢复上一个操作|
|P|粘贴 paste|
|v/V |可视化模式，分别为以字符为单位和以行为单位|
|Ctrl+N|内置代码补全，但是只能补全前文出现的代码。可使用插件|
## Vim 插件
vim插件功能很强大，后续会持续更新，目前只是一些基础的更新
vimPlug 为常用的插件管理插件，可在`vimrc`中插入
```shell
  call plug#begin()
      #内置插件
  call plug#begin()
```
在内置插件中写入插件的语句，然后再vim中输入 `PlugInstall`可以进行安装插件，之后便开始使用。如果要开启全局，同样在`vimrc`中写入插件的启动语句。即可全局使用，当删除插件的时候，需要把`vimrc`中相关语句删掉之后，在vim中输入`PlugClean`进行对插件的删除。

  可以在vim awesome网站中进行查找vim插件。