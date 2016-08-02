# Android CouponView 卡券视图#

1.效果：

CouponView 是一个继承自LinearLayout的布局View,边缘可以实现自动裁剪效果，所以用来做优惠券等视图效果很好。

下图所示的四种视图，分别代表，不裁剪，只裁横向，只裁竖向，横竖皆裁四种情况。

<img src="http://i.imgur.com/pj4XTxr.png" width="30%" height="30%">

2.使用方法：

	在build.gradle中添加一行： 
	
	compile 'com.orzangleli.coupon:coupon:1.0.1'

在布局文件中添加代码：
	
	<com.orzangleli.coupon.view.CouponView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="vertical"
        android:background="#FF9933"
        coupon:gap="4dp"
        coupon:radius="5dp"
        coupon:radiusBackgroundColor="#ffffff"
        coupon:showHorizontal="true"
        coupon:showVertical="true"
        android:layout_marginTop="10dp"
        >

        <TextView
            android:layout_width="match_parent"
            android:layout_height="40dp"
            android:text="购物优惠券"
            android:textSize="20sp"
            android:textColor="#FFFFFF"
            android:layout_marginTop="5dp"
            android:layout_marginLeft="15dp"
            android:gravity="center_vertical"
            />

        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="满50元减10元"
            android:textSize="14sp"
            android:textColor="#FFFFFF"
            android:layout_marginTop="3dp"
            android:layout_marginLeft="25dp"
            android:gravity="center_vertical"
            />
        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="使用期限：一周内"
            android:textSize="14sp"
            android:textColor="#FFFFFF"
            android:layout_marginTop="3dp"
            android:layout_marginLeft="25dp"
            android:layout_marginBottom="15dp"
            android:gravity="center_vertical"
            />


    </com.orzangleli.coupon.view.CouponView>


注意在父节点上添加一行：

	xmlns:coupon="http://schemas.android.com/apk/res-auto"

3.属性解释：
	
gap:间隔线长度

radius:圆弧半径

radiusBackgroundColor:圆背景颜色   一般来说需要与主背景颜色相同

showHorizontal:显示横向裁剪

showVertical:显示竖向裁剪



----------


如果想关注我，可以关注我的博客： [orzangleli's blog](http://www.orzangleli.com)


