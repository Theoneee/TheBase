# TheBase


#### [Gitee](https://gitee.com/theoneee/TheBase)

#### 介绍
主要以[QMUI](https://github.com/Tencent/QMUI_Android)封装的一个基础框架。

#### 预览


[如何写一个常见的主界面（ViewPager+Tab）](https://gitee.com/theoneee/TheBase/blob/master/gank/src/main/java/the/one/gank/ui/fragment/GankIndexFragment.java)

![输入图片说明](https://images.gitee.com/uploads/images/2019/0925/164724_adc57bb3_2286054.png "index_fragment.png")


[如何写一个常见的TitleBar+Tab+ViewPager布局](https://gitee.com/theoneee/TheBase/blob/master/gank/src/main/java/the/one/gank/ui/fragment/CategoryFragment.java)

![输入图片说明](https://images.gitee.com/uploads/images/2019/0925/164857_396d70bc_2286054.png "titlebar_tab_viewpager.png")


[如何写一个常见的列表显示界面](https://gitee.com/theoneee/TheBase/blob/master/gank/src/main/java/the/one/gank/ui/fragment/GankFragment.java)

![输入图片说明](https://images.gitee.com/uploads/images/2019/0925/164925_69861416_2286054.gif "70641806-d40e-434e-8220-e087e0f31a93.gif")

懒加载？下拉刷新？加载更多？空页面？网络错误页面?  统统都封装好了。

LIST? GRID? STAGGERED? 一句代码

```
  @Override
    protected int setType() {
        return TYPE_LIST? TYPE_GRID? TYPE_STAGGERED;
    }
```


#### 更多请结合几个项目看代码

[Demo](https://gitee.com/theoneee/TheBase/raw/master/apk/release/the.one.demo_1.0_release.apk)


[Aqtour](https://gitee.com/theoneee/TheBase/raw/master/apk/release/the.one.aqtour_1.0_release.apk)


[Gank](https://gitee.com/theoneee/TheBase/raw/master/apk/release/the.one.gank_1.0_release.apk)


[Mzitu](https://gitee.com/theoneee/TheBase/raw/master/apk/release/the.one.mzitu_1.0_release.apk)


[Wallpaper](https://gitee.com/theoneee/TheBase/raw/master/apk/release/the.one.wallpaper_1.0_release.apk)



#### 交流

QQ群： 761201022


#### 使用

1.根build 里添加

```
allprojects {
    repositories {
        maven { url 'https://jitpack.io' }
        google()
        jcenter()
    }
}
```
2.app的build里dependencies下添加
```
implementation 'com.gitee.theoneee:TheBase:lastversion`

```

[lastversion](https://gitee.com/theoneee/TheBase/releases)

```

以下非必须
annotationProcessor 'com.ljx.rxhttp:rxhttp-compiler:$rxhttpVersion' //集成了RxHttp，如需使用则添加
annotationProcessor 'com.jakewharton:butterknife-compiler:$butterknifeVersion' //butterknife 注解

```

[版本见这里](https://gitee.com/theoneee/TheBase/blob/master/baseConfigs.gradle)


3.manifest里application指定  
```

android:name="the.one.base.BaseApplication" 

```

或者继承 BaseApplication再指定成自己的

style AppTheme继承BaseTheme

```

<style name="AppTheme" parent="BaseTheme"/>

```

#### 以上三个必须要！！！


#### 感谢

[QMUI](https://github.com/Tencent/QMUI_Android)

[RxHttp](https://github.com/liujingxing/okhttp-RxHttp)

#### 第三方库

```
 'com.github.CymChad:BaseRecyclerViewAdapterHelper:2.9.40'
 'homhomlin.lib:sldinglayout:0.9.0'
 'com.github.bumptech.glide:glide:4.8.0'
 'com.jakewharton:butterknife:8.8.1'
 'org.greenrobot:eventbus:3.1.1'
 'com.belerweb:pinyin4j:2.5.1'
 'com.android.support:multidex:1.0.3'
 'com.github.tbruyelle:rxpermissions:0.10.2'
 'com.ms-square:expandableTextView:0.1.4'
 'com.github.chrisbanes:PhotoView:2.0.0'
 'com.orhanobut:logger:2.2.0'
 'com.wkp:StickLayout:1.0.6'
 'com.github.LuckSiege.PictureSelector:picture_library:v2.2.3'
 'top.androidman:superbutton:1.1.0'
 'com.rxjava.rxhttp:rxhttp:2.0.0'

  .....

```

还有一些为了自定义，集成到了项目里，所以并没有在依赖里出现，但是都保留原作者信息。


项目内容数据纯属项目练手。



you are the one.




