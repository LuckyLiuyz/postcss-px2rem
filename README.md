# postcss-px2rem


### 移动端适配，将css 单位px --> rem

例如设计师给出640px的设计稿，写css样式的时候，就按照640px切图，单位px。
完工后，js或者css媒体查询，设定1rem的值。例如1rem == 40px。那么我们只
需要把css文件里面的px换算成rem就行。 而不需要在切图的过程中换算成rem。

### 下载项目

    git clone https://github.com/Happy-LYZ/postcss-px2rem.git

### 初始化，安装依赖

    npm install

### 执行

    node run build 

### TIPS

对css文件只匹配了小写的px，如果需要不转换px2rem，则可以在书写css的时候，大写PX，这样浏览器是支持的。

### 参考
	[postcss-pxtorem](https://github.com/Aralic/postcss-pxtorem)
   
### 预期功能

1. 生成的文件，从当前目录剥离出来，再根目录新建output文件夹，生成的文件输出到这个文件夹
2. 缓存优化，已编译输出，但再未修改过的文件不再编译。提升性能。
