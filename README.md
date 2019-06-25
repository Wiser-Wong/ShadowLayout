# 带阴影的布局 ShadowContainer
## 操作手册
    <!-- 阴影-->
    <declare-styleable name="ShadowContainer">
        <attr name="container_shadowColor" format="color" />
        <attr name="container_shadowRadius" format="dimension" />
        <attr name="container_shadowRoundRadius" format="dimension" />
        <attr name="container_shadowShape">
            <flag name="container_rectangle" value="0x0001" />
            <flag name="container_round_rectangle" value="0x0100" />
        </attr>
        <attr name="container_shadowSide">
            <flag name="container_all" value="0x1111" />
            <flag name="container_left" value="0x0001" />
            <flag name="container_top" value="0x0010" />
            <flag name="container_right" value="0x0100" />
            <flag name="container_bottom" value="0x1000" />
        </attr>
        <attr name="container_round_corner">
            <flag name="container_corner_all" value="0x1111" />
            <flag name="container_corner_leftTop" value="0x0001" />
            <flag name="container_corner_leftBottom" value="0x0010" />
            <flag name="container_corner_rightTop" value="0x0100" />
            <flag name="container_corner_rightBottom" value="0x1000" />
        </attr>
    </declare-styleable>
## 集成
    
    allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  
  
    dependencies {
	        implementation 'com.github.Wiser-Wong:ShadowLayout:1.0.2'
	}

### 截图
![images](https://github.com/Wiser-Wong/ShadowLayout/blob/master/images/shadow.gif)
