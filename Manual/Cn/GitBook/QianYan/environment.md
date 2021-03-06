# 环境要求

- php版本大于等于5.6
- Swoole 拓展版本大于等于 1.9.11
- 仅支持 Linux,FreeBSD,MacOS 这三类操作系统

> 建议使用Ubuntu14/CentOS 6.5或更高版本操作系统

## 拓展安装教程

- 基础环境

    - Linux,FreeBSD 或MacOS 操作系统

    - php >= 5.6 (包含php-devel与php-common两个基础包)

    - gcc与autoconf

- 拓展编译

    - 拓展下载。
    
        到https://github.com/swoole/swoole-src/releases 下载最新的版本的swoole拓展源码，并解压到指定文件夹。

    - 打开终端（命令行），并切换到swoole拓展主目录写，分别执行：

        phpize

        ./configure

        make

        make && install

    - 以上步骤执行成功后，找到php.ini所在位置，编辑并加入extension=swoole.so,执行php -m可见swoole字样则说明拓展安装成功。

<script>
    var _hmt = _hmt || [];
    (function() {
        var hm = document.createElement("script");
        hm.src = "https://hm.baidu.com/hm.js?4c8d895ff3b25bddb6fa4185c8651cc3";
        var s = document.getElementsByTagName("script")[0];
        s.parentNode.insertBefore(hm, s);
    })();
</script>   
<script>
(function(){
    var bp = document.createElement('script');
    var curProtocol = window.location.protocol.split(':')[0];
    if (curProtocol === 'https') {
        bp.src = 'https://zz.bdstatic.com/linksubmit/push.js';        
    }
    else {
        bp.src = 'http://push.zhanzhang.baidu.com/push.js';
    }
    var s = document.getElementsByTagName("script")[0];
    s.parentNode.insertBefore(bp, s);
})();
</script>
