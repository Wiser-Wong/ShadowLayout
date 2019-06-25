# 带阴影的布局 ShadowContainer
## 截图
![images](https://github.com/Wiser-Wong/ShadowLayout/blob/master/images/shadow.gif)
## 集成
    
    allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  
  
    dependencies {
	        implementation 'com.github.Wiser-Wong:ShadowLayout:1.1'
	}
## 使用方法
    <com.wiser.library.shadow.ShadowContainer
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_alignParentBottom="true"
        android:layout_gravity="center"
        app:container_round_corner="container_corner_all"
        app:container_shadowBackgroundColor="@color/colorAccent"
        app:container_shadowColor="#000000"
        app:container_shadowRadius="10dp"
        app:container_shadowRoundRadius="10dp"
        app:container_shadowShape="container_rectangle"
        app:container_shadowSide="container_top">

        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_gravity="center"
            android:background="@mipmap/bg"
            android:gravity="center"
            android:padding="20dp"
            android:text="Hello World!"
            android:textColor="@color/colorAccent"
            android:textSize="40sp" />

    </com.wiser.library.shadow.ShadowContainer>
## 操作手册
* container_shadowBackgroundColor:阴影背景色
* container_shadowColor：阴影颜色
* container_shadowRadius：阴影边距
* container_shadowRoundRadius：阴影弧度半径
* container_shadowShape：阴影类型
   * container_rectangle：矩阵
   * container_round_rectangle：弧度矩阵
* container_shadowSide：阴影方向
   * container_all：所有方向
   * container_left：左边方向
   * container_top：上边方向
   * container_right：右边方向
   * container_bottom：下边方向
* container_round_corner：圆角类型
   * container_corner_all：四边角度圆角
   * container_corner_leftTop：左上角圆角
   * container_corner_leftBottom：左下角圆角
   * container_corner_rightTop：右上角圆角
   * container_corner_rightBottom：右下角圆角
