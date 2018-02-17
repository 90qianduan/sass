在 Rails 3 之前的版本中启用 Sass，需要在`environment.rb`文件中添加一行代码：

```
config.gem "sass"
```

Rails 3 则需要在 Gemfile 中添加：

```
gem "sass"
```

在 Merb 中使用 Sass，需要在`config/dependencies.rb`中添加：

```
dependency "merb-haml"
```

在 Rack 中使用 Sass，需要在`config.ru`中添加：

```
require 'sass/plugin/rack'
use Sass::Plugin::Rack
```

样式文件与 views 不同，不包含任何动态内容，因此 CSS 只需要在 Sass 文件被修改后再编译生成。默认情况下`.sass`与`.scss`文件放置在`public/stylesheets/sass`中（可通过[:template\_location](http://sass-lang.com/documentation/file.SASS_REFERENCE.html#template_location-option)修改路径），编译生成的 CSS 文件放置在`public/stylesheets`

中。例如`public/stylesheets/sass/main.scss`编译生成`public/stylesheets/main.css`。

