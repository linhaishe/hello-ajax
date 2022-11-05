### 2. HTTP协议

HTTP协议（HyperText Transfer Protocol，超文本传输协议）是用于从WWW服务器传输超文本到本地浏览器的传输协议。协议详细规定了浏览器和万维网服务器之间互相通信的规则

请求和响应都分别包括==行、头、空行、体==

#### 1. 请求报文

```
//(请求)行;分别为 请求方式 请求参数 Http协议版本：POST /s?ie=utf-8 HTTP/1.1
POST /s?ie=utf-8 HTTP/1.1
Get /s?ie=utf-8 HTTP/1.1

//(请求)头：都是键值对的表现方式
Host: atguigu.com
Cookie: name=guigu
Content-type: application/x-www-form-urlencoded
User-Agent: Chrome 83

//空行
//这里有个空行

//(请求)体
username=admin&password=admin
//get请求中，请求体必须为空
//post请求中，请求体可以不为空
```

#### 2. 响应报文

```html
//(响应)行
HTTP/1.1 200 ok // http协议版本 响应状态码 响应状态字符串

//(响应)头
Content-type: text/html; charset=utf-8
Content-length: 2048
Content-encoding: gzip

//空行
//这里有个空行

//(响应)体
<html>
 	<body>一些文本内容</body>
</html>
```

<img src="http://tva1.sinaimg.cn/large/005NUwygly1h7u6y945wkj31d810eqkn.jpg" alt="image.png" style="zoom: 33%;" />
