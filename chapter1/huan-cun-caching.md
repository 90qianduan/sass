### 缓存 \(Caching\) {#t3-2}

Sass 自动缓存编译后的模板与[partials](http://sass-lang.com/documentation/file.SASS_REFERENCE.html#partials)，这样做能够显著提升重新编译的速度，尤其在处理由`@import`导入多个子文件的大型项目时。

单独使用 Sass，缓存内容保存在`.sass-cache`文件夹中。在 Rails 和 Merb 项目中缓存文件保存在`tmp/sass-cache`文件夹中（可通过[`:cache_location`](https://www.sass.hk/docs/)修改路径）。禁用缓存可将`:cache`设为`false`。



