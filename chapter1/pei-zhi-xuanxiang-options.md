### 配置选项 \(Options\) {#options}

选项可以通过设置的[Sass::Plugin\#options](http://sass-lang.com/documentation/Sass/Plugin/Configuration.html#options-instance_method)hash，具体设置在Rails中的`environment.rb`或者Rack中的`config.ru`的文件中：

```
Sass::Plugin.options[:style] = :compact
```

或者，如果你使用Merb，那么可以在`init.rb`文件中设置`Merb::Plugin.config[:sass]`hash ：

```
Merb::Plugin.config[:sass][:style] = :compact
```

或者通过传递一个选项 \(options\) hash 给[Sass::Engine\#initialize](http://sass-lang.com/documentation/Sass/Engine.html#initialize-instance_method)，所有相关的选项也可通过标记在`sass`和`scss`命令行可执行文件中使用。可用选项有：

| 选项 | 描述 |
| :--- | :--- |
| :style | 设置输出CSS的代码风格，可以查看输出的代码风格。 |
| :syntax |  |
| :property\_syntax |  |
| :cache |  |
| :read\_cache |  |
| :cache\_store |  |
| :never\_update |  |
| :always\_update |  |
| :always\_check |  |
| :poll |  |
| :full\_exception |  |
| :template\_location |  |
| :css\_location |  |
| :cache\_location |  |
| :unix\_newlines |  |
| :filename |  |
| :line |  |
| :load\_paths |  |
| :filesystem\_importer |  |
| :sourcemap |  |
| :line\_numbers |  |
| :trace\_selectors |  |
| :debug\_info |  |
| :custom |  |
| :quiet |  |



