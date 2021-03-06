# PPT2PDF
开卷考试前把PPT转换成PDF的小工具

## 预计实现的功能
1. 把多个ppt或pptx合并并转换成一个pdf文件（调用MSOffice的API）。
2. 根据文件名和生成之后的pdf中的页码自动生成一个目录。
3. 可设置每页slide个数等常用参数。

## 必要的环境

1. Windows
2. .Net Framework 4.0及以上版本
3. Microsoft Office 2010及以上版本

## 可选参数

    -i, --input-files        Required. Input ppt or pptx files or directory

    -o, --output-file        (Default: output.pdf) Path of the generated PDF file.

    -v, --vertical-first     (Default: false) The order in which the handout should be printed.

    -h, --handout            (Default: SIX) A value that indicates how many slides to be printed in one page.

    -f, --frame-slides       (Default: false) Whether the slides to be exported should be bordered by a frame.

    -p, --only-output-ppt    (Default: false) Output merged PPT instead of PDF file.

    -d, --index              (Default: false) Generated a simple friendly lovely index page for you.

    --help                   Display this help screen.

    --version                Display version information.

## 运行时截图

### 命令行截图

![options](https://github.com/Dokyme/PPT2PDF/raw/master/assets/options.jpg)

![merging](https://github.com/Dokyme/PPT2PDF/raw/master/assets/merging.jpg)

![printing](https://github.com/Dokyme/PPT2PDF/raw/master/assets/printing.jpg)

### 输出质量截图

![quality](https://github.com/Dokyme/PPT2PDF/raw/master/assets/outputQuality.jpg)

## TODO

1. 自动生成索引。

## 目前可能存在的或已经发现的BUG

1. 生成文件的输出目录不正确（总是在当前登陆用户的目录的Documents目录）。
