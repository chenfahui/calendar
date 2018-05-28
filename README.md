# calendar
日历，可选农历或公历，并年月日分别选择JS

公历转农历：

     calendar.solar2lunarFormat({
       solarYear:solarYear,//公历年
       solarMonth:solarMonth,//公历月
       solarDay:solarDay//公历天
     });
    
农历转公历：

     calendar.lunar2solarFormat({
       lunarYear:lunarYear,//农历年
       lunarMonth:lunarMonth,//农历月
       lunarDay:lunarDay//农历天
     });
    
获取年数据：

     calendar.listYear({
         isLunar:isLunar,//是否农历
         nowYear:nowYear//当前年份
     });
    
根据年，获取月数据：

     calendar.listMonth({
         isLunar:isLunar,//是否农历
         year:year, //选中年份
         nowYear:nowYear,//当前年份
         nowMonth:nowMonth,//当前月份
     });
    
根据年月，获取天数据：

     calendar.listDay({
         isLunar:isLunar,//是否农历
         year:year, //选中年份
         month:month,//选中月份
         nowYear:nowYear,//当前年份
         nowMonth:nowMonth,//当前月份
         nowDay:nowDay//当前天
     });
    
根据农历数值，换算成汉字：

     calendar.toChinaFormat({
       lunarYear:lunarYear,//农历年
       lunarMonth:lunarMonth,//农历月
       lunarDay:lunarDay//农历天
     });
