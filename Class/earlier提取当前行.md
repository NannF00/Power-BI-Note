https://mp.weixin.qq.com/s?__biz=MzA4MzQwMjY4MA==&mid=2484067276&idx=1&sn=0226bc2d1a32733b1c59a170ac68362c&chksm=8e0c711bb97bf80d8b3feb6b805377d39bfa22a94b79b447393b4a27d5307fe7b67c195bab53&scene=21#wechat_redirect

    EARLIER(<column>, <number>)

    第一个参数是列名

    第二个参数一般可省略

    EARLIER函数提取本行对应的该列的值，实际上就是提取本行和参数列交叉的单元格

我的应用:获得截至当前日期,本年的工作日数目


    nWorkDayOfYear = 
        var theyear= 'Date'[nYear] 获取当前行年份
    return
        SUMX(FILTER('Date','Date'[nYear]=theyear&&'Date'[dDate]<=EARLIER('Date'[dDate])),'Date'[nISArbeitstag])
