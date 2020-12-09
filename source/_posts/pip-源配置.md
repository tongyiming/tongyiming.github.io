---
title: pip 源配置
---
# pip源
## pip 国内镜像
- 阿里云：https://mirrors.aliyun.com/pypi/simple/
- 中国科技大学：https://pypi.mirrors.ustc.edu.cn/simple/ 
- 豆瓣(douban) https://pypi.douban.com/simple/ 
- 清华大学 https://pypi.tuna.tsinghua.edu.cn/simple/ 

## 修改源方法
### 临时使用
可以在使用pip的时候在后面加上-i参数，指定pip源
``` 
eg: pip install scrapy -i https://pypi.tuna.tsinghua.edu.cn/simple
```
### 永久修改
修改 ~/.pip/pip.conf (没有就创建一个)， 内容如下：
```
[global]
trusted-host=pypi.tuna.tsinghua.edu.cn # 可以没有
index-url=https://pypi.tuna.tsinghua.edu.cn/simple/
```


