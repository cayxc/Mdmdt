---

---


# 主题演示demo

这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容。这是一段正文内容。
## 主题演示主题演示主题演示主题演示主题演示
这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容。是一段正文内容这是一段正文内容这是一段正文内容......

# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
---
# 引用文本
> 这是引用文本样式这是引用文本样式这是引用文本样式这是引用文本样式这是引用文本样式这是引用文本样式 <a href=''>这是超链接</a>。这种格式以`this is code`这是引用文本样式这是引用文本样式。
>
> > 这是嵌套引用文本样式这是嵌套引用文本样式这是嵌套引用文本样式这是嵌套引用文本样式......
---
[这是一个超链接文本样式](www.xxx-xy.com)

*斜体文本_斜体文本斜体文本斜体文本斜体文本*
**这些是加粗文本这些是加粗文本这些是加粗文本这些是加粗文本这些是加粗文本😀✓♸**

==标记文本标记文本标记文本标记文本==

<u>下划线下划线下划线下划线下划线</u>

的发~生大~发父^阿斯顿^

~这是删除文这是删除文本本~

这是上标样式：^上标^样式<sup>上标</sup> ，上标样式<sup>(x)</sup> ，上标样式<sup>[01]</sup>

这是下标样式：<sub>下标</sub>样式<sub>下标</sub> ，下标样式<sub>(y)</sub> ，下标样式<sub>[02]</sub>

上下标应用示例：>H<sub>2</sub>O 是液体，2<sup>10</sup> 运算结果是 1024

<!--这是注释内容这是注释内容-->

[^父]: 发生大发

^发撒的积分卡上的^

[^飞机上的快乐]: 发生大发



# 有序列表

1.这是有序列表
2.这是有序列表
3.这是有序列表
	1.这是有序列表
	2.这是有序列表
	3.这是有序列表

# 无序列表

- 这是无序列表
- 这是无序列表
- 这是无序列表
	- 这是无序列表
	- 这是无序列表
	- 这是无序列表

---
# 事项清单 

- [ ] 计划任务
- [x] 计划任务
- [ ] 计划任务
- [x] 计划任务

---

# 这是表格

|列表头 | 相关说 |  |  |  |
| -- | -- | -- | -- | -- |
|   这是第1行   | 相关说明相关说明相关说明相关说明相关说明...... |  |  |  |
|   这是第2行   | 相关说明相关说明相关说明相关说明相关说明...... |  |  |  |
|   这是第3行   | 相关说明相关说明相关说明相关说明相关说明...... |  |  |  |
|   这是第4行   | 相关说明相关说明相关`composer require --dev barryvdh/laravel-ide-helper`说明相关说明相关说明...... |  |  |  |
|  |  | | | |
|  |  | | | |
| | | | | |

|      |      |      |
| ---- | ---- | ---- |
|      |      |      |
|      |      |      |
|      |      |      |



---

# 代码块样式

单行代码块：`composer require --dev barryvdh/laravel-ide-helper`

$composer require --dev barryvdh/laravel-ide-helper$



大段~~代码~~块：

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>主题演示demo</title>
    <link rel="stylesheet" href="./scss/index.css">
    <script src="js/highlight.min.js"></script>
    <script src="./js/mdth.js"></script>
</head>
<body>

<h1>主题演示demo</h1>
<p>这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容。这是一段正文内容。</p>
  </body>
</html>
```

这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容这是一段正文内容。这是一段正文内容。

```javascript
//滚动元素的top值
    var top0 = $("#zhutu").offset().top-zhi;
    var top1 = $(".aboutMeBox").offset().top-zhi;
    var top2 = $(".myWorksBox").offset().top-zhi;
    var top3 = $(".mySkillBox").offset().top-zhi;
    var top4 = $(".myExperienceBox").offset().top-zhi;
    var top5 = $(".contactBox").offset().top-zhi;

    //顶部导航栏点击效果
    $("header nav ul li").click(function () {
        var indexC = $(this).index();
        var weizhi = $(".swiper-slide section").eq(indexC).offset().top-62;
        // 滑动到相应位置
        $("html, body").animate({
            scrollTop: weizhi}, 500);
    });
    $(window).scroll(function(){
        // 滚动到相应元地方导航栏菜单样式发生改变
        for(var i=0; i<=5; i++){
            if($(this).scrollTop() >= eval('top'+i)){
                //正常导航栏样式
                $("#showNav ul li").eq(i).addClass('activeA');
                $("#showNav ul li").eq(i).children().addClass('activeB');
                $("#showNav ul li").eq(i).siblings('li').removeClass('activeA');
                $("#showNav ul li").eq(i).siblings('li').children().removeClass('activeB');
                //隐藏的导航栏样式
                $("#hiddenNav ul li").eq(i).css('border-bottom', '0.2rem solid #52d3aa');
                $("#hiddenNav ul li").eq(i).children().addClass('activeD');
                $("#hiddenNav ul li").eq(i).siblings('li').css('border-bottom', '0.1rem solid #E9E9E9');
                $("#hiddenNav ul li").eq(i).siblings('li').children().removeClass('activeD');
            }
        }

        //滚动条滚动的距离大于"我的作品"时返回顶部按钮出现
        var juli = $(this).scrollTop();
        if(juli >= top2){
            $("#backTop").fadeIn('slow');
        }
        if(juli == 0){
            $("#backTop").fadeOut('slow');
        }

    });
```



```css
/* 这是多行注释
   * 会输出到编译后的 css 文件中
   * ......
   * 多行注释
*/
//  sass
body {
  font-size: $size-16;
  line-height: 1.6;
  box-sizing: border-box;
}
$nav-color: #F90;  //全局变量
nav {
  $width: 100px;  //局部变量
  width: $width;
  color: $nav-color;
}
//编译后
nav {
  width: 100px;
  color: #F90;
}
    <div className="CodeMirror-gutter-wrapper" style="left: -39px;">
      <div className="CodeMirror-linenumber CodeMirror-gutter-elt"
           style="left: 0px; width: 30px;">4
      </div>
    </div>;
```

```php
<?php

namespace App\Models;

use App\Observers\UserObserver;
use Illuminate\Notifications\Notifiable;
use Illuminate\Foundation\Auth\User as AuthModel;

class User extends AuthModel
{
    use Notifiable;

    protected $guarded = [];

    /**
     * The attributes that should be hidden for arrays.
     *
     * @var array
     */
    protected $hidden = [
        'password', 'remember_token',
    ];

    public function blogs()
    {
        return $this->hasMany(Blog::class,'user_id');
    }

    //获取所有粉丝
    public function follower()
    {
        return $this->belongsToMany(User::class,'followers','user_id','follower')->withTimestamps();
    }

    //获取所有关注
    public function following()
    {
        return $this->belongsToMany(User::class,'followers','follower','user_id')->withTimestamps();
    }

    //查看用户是否是粉丝
    public function isFollow($uid)
    {
        return $this->follower()->wherePivot('follower',$uid)->first();
    }

    //关注或取关
    public function followToggles($ids)
    {
        $ids = is_array($ids) ? : [$ids];
        return $this->follower()->toggle($ids);
    }

    protected static function boot()
    {
        //在模型中注册观察者
        static::observe(UserObserver::class);
        parent::boot();
    }
}

```





[测试](w w..efasdf adsf.cdsom)

[测试链接]: www.cjdlsfjs.com

[jsdlkfjaksdf](fsadfasf)

------

<img src="/Users/cayxc/Pictures/paper/d07bd618cd93.jpeg" alt="苏打粉" style="zoom:30%;" />

![]()

[TOC]

