### jdbc

![1652340970129](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1652340970129.png)

![1652340951060](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1652340951060.png)

![1652341414587](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1652341414587.png)

![1652341472106](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1652341472106.png)

![1652341764580](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1652341764580.png)





# HTML-基本知识

![1650378581694](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650378581694.png)

![1650378600160](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650378600160.png)

![1650378641737](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650378641737.png)

![1650379848968](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650379848968.png)

![1650381568205](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650381568205.png)

![1650381238276](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650381238276.png)

![1650381535715](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650381535715.png)

![1650381752022](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650381752022.png)

无<h7></h7>

![1650382194784](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650382194784.png)

![1650382245562](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650382245562.png)

![1650382393975](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650382393975.png)

![1650382456545](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650382456545.png)

![1650382623192](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650382623192.png)

![1650382573656](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650382573656.png)

![1650382816705](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650382816705.png)

![1650382746859](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650382746859.png)

![1650460851038](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650460851038.png)

![1650460872597](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650460872597.png)

![1650461035730](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650461035730.png)

![1650460908482](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650460908482.png)

div ---层

![1650462325218](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650462325218.png)

![1650462882995](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650462882995.png)

![1650464284456](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650464284456.png)

![1650464327835](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650464327835.png)

![1650464805364](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650464805364.png)

![1650551855686](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1650551855686.png)

# js

# 4Servlet

## 4.1HTTP

### 4.1.1浏览器中的书写格式

​	服务器端资源需要通过浏览器进行，此时由浏览器将我们给出的请求解析为满足HTTP协议的格式并发出。我们发出的请求格式需要按照浏览器规定的格式来书写，在浏览器中书写格式如下：

HTTP:// IP地址/ 项目/资源 ？信息

当浏览器获取到信息以后，按照特定格式解析并发送即可。接收到服务器端给出的响应时，也按照HTTP协议进行解析获取到各个数据，最后按照特定格式展示给用户  

### 4.1.2HTTP协议的特点

1.支持客户/服务器模式

2.简单快速：客户向服务请求服务时，只需要传送请求方法和路径。请求方法常用的有GET、POST。每种方法规定了客户和服务器联系的类型不同。由于HTTP协议简单，使得HTTP服务器规模小，因而通信速度很快。

3、灵活：HTTP允许传输任意类型的数据对象。传输的类型由Content-Type加以标记。

4.无连接：无连接是表示每次连接只处理一个请求。服务器处理完客户的请求，并收到客户的应答后，即断开连接。采用这种方式可以节省传输时间。

HTTP1.1版本后支持持续连接。通过这种连接就有可能在建立一个TCP连接后，发送请求并得到回应，然后发送更多的请求并得到更多的回应。通过把建立和释放TCP连接的开销分摊到多个请求上，则对于每个请求而言，由于TCP而造成的相对开销被大大降低。而且，还可以发送流水线请求，也就是说在发送请求1之后的回应到来之前就可以发送请求2.也可以认为，一次连接发送多个请求，由客户机确认是否关闭连接，而服务器会认为这些请求分别来自不同的客户端。

5.无状态：HTTP协议是无状态协议。无状态是指协议对于事务处理没有记忆能力。缺少状态意味着如果后续处理需要面前的信息，则它必须重传，这样可能导致每次连接传送的数据量增大。另一方面，在服务器不需要先前信息时它的应答就较快。

### 4.1.3HTTP之URL

​	HTTP（超文本传输协议）是一个基于请求与响应模式的，应用层的协议，常基于TCP的连接方式，绝大多数的web开发，都是构建的HTTP写于之上的web应用。

​	HTTP URL（URL是一种特殊类型的URI，包含了用于查找某个资源的足够的信息）的格式如下：

http://hoat[:port]/[abs_path]

htttp://IP(主机名/域名):端口/访问的资源路径

http表示要通过HTTP协议来定位网路资源

host表示合法的Internet主机域名或者IP地址

port指定一个端口号，为空则使用缺省端口80

abs_path指定请求资源的URI；如果URL中没有给出abs_path，那么当他作为请求URI时，必须以"/"的形式给出，通常这个工作浏览器自动帮我们完成。

### 4.1.4HTTP请求

HTTP请求由三部分组成，分别是：请求行--第一行，请求头--键值对，请求正文

通过浏览器，F12 -->Network查看

#### 1.Get请求没有请求体

![1653114717412](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653114717412.png)

#### 2.post请求

![1653114806894](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653114806894.png)

#### 格式

请求行

请求头1

请求头2

……

请求空行

请求体

请求行以一个方法符号开头，以空格分开，后面跟着请求的URI的协议的版本。

格式如下：Method Resquest-URI HTTP-Version CRLF

​		method表示请求方法；

​		Request-URI是一个统一资源标识符

​		HTTP-Version表示请求的HTTP协议版本

​		CRLF表示回车和换行

### 4.1.5HTTP响应

在接收和解释请求消息后，服务器返回一个HTTP响应消息。HTTP响应也是由三个部分组成，分别是：状态行、消息报头、响应正文

![1653115606139](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653115606139.png)

![1653115627078](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653115627078.png)

### 4.1.6消息头

![1653118665100](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653118665100.png)

#### 4.1.6.1请求头

![1653118697489](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653118697489.png)

#### 4.1.6.2响应头

![1653119124002](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653119124002.png)

## 4.2.Tomcat服务器

### 4.2.1.什么是Tomcat

![1653120081490](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653120081490.png)

### 4.2.2.Tomcat目录结构

![1653121003868](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653121003868.png)

### 4.2.3.IDEA配置Tomcat

![1653121118727](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653121118727.png)

![1653121138882](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653121138882.png)

![1653121154369](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653121154369.png)

![1653121191776](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653121191776.png)

## 4.3.Servlet的实现

![1653121324452](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653121324452.png)

### 4.3.1创建Web项目

![1653121525925](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653121525925.png)

![1653121562568](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653121562568.png)

![1653121592939](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653121592939.png)

![1653121610540](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653121610540.png)

### 4.3.2.Servlet的实现

#### 4.3.2.1.新建类

![1653121839018](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653121839018.png)

![1653121872621](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653121872621.png)

#### 4.3.2.2.实现Servlet规范

​	实现Sevlet规范，即继承HttpServlet类，并到如响应

的包，该类中已经完成的通信规则，我们只需要进行业务实现即可

```java
`package com.XXX.servlet;`

`import javax.setvlet.http.HttpServlet;`

public class servlet01 extends HttpServlet{
    
}
```

#### 4.3.2.3重写servlet方法

满足Servlet规范的只是让我们的类能够满足接收请求的要求，接收到请求后需要对请求进行分析，以及进行业务逻辑出里，计算出结果，则需要添加代码，在规范中有叫servlet的方法，专门用来做请求处理的操作。业务代码则可以写在该方法中

```java
package com.xxx.servlet;
import javax.servlet.ServletException;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;
public class Servlet01 extends HttpServlet{
    @Override
    protected void service(HttpServletRequest req, HttpservletResponse resp) throws ServletException,IOException{
        System.out.println("Hello World!");
        resp.getWriter().write("Hello World");
    }
} 
```

#### 4.3.2.4设置注解

在完成好一切代码的编写后，还需要向服务器说明，特定请求对应特定资源。

在开发servlet项目，使用@WebServlet将一个继承于javax.servlet.http.HttpServlet的类定义为Servlet组件。

在Servlet3.0中，可以使用@WebServlet注解将一个继承于javax.servlet.http.HttpServlet的类标注为可以处理用户请求的Servlet。

```java
package com.xxx.servlet;
import javax.servlet.ServletException;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;
@WebServlet("/ser01")
public class Servlet01 extends HttpServlet{
    @Override
    protected void service(HttpServletRequest req, HttpservletResponse resp) throws ServletException,IOException{
        System.out.println("Hello World!");
        //通过流输出数据到浏览器
        resp.getWriter().write("Hello World");
    }
} 
```

用注解配置Servlet

#### 4.3.2.5.Servlet的实现方式

1.继承HttpServlet类----最常用一般都用这个

2.继承GenericSevlet类---实现方法较少

3.实现Servlet接口

### 4.3.3.Servlet的生命周期

​	Servlet没有main()方法，不能独立运行，他的运行完全由Servlet引擎来控制和调度。所谓的生命周期，指的是servlet容器何时创建servlet实例、何时调用其方法进行请求的处理、核实并销毁其实例的整个过程。

##### 	实例和初始化时机

​	当请求到达容器时，容器查找该servlet对象是否存在，如果不存在，则会创建实例并进行初始化。

##### 	就绪/调用/服务阶段

​	有请求到达容器，容器调用servlet对象的service()方法，处理请求的方法在整个生命周期中可以被多次调用；HttpServlet的service()方法，会依据请求方式来调用doGet()或doPost()方法。但是，这两个do方法默认情况下会抛出异常，需要子类去override。

##### 	销毁时机

​	当容器关闭时（应用程序停止时），会将程序中的Servlet实例进行销毁。

上述的生命周期可以通过Servlet中的生命周期方法来观察。在Servlet中有三个生命周期方法，不由用户手动调用，而是在特定的时机有容器自动调用，观察三个生命周期方法即可观察到Servlet的生命周期。

init方法，在Servlet实例创建之后执行（证明该Servlet有实例创建了）--初始化方法，服务器自动调用，如果不存在Servlet实例就创建并初始化--只调用一次

```java
public void init(ServletConfig config) throws ServletException{
    System.out.println("实例创建了……");
}
```

service方法，每次有请求到达某个Servlet方法时执行，用来处理请求（证明servlet进行服务了）

```java
protected void service(HttpServletRequest req, HttpservletResponse resp) throws ServletException,IOException{
        Syetem.out.println("服务调用了……");
    }

```

destroy方法，Servlet实例销毁时执行（证明Servlet的实例被销毁了）--只能调用一次

```java
public void destroy(){
    System.out.println("实例销毁了……");
}
```

![1653195928710](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653195928710.png)

![1653196105730](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653196105730.png)

### 4.3.4HttpServletRequest对象

![1653196304894](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653196304894.png)

## 接受请求

### 常用方法

​	1.方法

​	![1653196587792](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653196587792.png)

2.示例

```java
//获取客户端请求的完整URL（从http开始，到？面前结束）
String ur1 = request.getRequestURL().toString();
System.out.println("获取客户端请求的部分URL："+queryString);

//获取客户端请求的部分URL（从项目站点名开始，到？前面结束）
String uri = request.getRequestURI();
System.out.println("获取客户端请求的部分URL："+queryString);
//获取请求行中的参数部分即参数字符串
String queryString = request.getQueryString();
System.out.println("获取请求行中的参数部分："+queryString);
//获取客户端的请求方式
String method = request.getMethod();
System.out.println("获取客户端的请求方式：" +method);
//获取HTTP的版本号
String protocol = request.getProtocol();
System.out.println("获取HTTP版本号"+protocol);
//获取webapp的名字
String webapp = request.getContextPath();
System.out.println("获取webapp的名字" + webapp);
```

#### 获取请求参数

1.方法

![1653198827194](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653198827194.png)

2.示例

```java
//获取指定名称的参数，返回字符串（重点！！！）
String uname = request.getParameter("uname");
System.out.println("uname的参数："+uname);
//获取指定名称参数的所有参数值，返回数组
String[] hobbys = request.getParameterValues("hobby");
System.out.println("获取指定名称参数的所有参数值："+Arrays.toString(hobbys));
```

### 请求乱码问题

​	![1653377014378](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653377014378.png)

##### 方式一：

```java
request.setCharacterEncoding("UTF-8")
```

这种方式只针对POST有效（必须在接受所有数据之前设定）

##### 方式二：

```java
new String(request.getParameter(name).getBytes("ISO-8859-1"),"UTF-8");
```

借助String对象的方法，该方式对任何请求有效，是通用的。

**Tmcat8起，以后的GET方式请求是不会出现乱码的**

### 请求转发

​	请求转发，是一种服务器的行为，当客户端请求到达后，服务器进行转发，此时会将请求对象进行保存，地址栏中的URL地址不会改变，得到响应后，服务器再将响应发送给客户端，从始至终只有一个请求发出。

实现方式如下，达到多个资源协同响应的效果。

```java
request.getRequestDispatcher(url).forward(request,response);
```

特点：

​	1.服务端行为

​	2.地址栏不会改变 

​	3.只有一个请求

​	4.request数据可以共享

### request作用域

通过该对象可以在一个请求中传递数据，作用范围，在一次请求中有效，即服务器跳转有效

```java
//设置与对象内容
request.setAttribute(String name,Object value);
//获取对象内容
request.getAttribute(String name);
//删除需对象内容
request.removeAttribute(String name);
```

![1653382578128](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653382578128.png)

![1653382725150](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653382725150.png)

![1653383021275](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653383021275.png)

![1653382969857](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653382969857.png)

request域对象中的数据在一次请求中有效，则经过请求转发，request域中的数据依然存在，则在请求转发的过程中可以通过request来传输/共享数据。

## HttpServletResponse对象

![1653383357129](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653383357129.png)

### 响应数据

接收到客户端请求后，可以通过HttpServletResponse对象直接响应，响应时需要获取输出流。有两种形式：

​	**getWriter() 获取字符流（只能响应回字符）**

​	**getOutputStream() 获取字节流（能响应一切数据）**

响应回的数据到客户端被浏览器解析，

注意：两者不能同时使用

```java
//字符输出流
PrintWriter writer = response.getWriter();
writer.Write("Hello");
writer.write("<h2>Hello</h2>");
```

```java
//字符输出流
PrintWriter writer = response.getOutputStream();
writer.Write("Hello".getBytes());
writer.write("<h2>Hello</h2>".getBytes());
```

### 响应乱码

在响应中，如果我们响应的内容中含有中文，则有可能出现乱码。这是因为服务器响应的数据也会经过网络传输，服务器端有一种编码方式，在客户端也存在一种编码方式，当两端使用的编码方式不同时则会出现乱码。

**getWriter()的字符乱码**

​	对于getWriter() 获取到的字符流，响应中文必定出乱码，由于服务器端在进行编码时默认会使用ISO-8859-1格式的编码，改编码方式并不支持中。

​	要解决该种乱码只能在服务算告知服务器使用一种能够支持中文的编码格式，比如我们通常用的“UTF-8”.

```java
response.setCharacterEncoding("UTF-8");
```

此时还只完成了一半的工作，还要保证数据正确显示，还需要**指定客户端**的解码方式。

```java
response.serHeader("content-type","text/html;charset=UTF-8");
```

l两端指定编码后，乱码就解决了。一句话：保证发送端和接收端的编码一致

```java
//设置服务端的编码
response.serCharacterEncoding("UTF-8");
//设置客户端的响应类型及编码
response.setHeader("content-type","text/html;charset=UTF-8");
//得到字符输出流
PrintWriter writer = response.getWriter();
writer.write("<h2>你好</h2>");
```

以上两端编码的指定也可以通过一句话来实现： 

```java
response.setContenType("text/html;charset=UTF-8");
```

**getOutputStream()字节乱码**

​	对于getOutputStream()方式获取到的字节流，响应中文时，由于本身就是传输的字节，所以此时可能出现乱码，也可能正确显示。当服务器端给的字节恰好和客户端使用的编码方式一致时则文本正确显示，否则出现乱码。无论如何我们都应该准确掌握服务器和客户端使用的是另一种编码格式，以确保数据正确显示。

​	**指定客户端和服务器使用的编码方式一致。**

```java
response.setHeader("content-type","text/html;charset=UTF-8");

//设置客户端的编码及响应类型
ServletOutputputStream out = response.getOutputStream();
response.setHeader("content-type","text/html;charset=UTF-8");
out.write("<h2>你好<h2>".getBytes("UTF-8"));
```

### 重定向

​	重定向是一种服务器指导，客户端的行为。客户端发出第一个请求，被服务器接受处理后，服务器会进行响应，在响应的同时，服务器会给客户端一个新的地址（下次请求的地址response.sendRedirect(url);）,当客户端接收到响应后，会立刻、马上、自动根据服务器给的新地址发起第二个请求，服务器接收请求并作出响应，重定向完成。

​	从描述中可以看出重定向当中有两个请求存在，并且属于客户端行为。

```java
//重定向跳转到index.jsp
response.sendRedirect("index.jsp");
```

​	通过观察浏览器我们会发现第一次请求获得的响应码为302，并且含有一个location头信息。并且地址栏最终卡到的地址是和第一次请求的地址不同的，地址栏已经发生变化。

![1653923136726](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653923136726.png)

requset对象和response对象不共享

### 请求转发和重定向的区别

​	请求转发和重定向比较：

![1653924462505](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653924462505.png)

两者都可进行跳转，根据实际需求选取即可。

## Cookie对象

![1653978571347](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653978571347.png)

### Cookie的创建和发送

​	通过new Cookie("key","value");来创建一个Cookie对象，要想将Cookie随响应发送到客户端，需要先添加到response对象中，response.addCookie(cookie);此时该cookie对象则随着响应发送到客户端。在浏览器上可以看见。

```java
//创建Cookie对象
Cookie cookie = new Cookie("uname","zhangsan");
//发送Cookie对象
response.addCookie(cookie);
```

![1653979068639](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1653979068639.png)

### Cookie的获取

​	在服务器端只提供了一个getCookies()的方法来获取客户端传回的所有cookie组成的一个数组，如果需要获取单个cookie则需要通过遍历，getName()获取Cookie的名称，getValue()获取Cookie的值。

```java
//获取Cookie数组
Cookie[] cookies = request.getCookies();
//判断数组是否为空
if(cookies != null && cookies.length>0){
	//遍历cookies数组
	for(Cookie cookie : cookies){
		System.out.println(cookie.getName());
		System.out.println(cookie.getValue());
	}
}
```

### Cookie设置到期时间

​	除了Cookie的名称和内容外，我们还需要关心一个信息，到期时间，到期时间用来指定该cookie何时失效。默认为当前浏览器关闭即失效。我们可以通过手动设定cookie的有效时间（通过到期时间计算），通过setMaxAge(int time);方法设定cookie的最大有效时间，以秒为单位。

**到期时间的取值**

​	负整数

​	若为负数，表示不存储cookie。

​	cookie的maxAge属性的默认值就是-1，表示只在浏览器内存中存活，一旦关闭浏览器窗口，那么cookie就会消失。

​	正整数

​	若大于0的整数，表示存储的秒数。

​	表示cookie对象可存活指定的秒数。当生命大于0时，浏览器会把Cookie保存到硬盘上，就算关闭浏览器，就算重启客户端电脑，cookie也会存活相应的时间。

​	零

​	若为0，表示删除该cookie。

​	cookie生命等于0是一个特殊的值，他表示cookie被作废！也就是说，如果原来浏览器已经保存了这个Cookie，那么可以通过Cookie的setMaxAge(0)来删除这个cookie。无论是在浏览器内存中，还是在客户端硬盘上都会删除这个Cookie。

```java
//到期时间为负整数：cookie存在浏览器中，关闭浏览器失效
Cookie cookie1 = new Cookie("uname1","zhangsan");
cookie1.setMaxAge(-1);
response.addCookie(cookie1);
//到期时间为正整数：cookie存活指定秒数
Cookie cookie2 = new Cookie("uname2","lisi");
cookie2.serMaxAge(30);
response.addCookie(cookie2);
//到期时间为零：删除指定cookie
Cookie cookie3 = new Cookie("uname3","java");
cookie3.setMaxAge(0);
response.addCookie(cookie3);
```

### Cookie的注意点

1.Cookie保存在当前浏览器中。

​	在一般的站点中常常有记住用户名这样一个操作，该操作只是将信息保存在本机上，换电脑以后这些信息就无效了。而且cookie还不能跨浏览器。

2.Cookie存中文问题

​	Cookie中不能出现中文，如果有中文则通过URLEncoder.encode()来进行编码，获取时通过URLDecoder.decode()来进行解码。

```java
String name = "姓名";
String value = "张三";

name = URLEncoder.encode(name);
value = URLEncoder.encode(value);

Cookie cookie = new Cookie(name,value);
response,addCookie(cookie);

URLDecoder.decode(cookie.getName);
URLDecoder.decode(cookie.getValue);
```

3.同名Cookie问题

​	如果服务器端发送重复的Cookie那么会覆盖原有的Cookie。

4.浏览器存放Cookie的数量

​	不同的浏览器对Cookie也有限定，Cookie的存储是有上限的。Cookie是存储在客户端（浏览器）的，而且一般是由服务器端创建和设定。后期结合Session来实现回话跟踪。

### Cookie的路径

​	Cookie的setPath设置cookie的路径，这个路径直接决定服务器的请求是否会从浏览器中加载某些cookie。

**情景一：**当前服务器下任何项目的任意资源都可获取Cookie对象

```java
/*当前项目路径为：s01*/
Cookie cookie = new Cookie("xxx","xxx");
//设置路径为"/",表示在当前服务器下任何项目都可以访问到Cookie对象
cookie.setPath("/");
response.addCookie(cookie);
```

**情景二：**当前项目下的资源可获取Cookie对象（默认不设置Cookie的path）

```java
//当前项目路径为：s01
Cookie cookie = new Cookie("xxx","xxx");
//设置路径为"/s01",表示在当前项目下的任何项目都可访问到Cookie对象
cookie.setPath("/s01");
response.addCookie(cookie);
```

**情景三：**指定项目下的资源可获取Cookie对象

```java
//当前项目路径：s01
Cookie cookie = new Cookie("xx","xx");
//设置路径为"/s02"，表示在s02项目下才可以访问Cookie对象
cookie.setPath("/s02");
response.addCookie(cookie);
```

**情景四：**指定目录下的资源可获取Cookie对象

```java
//当前项目路径为：s91
Cookie cookie = new Cookie("xx","xx");
//设置路径为"/s01/cook",表示在s02/cook目录下才可以访问到Cookie对象
cookie.setPath("/s01/cook");
response.addCookie(cookie);
```

​	如果我们设置path，如果当前访问的路径包含了cookie的路径（当前访问路劲在cookie路径基础上要比cookie的范围小）cookie就会加载到request对象之中。

​	cookie的路径值的是可以访问该cookie的顶层目录，该路径的子路径也可以访问该cookie。

​	**总结：当访问的路径包含了cookie的路径是，则该请求将带上cookie；如果访问路径不包含cookie路径，则该请求不会携带该cookie。**

## HttpSession对象

​	**HttpSession**对象是javax.servlet.http.HttpSession的实例，该接口并不像HttpServletRequest或HttpServletResponse还存在一个父接口，该接口只是一个纯粹的接口。这因为session本身就属于HTTP协议的范畴。

​	对于服务器而言，每一个连接到它的客户端都是一个session，servlet容器使用此接口创建HTTP客户端和HTTP服务器之间的会话。会话将保留指定的时间段，跨多个连接或来自用户的页面请求。一个会话通常对应于一个用户，该用户可能多次访问一个站点。可以通过此接口查看和操作有关某个会话的信息，比如会话标识符、创建时间和最后一次访问时间。在整个session中，最重要的就是属性的操作。

​	session无论客户端还是服务器端都可以感知到，若重新打开一个新的浏览器，则无法取得之前设置的session，因为每一个session只保存在当前的浏览器当中，并在相关的页面取得。

​	Session的作用就是为了标识一次会话，或者说确认一个用户；并且在一次会话（一个用户的多次请求）期间共享数据。我们可以通过request.getSession()方法，来获取当前会话的session对象。

```java
//如果session对象存在，则获取，如果session对象不存在，则创建
HttpSession session = request.getSession();
```

获取session的会话标识符  getId()

获取session的创建时间      getCreationTime()

获取最后一次访问时间        getLastAccessedTime()

判断是否是新的session对象  isNew()

### 标识符JSESSIONID

​	Session既然是为了标识一次会话，那么此次会话就应该有一个唯一的标志，这个标志就是sessionId。

​	每当一次请求到达服务器，如果开启了会话（访问了session），服务器第一步会查看是否从客户端回传一个名为JSESSIONID的cookie，如果没有则认为这是一次新的会话，会创建一个新的session对象，并用唯一的sessionId为此次会话做一个标志。如果有JSESSIONID这个cookie回传，服务器则会根据JSESSIONED这个值去查看是否含有id为JSESSION 值得session对象，如果没有则认为是一个新的会话，重新创建一个新的session对象，并标志此次会话；如果找到了相应得session对象，则认为是之前标志过得一次会话，返回该session对象，数据达到共享。

​	这里提到一个叫做JSESSIONID得cookie，这是一个比较特殊得cookie，当用户请求服务器时，如果访问了session，则服务器会创建一个名为JSESSIONID，值为获取到的session（无论是获取到的还是新创建的）的sessionId的cookie对象，并添加到response对象中，响应给客户端，有效时间为关闭浏览器。

​	所以Session的底层依赖Cookie来实现。

### session域对象

Session用来表示一次会话，在一次会话中数据是可以共享的，这时session作为域对象存在，可以通过setAttribute(name,value)方法向域对象中添加数据，通过getAttribute(name)从域对象中获取数据，通过removeAttribute(name)从域对象中移除数据。

```java
//获取session对象
HttpSession session = request.getSession();
//设置session域对象
session.setAttribute("uname","admin");
//获取指定名称的session域对象
String uname = (String) request.getSession().getAttribute("uname");
//移除指定名称的session域对象
session.removeAttribute("uname");
```

​	数据存储在session域对象中，当session对象不存在了，或者是两个不同的session对象时，数据也就不能共享了。这就不得不谈到session的生命周期。

### session对象的销毁

#### 默认时间到期

​	当客户端第一次请求servlet并且操作session时，session对象生成，Tomcat中session默认的存活时间为30min，即你不操作界面的时间，一旦有操作，session会重新计时。

​	那么session的默认时间可以改吗？肯定可以的。

​	可以在Tomcat中的conf目录下的web.xml文件中进行修改。

```html
<!-- session 默认的最大不活动时间。单位：分钟。-->
<session-config>
	<session-timeout>30</session-timeout>
</session-config>
```

#### 自己设定到期时间

​	当然除了以上的修改方式外，我们也可以在程序中设定session的生命周期，通过session.setMaxInactiveInterval(int)来设定session的最大不活动时间，单位为秒。

```java
//获取session对象
HttpSession session = request.getSession();
//设置session的最大不活动时间
session.setMaxInactiveInterval(15);
```

当然我们也可以通过getMaxInactiveInterval()方法来查看当前Session对象的最大不活动时间。

```java
//获取session的最大不活动时间
int time = session.getMaxInactiveInterval();
```

#### 立刻失效

​	或者我们也可以通过session.invalidate()方法让session立刻失效

```java
//销毁session对象
session.invalidate();
```

**关闭浏览器session失效**：session底层依赖cookie实现，并且该cookie的有效时间为关闭浏览器，从而session在浏览器关闭时也相当于失效了（因为没有JSESSION再与之对应）。

**关闭服务器**：当关闭服务器时，session销毁。Session失效则意味着此次会话结束，数据共享结束。

## ServletContext对象

​	每一个web应用都有且仅有一个ServletContext对象，又称Application对象，从名称中可知，该对象是与应用程序相关的。在WEB容器启动的时候，会为每一个WEB应用程序创建一个对应的Servletcontext对象。

​	该对象有两大作用，第一：作为域对象用来共享数据，此时数据在整个应用程序中共享；第二：该对象中保存了当前应用程序相关信息。例如可以通过getServerInfo()方法获取当前服务器信息，getRealPath(String path)获取资源的真实路径等。

### ServletContext对象的获取

​	获取ServletContext对象的途径有很多。比如：

1.通过request对象获取

```java
ServletContext servletContext = request.getServletContext();
```

2.通过session对象获取

```java
ServletContext servletContext = request.getSession().getServletContext();
```

3.通过servletConfig对象获取，在Servlet标准中提供了Servlet Config方法

```java
ServletConfig servletConfig = getServletConfig();
ServletContext servletContext = servletConfig.getServletContext();
```

4.直接获取

```java
ServletContext servletContext = getServletContext();//只有在servlet中才能用
```

### 常用方法

1.获取当前服务器的版本信息

```java
String servletInfo = request.getServletContext().getServerInfo();
```

2.获取项目的真实路径

```java
String realPath = request.getServletContext().getRealPath("/");
```

### ServletContext域对象

​	ServletContext也可当做域对象来使用，通过向ServletContext中存取数据，可以使得整个应用程序共享某些数据。当然不建议存放过多数据，因为ServletContext中的数据一旦存储进去没有手动移除将会一直保存。

```java
//获取ServletContext对象
ServletContext servletContext = request.getServletContext();
//设置域对象
servletContext.setAttribute("name","zhangsan");
//获取域对象
String name = (String)servletContext.getAttribute("name");
//移除域对象
servletContext.removeAttribute("name");
```

**Servlet的三大域对象**

1.request域对象

​	在一次请求中有效。请求转发有效，重定向失效。

2.session域对象

​	在一次会话中有效。请求转发和重定向都有效，session销毁后失效。

3.servletContext域对象

​	在整个应用程序中有效。服务器关闭后失效。

## 文件上传和下载

### 文件上传

​	文件上传涉及到前台页面的编写和后台服务器端代码的编写，前台发送文件，后台接收并保存文件，这才是一个完整的文件上传。

### 前台页面

​	在做文件上传的时候，会有一个上传文件的界面，首先我们需要一个表单，并且表单的请求方式为POST;其次我们的form表单的enctype必须设为"multipart/form-data",即**enctype="multipart/form-data"**,意思是设置表单的类型为文件上传表单。默认情况下这个表单类型是"application/x-www-form-urlencoded",不能用于文件上传。只有使用了multipart/form-data才能完整地传递文件数据。

```html
<!--
	文件上传表单
		1.表单提交类型 method="post"
		2.表单类型 enctype="multipart/form-data"
		3.表单元素类型 文件域设置name属性值
-->
<form method="post" action="uploadServlet" enctype="multipart/form-data">
    姓名:<input type="text" name="uname"> <br>
    文件:<input type="file" name="myfile"> <br>
    <button type="submit">
        提交
    </button>
</form>
```

![1654510386796](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1654510386796.png)

### 后台实现

​	使用注解**@MultipartConfig**将一个Servlet标识为支持文件上传。Servlet将multipart/form-data的POST请求封装成Part，通过Part对上传的文件进行操作。

```java
@WebServlet("/uploadServlet")
@MultipartConfig//如果是文件上传表单，一定要加这个注解
public class UploadServlet extends HttpServlet{
    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response)throws ServletException,IOException{
        //设置请求的编码格式
        request.serCharacterEncoding("UTF-8");
        //获取普通表单项（文本框）
        String uname = request.getParameter("uname");//"uname"代表的是文本框的name属性值
        //通过getPart(name)方法获取Part对象（name代表的是页面中file文件域的name属性值）
        Part part = request.getPart("myfile");
        //通过Part对象，获取上传的文件名
        String fileName = part.getSubmittedFileName();
        //获取上传文件需要存放的路径（得到项目存放的真实路径）
        String realPath = request.getServletContext().getRealPath("/");
        //将文件上传到指定位置
        part.write(realPath+fileName);
    }
}
```

 

### 文件下载

​	文件下载，即将服务器上的资源下载（拷贝）到本地，我们可以通过两种方式下载。第一种是通过超链接本身的特性来下载；第二种是通过代码下载。

**超链接下载**

​	当我们在HTML或JSP页面中使用a标签时，意愿是希望能够进行跳转，但当超链接遇到浏览器不识别的资源时会自动下载；当遇见浏览器能够直接显示的资源，浏览器就会默认显示出来，比如txt、png、jpg等。当然我们也可以通过download属性规定浏览器进行下载。但有些浏览器并不支持。

默认下载

```html
<!-- 当超链接遇到浏览器不识别的资源时，会自动下载-->
<a href="test.zip">超链接下载</a>
```

指定download属性下载

```html
<!-- 当超链接遇到浏览器识别的资源时，默认不会下载。通过download属性可进行下载-->
<a href="test.txt" download>超链接下载</a>
```

download属性可以不写任何信息，会自动使用默认文件名。如果设置了download属性的值，则使用设置的值作为文件名。当用户打开浏览器点击连接时就会直接下载文件。

![1654529587203](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1654529587203.png)

**后台实现下载**

**实现步骤**：

1.需要通过response.setContentType方法设置Content-type头字段的值，为浏览器无法使用某种方式或激活某个程序来处理的MIME类型，例如“application/octet-stream”或”application/x-madownload“等。

2.需要通过response.setHeader方法设置Content-Disposition头的值为“attachment;filename=文件名”

3.读取下载文件，调用response.getOutputStream方法向客户端写入附件内容。

```java
public class DownloadServlet extends HttpServlet{
    protected void service(HttpServletRequest request,HttpServletResponse response)throws ServletException,IOException{
        //设置请求的编码
        request.setCharacterEncoding("UTF-8");
        //获取文件下载路径
        String path = getServletContext().getRealPath("/");
        //获取下载的文件名
        String name = request.getParameter("fileName");
        //通过路径的得到file对象
        File file = new File(Path + name);
        //判断file对象是否存在，且是否是一个标准文件
        if(file.exists() && file.isFile()){
            //设置响应类型（浏览器无法使用某种方式或激活某个程序来处理的类型）
            response.setContentType("application/x-msdownload");
            //设置头信息
            response.setHeader("Content-Disposition","attachment;filename=" + name);
            //得到输入流
            InputStream is = new FileInputStream(file);
            //得到输出流
            ServletOutputStream os = response.getOutputStream();
            //定义bytes数组
            byte[] car = new byte[1024];
            //定义长度
            int len = 0;
            //循环输出
            while((len = is.read(car)) != -1){
                os.write(car,0,len);
            }
            //关闭流 释放资源
            is.close();
            os.close();
        }else{
            System.out.println("文件不存在");
        }
    }
}
```

![1654610949948](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1654610949948.png)

![1654611021850](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1654611021850.png)

![1654611286033](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1654611286033.png)

![1654611361171](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1654611361171.png)

# JSP和JSTL

## JSP的基础语法

### 简介

​	Jsp：Java Servler Page SUN公司提供的动态网页编程技术，是Java Web 服务端的动态资源。

​	它相比 html 而言，html 只能为用户提供静态数据，而Jsp技术允许在页面中嵌套 Java 代码，为用户提供动态数据。

​	相比 servlet ，servlet 很难对数据进行排版，而 Jsp 除了可以用 Java 代码产生动态数据的同时，也很容易对数据进行排版。

​	不管是 JSP 还是 Servlet，虽然都可以用于开发动态web资源。但由于这 2 门技术各自的特点，在长期的软件实践中，人们逐渐把 servlet 作为 web 应用中的控制组件来使用，而把 JSP 技术作为数据显示模板来使用。

​	其实 JSP 就是一个 Servlet，当我们第一次访问 JSP 的时候，Jsp 引擎都会将Jsp 翻译成一个 Servlet，这个文件存放在tomcat（源码目录）中的 work 目录中。

![1655174055276](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1655174055276.png)

![1655174889452](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1655174889452.png)

![1655174914328](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1655174914328.png)

![1655174937262](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1655174937262.png)

### 注释

在Jsp 中支持两种注释的语法操作：

​	一种是显示注释，这种注释是允许客户端看见的；另一种是隐式注释，此种注释是客户端无法看见的

​	1.显示注释语法：从HTML 风格继承而来

​	2.隐式注释语法：从Java 风格注释；jsp 自己的注释



JSP的三种注释方式：

```
1） // 单行注释 /* 多行注释 */
2) <!-- HTML 风格注释 -->  可以在浏览器查看源码时看见 是显示注释
3) <%-- JSP --%>--隐式注释
```

### Scriptlet

​    在JSP 中最重要的部分就是 Scriptle（脚本小程序），所有嵌入在 HTML 代码中的 Java 程序。

​	在 JSP 中一共有三种 Scriptlet 代码：都必须使用 Scriptlet 标记出来

第一种：<%     %>: Java脚本段，可以定义局部变量，编写语句

第二种：<%!    %>:声明，可以定义全局（成员）变量、方法、类

第三种：<%=   %>:表达式，数据一个变量或具体内容

​	通过观察解析为 Java 文件的 jsp 代码理解三种小脚本

```jsp
<%@ page language="java" contenType="text/html; charset=UTF-8" pageEncoding="UTF-8"%>
<!DOCTYPE>
<html>
    <head>
        <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
        <title>Scriptlet</title>
    </head>
    <body>
        <%
        	String str = "Hello Jsp"
        	System.out.println(str);
        	response.getWriter().Write(str);
        
        %>
        <%!
    		String memberStr = "a member 			 string";
    	%>
    </body>
</html>
```

###  JSP 的指令标签

​	使用包含 操作，可以将一些重复的代码包含进来继续使用，从正常的页面组成来看，有时可能会分为几个区域。而其中的一些区域可能是一直不需要改变的，改变的就是其中的一个具体内容的区域。现在有两种 方法可以实现上述功能。

​	方法一：在每一个 JSP 页面中都包含工具栏、头部信息、尾部信息、具体内容

​	方法二：将将工具栏、头部信息都分成各个独立的文件，使用的时候直接导入

​	很明显，第二种方法比第一种更好，第一种会存在很多重复的代码，并且修改很不方便，在JSP中如果要想实现包含的操作，有两种做法：**静态包含、动态包含**，静态包含使用include指令即可，动态包含则需要使用include动作标签。

#### include 静态包含

```jsp
<%@ include file ="要包含的文件路径" %> <!-- 相对路径 -->
```

例如：

```jsp
<%@ include file="include.jsp"%>
或
<%@ include file="include.html"%>
```

​	静态包含就是将内容进行了直接的替换，就好比程序中定义的变量一样实在servlet引擎转译时，就把此文件内容包含了进去（两个文件的源码整合到一起，全部放到_jspService方法中），所以只生成了一个servlet，所以两个页面不能有同名的变量。运行效率要高一点点。耦合性较高，不够灵活。

#### include 动态包含

 	动态包含在代码的编译阶段，包含和被包含部分时两个独立的部分，只有当运行时，才会动态包含进来，好比方法的调用。

```jsp
<jsp:include page="include.jsp"></jsp:include>
```

注意：动态包含， 中间不要加任何内容，包括空格，除非确认要使用参数，否则报错！

```jsp
<jsp:include page="include.jsp"></jsp:include>
<%
	String s = "hello.jsp";
%>
<jsp:include page="<%=a %>"></jsp:include>
```

​	使用动态包含还可以通过在页面之间传参。

​	接收参数通过request.getParameter(name);

 

**特点**：1.动态包含相当于方法的调用

​			2.动态包含会生成多个源文件

​			3.可以定义同名变量

​			4.效率高，耦合度低

 

### JSP的四大域对象

​	在JSP中提供了四种属性的保存范围，所谓的保存范围，指的是设置的对象，可以再多少个页面中保存并可以继续使用

​	1.page范围

​			pageContext：只在一个页面中保存属性，跳转之后无效。

​	2.request范围

​			request：只在一次请求中保存，服务器跳转后依然有效

​	3.session范围

​		session：在一次会话范围中，无论何种跳转都可以使用

​	4.application范围

​			application：在整个服务器上保存

![](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\1655193879249.png)

#### 验证属性范围的特点

​	1.page 

​		本页面中取得，服务器端跳转（<jsp:forward>>）后无效

​	2.request

​		服务器跳转有效，客户端跳转无效

​		如果是客户端跳转，则相当于发出了两次请求，那么第一次的请求将不存在了；如果希望不管是客户端还是服务器跳转，都能保存的话，就需要继续扩大范围。

​	3.session

​		无论客户端还是服务端都可以取得，但是现在重新开启一个新的浏览器，则无法取得之前设置的session了，以为每一个session只保存在当前的浏览器当中，并在相关的也面取得。

​		对于服务器而言，每一个连接到它的客户端都是一个session对象

​		如果想要让属性设置一次后，不管是否是新的浏览器打开都能取得则可以使用application

​	4.application

​		所有的application属性直接保存在服务器上，所有的用户（每一个session）都可以直接访问取得

​		只要是通过application设置的属性，则所有的session都可以取得，表示公共的内容，但是如果此时服务器重启了，则无法取得了，因为关闭服务器后，所有的属性都消失了，所以需要重新设置。

​       