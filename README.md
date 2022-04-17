# 小程序开发

### 事件绑定

* **bind**: 不会阻止冒泡,(bindtap:点击事件)
* **catch**:阻止冒泡事件,(catchtap:点击事件)

#### 事件流

1.捕获:从外向内,父元素捕获,向子元素传递,父元素不触发事件

2.目标子元素执行相应事件

3.冒泡:从内向外,子元素向父元素冒泡,触发父元素相应事件



### 路由跳转

* **navigateTo**:保留当前页面,跳转到应用内的某个页面,使用`wx.navigateBack`可以返回到原页,不能导航到`tabBar`页面(页面左上角带返回按钮,点击返回)

* **redirectTo**:关闭当前页面,跳转到应用内的某个页面.(页面左上角是主页按钮,点击返回主页)

* **switchTab**:跳转到`tabBar`页面,同时关闭其他非`tabBar`页面

* **navigateBack**:返回上一页面

* **reLanch**:关闭所有页面,打开到应用内的某个页面,(页面左上角是主页按钮,点击返回主页)其中关于它们的页面栈的关系如下:

  1.`navigateTo`:新页面入栈

  2.`redirectTo `:当前页面出栈,新页面入栈

  3.`navigateBack `:页面不断出栈,直到目标返回页,新页面入栈

  4.`switchTab`:页面全部出栈,只留下新的`Tab`页面

  5.`reLanch `:页面全部出栈,只留下新的页面

  

  

  











### tip

* `wx.canIUse('open-data.type.userAvatarUrl')`&nbsp;检查**open-data**元素上**type**属性的值是否为**userAvatarUrl**,有则返回**true**
* 

