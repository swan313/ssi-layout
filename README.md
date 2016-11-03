# ssi-layout
用ssi方式，实现静态页的动态变动
需要启动服务器环境 
配置httpd.conf文件，使.html扩展名的文件启用SSI
httpd.conf代码
    AddType text/html .html
    AddOutputFilter INCLUDES .html  

去掉注释 !!

例子：
<Directory "E:\wamp\www">
AddType text/html .ssi
Options Includes
AddOutputFilterByType INCLUDES;DEFLATE text/html
</Directory>
