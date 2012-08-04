##Sass配置使用

###安装
需要ruby环境
在终端输入
<pre>
gem install compass
</pre>
该命令会自动下载和安装 COMPASS 及其依赖模块(包括 SASS）。

###使用
创建一个compass项目
在终端输入
<pre>
compass create _programName
</pre>

这个命令会创建一个包含一系列文件的目录，其中最重要的是配置文件 config.rb，其他文件如果你不需要都可以删除。

在 config.rb 中你可以修改 SASS 和 CSS 的目录及其它一些基础设置。

###实时编译Sass文件
终端输入
<pre>
comprass watch
</pre>
COMPASS 将会实时监控 SASS 目录的文件变化，只要你一保存文件，立即将相应文件编译为 CSS 文件。

##让 Firebug 里显示 SASS 行号
既然现在用 SASS 来开发，我们就需要浏览器开发工具中显示样式对应的 SASS 行号而不是 CSS 行号了。

如果你使用 Firebug 可以安装 <code>FireSass</code> 来解决这个问题。

首先修改 SASS 的配置文件让其在 CSS 文件中输出调试信息，打开项目目录下的 config.rb，添加一行并保存

<pre>sass_options = {:debug_info => true}</pre>
如果你在 watch，结束掉重新运行配置的修改才会生效。

