
# RecycleView 使用基本流程 #



## xml布局文件 ##

activity_main添加Android.support.v7.widget.RecycleView控件

新建item.xml自定义布局文件，添加相应的控件。

##MainActivity##

**初始化操作**

初始化相应控件

RecycleView recycleview

初始化数据源

String data[]

初始化适配器(自定义适配器)

MyAdapter myAdapter

**找到对应控件**

recycleview = findviewById

**new MyAdapter**

## MyAdapter ##

**自定义ViewHolder显示呈现内容**

public class MyAdapter extend RecyclerView.Adapter<MyViewHoder>

**构造函数传入相应的数据源**

Myadapter(String data[])

**创建新的ViewHoder 解析Xml成View**

MyViewHolder onCreateViewHolde()

新建一个视图填充器(重父布局中获取)

将父布局中的Xml视图转化为View对象

将View对象填充到viewHoder中

**获取数据**

getItemCount()

**绑定数据与页面**

onBindViewHolder(MyViewHolder holder, int position) 

## MyViewHoder ##

**初始化item中的控件**




