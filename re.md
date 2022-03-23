### nginx 配置说明

1、在nginx官网上下载安装包
2、把打包好的dist文件放到html文件夹下，
3、更改conf/nginx.conf 文件中的 server 

`
server{
    listen  8012;
    server_name  localhost;

    location / { 
        root html/dist;
        index index.html index.htm;
    }
}
`

### nginx 命令

# 启动 start nginx
# 关闭 nginx.exe -s stop
# 重启 nginx.exe -s reload
