# Social-Egine
1、参考模板编写好配置conf文件

2、运行 /opt/logstash/bin/logstash -f /path/to/conf/file -t 对配置文件进行检查，如果没有错误，就可以开始尝试导入

3、运行 
>$screen -S logstash
>
>$/opt/logstash/bin/logstash -f /path/to/conf/file 

使用快捷键 Ctrl+A+D 退出当前Scree

数据导入时间根据数据量大小来判断，平均，每小时200W条记录

4、查看导入情况
>$screen -ls 

>列出当前所有screen

>$screen -R 11694.logstash

>重新打开screen

5、最终导入进程不再产生数据，可以判断数据导入完毕。按Ctrl+C 终止logstash

6、同一时间，只能有一个Logstash在运行，注意时间分配