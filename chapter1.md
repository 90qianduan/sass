## 使用 Sass \(Using Sass\) {#t3}

Sass 可以通过以下三种方式使用：作为命令行工具；作为独立的 Ruby 模块 \(Ruby module\)；或者作为 Rack-enabled 框架的插件（例如 Ruby on Rails 与 Merb）。无论哪种方式都需要先安装 Sass gem （Windows 系统需要先[安装 Ruby](http://rubyinstaller.org/)）：

```
gem install sass
```

在命令行中运行 Sass：

```
sass input.scss output.css
```

监视单个 Sass 文件，每次修改并保存时自动编译：

```
sass --watch input.scss:output.css
```

监视整个文件夹：

```
sass --watch app/sass:public/stylesheets
```

更多命令的用法请通过`sass --help`获取帮助。

在 Ruby 中使用 Sass 也非常容易，Sass gem 安装完毕后运行`require "sass"`然后按照下面的方法使用[Sass::Engine](http://sass-lang.com/docs/yardoc/Sass/Engine.html)：

```
engine = Sass::Engine.new("#main {background-color: #0000ff}", :syntax => :scss)
engine.render #=> "#main { background-color: #0000ff; }\n"
```





