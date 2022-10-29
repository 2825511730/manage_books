

**计算机类毕设源码大全：[十几套计算机专业毕业设计文档及源码分享](https://mp.weixin.qq.com/mp/homepage?__biz=MzkyMDAxNTQ4NQ==&hid=5&sn=097a81acff1e1971604ea1b571c13b9e&scene=18)** 

**系统演示链接：[点击这里查看演示](http://books.cyouagain.cn)**

**获取源码：微信搜索公众号【IT学长】回复“基于web的图书管理系统”**

**详细开发文档：[《基于Web的图书管理系统设计与实现（附源码下载地址）》](https://mp.weixin.qq.com/s/zZ40HrMcNoUx87aH8dGfhw)**

**运行教程：[《基于Web的图书管理系统运行教程》](https://mp.weixin.qq.com/s/tMrcyR2cpHfZ4NjGdBUIrA)**

**演示截图：[《基于Web的图书管理系统演示截图》](https://blog.csdn.net/m0_73470247/article/details/126644988)**

@[toc]

## 01 系统简述
图书管理系统就是利用计算机，结合互联网对图书进行结构化、自动化管理的一种软件，来提高对图书的管理效率。本系统采用Java+Servlet+Jsp 的方式实现基于web的图书管理系统。

## 02 开发工具及相关技术
#### 2.1 Java技术
Java 是由 Sun Microsystems 在 1995 年首先发布的编程语言和计算平台。有许多应用程序和 Web 站点只有在安装 Java 后才能正常工作，而且这样的应用程序和 Web 站点日益增多。Java 快速、安全、可靠。从笔记本电脑到数据中心，从游戏控制台到科学超级计算机，从手机到互联网，Java 无处不在。

#### 2.2 HTML、css、javascript技术
HTML的英文全称是 Hypertext Marked Language，即超文本标记语言。HTML是由Web的发明者 Tim Berners-Lee和同事 Daniel W. Connolly于1990年创立的一种标记语言，它是标准通用化标记语言SGML的应用。用HTML编写的超文本文档称为HTML文档，它能独立于各种操作系统平台(如UNIX， Windows等)。使用HTML语言，将所需要表达的信息按某种规则写成HTML文件，通过专用的浏览器来识别，并将这些HTML文件“翻译”成可以识别的信息，即现在所见到的网页。

层叠样式表(英文全称：Cascading Style Sheets)是一种用来表现HTML（标准通用标记语言的一个应用）或XML（标准通用标记语言的一个子集）等文件样式的计算机语言。CSS不仅可以静态地修饰网页，还可以配合各种脚本语言动态地对网页各元素进行格式化。CSS 能够对网页中元素位置的排版进行像素级精确控制，支持几乎所有的字体字号样式，拥有对网页对象和模型样式编辑的能力。

JavaScript（简称“JS”） 是一种具有函数优先的轻量级，解释型或即时编译型的编程语言。虽然它是作为开发Web页面的脚本语言而出名的，但是它也被用到了很多非浏览器环境中，JavaScript 基于原型编程、多范式的动态脚本语言，并且支持面向对象、命令式和声明式（如函数式编程）风格。JavaScript在1995年由Netscape公司的Brendan Eich，在网景导航者浏览器上首次设计实现而成。因为Netscape与Sun合作，Netscape管理层希望它外观看起来像Java，因此取名为JavaScript。但实际上它的语法风格与Self及Scheme较为接近。JavaScript的标准是ECMAScript 。截至 2012 年，所有浏览器都完整的支持ECMAScript 5.1，旧版本的浏览器至少支持ECMAScript 3 标准。2015年6月17日，ECMA国际组织发布了ECMAScript 的第六版，该版本正式名称为 ECMAScript 2015，但通常被称为ECMAScript 6 或者ES6。

#### 2.3 Servlet技术
Servlet（Server Applet）是Java Servlet的简称，称为小服务程序或服务连接器，用Java编写的服务器端程序，具有独立于平台和协议的特性，主要功能在于交互式地浏览和生成数据，生成动态Web内容。

狭义的Servlet是指Java语言实现的一个接口，广义的Servlet是指任何实现了这个Servlet接口的类，一般情况下，人们将Servlet理解为后者。Servlet运行于支持Java的应用服务器中。从原理上讲，Servlet可以响应任何类型的请求，但绝大多数情况下Servlet只用来扩展基于HTTP协议的Web服务器。
#### 2.4 Eclipse开发工具
Eclipse 是一个开放源代码的、基于Java的可扩展开发平台。就其本身而言，它只是一个框架和一组服务，用于通过插件组件构建开发环境。幸运的是，Eclipse 附带了一个标准的插件集，包括Java开发工具（Java Development Kit，JDK）。

#### 2.5 MySql数据库
MySql是最流行的关系型数据库管理系统，在WEB应用方面MySQL是最好的RDBMS(Relational Database Management System：关系数据库管理系统)应用软件之一。MySql数据库有以下特点：

 1. Mysql是开源的，所以你不需要支付额外的费用。 
 3. Mysql支持大型的数据库。可以处理拥有上千万条记录的大型数据库。
 4. MySQL使用标准的SQL数据语言形式。
 5. Mysql可以允许于多个系统上，并且支持多种语言。这些编程语言包括C、C++、Python、Java、Perl、PHP、Eiffel、Ruby和Tcl等。
 6. Mysql对PHP有很好的支持，PHP是目前最流行的Web开发语言。
 7. MySQL支持大型数据库，支持5000万条记录的数据仓库，32位系统表文件最大可支持4GB，64位系统支持最大的表文件为8TB。
 8. Mysql是可以定制的，采用了GPL协议，你可以修改源码来开发自己的Mysql系统。

## 03 系统功能描述
系统的用户主要有两大类：一是图书管理系统的管理员，二是普通用户。根据用户类型的不同，将系统划分为普通用户端和管理员端，它们具有的主要功能如下：

**用户端**
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200711142212377.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQwNjI1Nzc4,size_16,color_FFFFFF,t_70)

图书查询：根据图书编号、图书名称查询图书信息，可查询图书的编号、名称、分类、作者、价格、在馆数量等。

借阅信息：可查询图书的基本信息、借阅日期、截止还书日期、超期天数等。

借阅历史：查询自己以往的借阅历史，包括哪些图书等具体信息。

我的：查看个人资料，修改账户密码，退出系统。

**管理员端**
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200711142331762.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQwNjI1Nzc4,size_16,color_FFFFFF,t_70)
图书管理：根据图书编号、图书名称查询图书基本信息，添加、修改、删除图书。

图书分类管理：根据分类名称查询图书分类信息，添加、修改、删除图书分类。

图书借阅：展示所有正在借阅图书的信息。

图书归还：展示所有已归还图书的信息。

公告管理：向用户发布公告。

读者管理：根据账号、姓名查询读者基本信息，添加、修改、删除读者信息。

我的：查看个人资料，修改账户密码，退出系统。

## 04 工程结构及其说明
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200711142439453.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQwNjI1Nzc4,size_16,color_FFFFFF,t_70)
项目名称：manage_books
Package包说明：
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200711142614767.png)

## 05 主要功能详细设计与实现
#### 5.1 用户端--图书查询模块
用户访问图书查询模块时显示当前可以借阅图书，有按图书名称查询图书信息的功能，可以进行借书操作。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200711142820895.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQwNjI1Nzc4,size_16,color_FFFFFF,t_70)
其中查询功能的Servlet代码如下：

```java
package com.cya.controller;
import java.io.IOException;
import java.util.ArrayList;
import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import com.cya.dao.BookDao;
import com.cya.pojo.Book;
/**
 * Servlet implementation class selectServlet
 */
@WebServlet("/selectServlet")
public class selectServlet extends HttpServlet {
    private static final long serialVersionUID = 1L;

    /**
     * @see HttpServlet#HttpServlet()
     */
    public selectServlet() {
        super();
        // TODO Auto-generated constructor stub
    }

    /**
     * @see HttpServlet#doGet(HttpServletRequest request, HttpServletResponse response)
     */
    protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        // TODO Auto-generated method stub
       //response.getWriter().append("Served at: ").append(request.getContextPath());

    }

    /**
     * @see HttpServlet#doPost(HttpServletRequest request, HttpServletResponse response)
     */
    protected void doPost(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        // TODO Auto-generated method stub
       //doGet(request, response);
        request.setCharacterEncoding("UTF-8");
        response.setContentType("text/html;charset=UTF-8");
        //因为在管理员界面和读者界面都有查找功能，为了将查找的结果返回正确的页面，设置了tip，tip=1表示管理员界面
        int tip = Integer.parseInt(request.getParameter("tip"));
        String name = request.getParameter("name");
        BookDao bookdao = new BookDao();
        ArrayList<Book> data = bookdao.getLikeList(name);
        //将获取的结果存入请求中
        request.setAttribute("data", data);
        String url = "";
        //转发不同的界面
        if (tip == 1) {
            url = response.encodeURL("/books/admin/admin_books.jsp");
        } else {
            url = response.encodeURL("/books/user/select.jsp");
        }
        //将请求转发
        request.getRequestDispatcher(url).forward(request, response);
    }

}
```

#### 5.2 用户端--借阅信息模块
当普通用户借阅完图书，会在该模块自动生成借阅信息，如借阅日期，归还日期，也可在该模块进行还书，如下图所示。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200711143029669.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQwNjI1Nzc4,size_16,color_FFFFFF,t_70)
其中，还书功能的Servlet代码如下：

```java
package com.cya.controller;
import java.io.IOException;
import java.io.PrintWriter;
import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import javax.servlet.http.HttpSession;
import com.cya.pojo.Admin;
import com.cya.dao.AdminDao;
import com.cya.dao.BookDao;
/**
 * Servlet implementation class borrowServlet
 */
@WebServlet("/borrowServlet")
public class borrowServlet extends HttpServlet {
    private static final long serialVersionUID = 1L;

    /**
     * @see HttpServlet#HttpServlet()
     */
    public borrowServlet() {
        super();
        // TODO Auto-generated constructor stub
    }

    /**
     * @see HttpServlet#doGet(HttpServletRequest request, HttpServletResponse response)
     */
    protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        // TODO Auto-generated method stub
       //response.getWriter().append("Served at: ").append(request.getContextPath());
        //设置编码类型
        request.setCharacterEncoding("UTF-8");
        response.setContentType("text/html;charset=UTF-8");
        BookDao bookdao = new BookDao();
        //为了区分借书和还书的功能，设置tip，tip为1，表示借书
        int tip = Integer.parseInt(request.getParameter("tip"));
        if (tip == 1) {
            //获取图书id
            int bid = Integer.parseInt(request.getParameter("bid"));
            HttpSession session = request.getSession();
            Admin admin = new Admin();
            String status=request.getParameter("status");
            String id="";
            if(status.equals("user")) {
                //获取到存入session的读者id
                id = (String) session.getAttribute("uid");
            }
            else {
                //获取到存入session的aid读者id
                 id = (String) session.getAttribute("aid");
            }

            AdminDao admindao = new AdminDao();
            //通过aid获取到读者的信息
            admin = admindao.get_AidInfo2(id);
            //将借阅记录存入数据表
            bookdao.borrowBook(bid, admin);
            response.sendRedirect("/manage_books/books/user/select.jsp");
        } else {
            //还书功能，获取借阅记录的hid
            int hid = Integer.parseInt(request.getParameter("hid"));
            /**
             * 还书在管理员和读者界面都有，为了区分，设置了show字段，show为1表示读者界面
             */
            int show = Integer.parseInt(request.getParameter("show"));
            //调用还书函数，改变status字段
            bookdao.borrowBook2(hid);
            if (show == 1) {
                response.sendRedirect("/manage_books/books/user/borrow.jsp");
            } else {
                response.sendRedirect("/manage_books/books/admin/admin_borrows.jsp");
            }

        }

    }

    /**
     * @see HttpServlet#doPost(HttpServletRequest request, HttpServletResponse response)
     */
    protected void doPost(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        // TODO Auto-generated method stub
        doGet(request, response);
    }

}
```
#### 5.3 管理员端--图书管理模块
管理员可以通过根据图书号 、图书名称，作者名称，出版社等查询图书信息。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200711143221127.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQwNjI1Nzc4,size_16,color_FFFFFF,t_70)

管理员登录系统以后，可以进行图书添加操作，这是管理员主要的输入信息部分，填写好各项信息后，单击保存按钮，系统将对这些信息进行处理。界面见下图所示：
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200711143310535.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQwNjI1Nzc4,size_16,color_FFFFFF,t_70)

除此以外，管理员对已经添加好的图书信息有修改权限。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200711143409474.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQwNjI1Nzc4,size_16,color_FFFFFF,t_70)
其中，添加图书功能的代码如下：

```java
package com.cya.controller;
import java.io.IOException;
import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import com.cya.dao.BookDao;
/**
 * Servlet implementation class AddBookServlet
 */
@WebServlet("/AddBookServlet")
public class AddBookServlet extends HttpServlet {
    private static final long serialVersionUID = 1L;

    /**
     * @see HttpServlet#HttpServlet()
     */
    public AddBookServlet() {
        super();
        // TODO Auto-generated constructor stub
    }

    /**
     * @see HttpServlet#doGet(HttpServletRequest request, HttpServletResponse response)
     */
    protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        // TODO Auto-generated method stub
//        response.getWriter().append("Served at: ").append(request.getContextPath());
    }

    /**
     * @see HttpServlet#doPost(HttpServletRequest request, HttpServletResponse response)
     */
    protected void doPost(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        // TODO Auto-generated method stub
//        doGet(request, response);
        //设置编码类型
        request.setCharacterEncoding("UTF-8");
        response.setContentType("text/html;charset=UTF-8");
        //获取要添加图书的信息
        String card = request.getParameter("card");
        String name = request.getParameter("name");
        String type = request.getParameter("type");
        String autho = request.getParameter("autho");
        String press = request.getParameter("press");
        int num = Integer.parseInt(request.getParameter("num"));
        BookDao bookdao = new BookDao();
        //调用函数，存入图书
        bookdao.addBook(card, name, type, autho, press, num);
        response.sendRedirect("/manage_books/books/admin/admin_books.jsp");
    }

}
```

#### 5.4 管理员端--图书分类模块
管理员在该界面可以增加、删除、修改图书分类信息，操作效果如图。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200711143555646.png)
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200711143617913.png)
修改图书分类功能的代码如下：

```java
package com.cya.controller;
import java.io.IOException;
import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import com.cya.dao.BookDao;
import com.cya.dao.TypeDao;
/**
 * Servlet implementation class updateBookTypeServlet
 */
@WebServlet("/updateBookTypeServlet")
public class updateBookTypeServlet extends HttpServlet {
    private static final long serialVersionUID = 1L;

    /**
     * @see HttpServlet#HttpServlet()
     */
    public updateBookTypeServlet() {
        super();
        // TODO Auto-generated constructor stub
    }

    /**
     * @see HttpServlet#doGet(HttpServletRequest request, HttpServletResponse response)
     */
    protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        // TODO Auto-generated method stub
//        response.getWriter().append("Served at: ").append(request.getContextPath());
    }

    /**
     * @see HttpServlet#doPost(HttpServletRequest request, HttpServletResponse response)
     */
    protected void doPost(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        // TODO Auto-generated method stub
//        doGet(request, response);
        //修改图书类型信息
        request.setCharacterEncoding("UTF-8");
        response.setContentType("text/html;charset=UTF-8");
        String name = request.getParameter("name");
        int tid = Integer.parseInt(request.getParameter("tid"));
        TypeDao typedao = new TypeDao();
        typedao.updateTypeBook(tid, name);
        response.sendRedirect("/manage_books/books/admin/admin_booksType.jsp");
    }

}
```

## 06 源码下载

本期文章就分享到这里，创作不易欢迎点赞分享！原创文章，转载请注明出处。如需<font color='red'>**本系统完整源码请在微信搜索公众号【IT学长】，后台回复 `“基于web的图书管理系统”`**</font>。
