Go官网下载：https://golang.google.cn/dl/

![image-20220330100618735](C:\Users\张少华\AppData\Roaming\Typora\typora-user-images\image-20220330100618735.png)

一直Next，安装位置自己决定

**重点**

1. ![image-20220330101127940](C:\Users\张少华\AppData\Roaming\Typora\typora-user-images\image-20220330101127940.png)

   一开始go会自动给我们设置一个环境变量，这里需要将其改为我们安装Go的根目录bin的路径

2. 在Path路径下添加Go的根目录bin的路径![image-20220330101430839](C:\Users\张少华\AppData\Roaming\Typora\typora-user-images\image-20220330101430839.png)

![image-20220330101532725](C:\Users\张少华\AppData\Roaming\Typora\typora-user-images\image-20220330101532725.png)

至此，在CMD中输入go会出现

![image-20220330101637037](C:\Users\张少华\AppData\Roaming\Typora\typora-user-images\image-20220330101637037.png)

到这，我们的环境已经配置好了。

### 使用vscode编写go项目

打开vscode，先安装vscode的go语言扩展
![image-20220330101931325](C:\Users\张少华\AppData\Roaming\Typora\typora-user-images\image-20220330101931325.png)

终端输入以下命令更改env设置安装

```go
go env -w GO111MODULE=on
go env -w GOPROXY=https://goproxy.cn,direct
```

这是更改为国内代理，不然即有可能出现

![在这里插入图片描述](https://img-blog.csdnimg.cn/4233c26fc2bb4da49740227ffcf918ef.png?x-oss-process=image/watermark,type_ZHJvaWRzYW5zZmFsbGJhY2s,shadow_50,text_Q1NETiBAc3l3ZGVidWc=,size_20,color_FFFFFF,t_70,g_se,x_16)

最后安装好之后就开始我们的HelloWord了！！！

在新建的hello.go写入

```go
package main

import "fmt"

func main() {
   fmt.Println("hello word!")
}
1234567
```

在终端cd到目录下使用以下命令运行

```go
go run hello.go
```

到这，我们已经完成了搬砖的第一步。

