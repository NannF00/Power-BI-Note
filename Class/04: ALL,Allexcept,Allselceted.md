清除度量值的筛选功能

为什么用all?

不用all,就筛选成1了,不是总数26

# 

![image](https://user-images.githubusercontent.com/117897416/236496946-e2f634b1-e1b8-4cff-8ec7-fa8bb2f158d5.png)

当ALL函数参数为表的时候,忽略所有筛选条件,无论是表的内部还是外部切片器

![image](https://user-images.githubusercontent.com/117897416/236487937-4ce2c98e-cf31-464f-9968-6bbc64a75b1b.png)


- 销售表中的商品数量=Calculate(CountRows'商品表','销售表')

以销售表中具有的商品作为商品表的筛选条件. 换个思维

- 计算占比

[度量值]/[all(度量值)]

![image](https://user-images.githubusercontent.com/117897416/236850767-6d552adc-4658-4c54-9274-5d180894e589.png)

今天就到这里

# Allselected

牵扯到计算百分比(外部有切片器)的时候用: 可以只计算被选择的

对比: 

![image](https://user-images.githubusercontent.com/117897416/237046500-69d495b4-e382-4e49-ba6c-a702995c0409.png)

![image](https://user-images.githubusercontent.com/117897416/237046849-b1494a33-7502-400b-8039-92ffd3cb0827.png)




