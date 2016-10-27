# Markdown Test
# 1.English Version
This is a markdown syntax test file.
# 2.中文版本
这是一个markdown语法测试文件。
# 3.引用  
**示例**
*引用*
>这是一个引用语法。  
>书山有路勤为径，学海无涯苦作舟。  

# 4.代码示例  
* 1 **代码行inline code**  
` rm -rf /home/shiyan/test `  
``
	select * from users where userid = 100
``  
```javascript
var a=1,b=2;  
var c=a+b;  
alert(c);   
```
* 2 **代码块block code**  

```
	public void main(){
		System.out.println("Test.md");
	}
	public void test(String str){
		if("test".equals(str)){
			System.out.println("Congratulations！ The right answer is test.");
		}
	}

	public class Test{
		public static void main(String args[]){
			int a=1,b=2;
			int c=a+b;
			System.out.println(c);
		}
	}  
```
## 5 图床和链接  
**图床**
![coding](http://i1.piimg.com/4851/db390845e99c4f94.jpg)

分割线
---
---

**链接**  
[百度一下，你就知道](http://www.baidu.com)  
## 6 表格
| Name | Sex | Age |
| -----|:----:|:----:|
|luxingda| male | 23|
|李明|female| 18|

## 7 代码框
```  
	public ModelAndView handleRequest(HttpServletRequest request,
			HttpServletResponse response) throws Exception {
		ModelAndView mv = new ModelAndView();
		mv.addObject("msg", "controller1 configuration");
		mv.setViewName("hello");
		return mv;
	}
```

```
	public class User{
		private String userid;
		private String username;
		private String password;
		private String priority;
		public User(){}
		public User(String userid,String username,String password,String priority){
			this.userid=userid;
			this.username=username;
			this.password=password;
			this.priority=priority;
		}
		public void setUserid(){}...
		public void static void Main(String args[]){
			User user=new User();
			user.setUserid(UUID.random(10).toString());
			user.setUsername("Liming");
			user.setPassword("admin123");
			user.setPriority("3");
		}
		public boolean addUser(User user){
			UserDaoImpl udi=new UserDao();
			udi.addUser(user);
		}
	}
```