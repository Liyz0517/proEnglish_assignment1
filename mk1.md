## Markdown初学

#### 四级标题

这是一个链接(按住command打开)[百度](https://www.baidu.com)

<a href="/Users/liyongzhen/Desktop/markdown文件/mk2.md">另一个markdown文件</a>



![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png)



[1]: http://static.runoob.com/images/runoob-logo.png

``` java
/**
	 * 查询购物车
	 * @param   user   用户实体类
	 * @return  String 表示跳转页面
	 */
	@RequestMapping("getShoppingCartByUser_id")
	public String getShoppingCartByUser_id( User user, HttpServletRequest request ) {
		
		// 根据用户id 获取购物车信息
		List<Product> list = userBizInf.getShoppingCartByUser_id(user);
		
		if ( list != null ) {
			request.setAttribute("msg", list);
			
			request.setAttribute( "aaa", userBizInf.getUserByUser_id(user) );
			
			return "/shoppingCart.jsp";
		} else {
			return "/error.jsp";
		}
	}
```



在 Markdown 中增加文献引用。[<sup>1</sup>](#refer-anchor-1)



1.列表1

* 表项1
* 表项2

2.

* 表项1
* 表项2

| 表头   | 表头   |
| ------ | ------ |
| 单元格 | 单元格 |
| 单元格 | 单元格 |

**粗体文字**

_斜体文字_

~~删除线文字~~

<u>带下划线的文字</u>

