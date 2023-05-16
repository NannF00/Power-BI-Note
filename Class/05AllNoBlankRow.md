返回表中除空白以外所有的行

- 表=Allnoblankrow('子表')

- 表=Allnoblankrow('子表'[姓名])

- - 对列去重

- 返回:即使只有一列,它也是表

# all 与Allnoblankrow 的应用:核对差异

![image](https://github.com/NannF00/Power-BI-Note/assets/117897416/f5e91955-d3ff-4fa3-adeb-41ba6e306816)

用了Calculate(sum('销售表'[销量]),Allnoblankrow('商品表'))函数之后,返回的只有商品中有的商品的销量,对比all函数,可以看出空白行就是多加进去的商品

![image](https://github.com/NannF00/Power-BI-Note/assets/117897416/14c406b4-5f95-4fce-acd5-4fec0a5d260b)

