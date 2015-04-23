LearningMaterials
## Linux
* [深入分析Linux内核源码](http://oss.org.cn/kernel-book/)
* [Linux 设备驱动 Edition 3](http://oss.org.cn/kernel-book/ldd3/)

## Android
+ [Mastering the Android Touch System](http://v.youku.com/v_show/id_XODQ1MjI2MDQ0.html?f=23088492)

## Others
+ [深入 Python :Dive Into Python 中文版](http://woodpecker.org.cn/diveintopython/toc/index.html)
+ [The Django Book](http://djangobook.py3k.cn/2.0/)


##git删除
+ 1、从你的资料库中清除文件

        git filter-branch --force --index-filter 'git rm --cached --ignore-unmatch projects/Moon.mp3' --prune-empty       --tag-name-filter cat -- --all
    
+ 2、 推送我们修改后的repo

        git push origin master --force

+ 3、清理和回收空间

        rm -rf .git/refs/original/

        git reflog expire --expire=now --all
    
        git gc --prune=now
    
        git gc --aggressive --prune=now
