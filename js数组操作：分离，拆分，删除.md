* 注意：以下操作可能会导致数组的长度改变，建议在使用时先将数组的长度存下来
* let arr_len=arr.length;
 ## slice
 slice 数组拆分：创建一个由当前数组中的一项或多项组成的新数组；不会修改原来数组
 用法：slice(para1) 从para1开始到数组的最后部分
       slice(para1,para2) 从原数组para1开始到para2的一个数组
       
 ## splice 
 splice用于删除数组中的元素
 splice(para1,para2) 删除数组中从para1到para2
 
 
 ## split
 * 根据特定的字符来切割字符串，返回一个数组
 
 
 ## 综合实例,将数组拆解成小数组
 function splitArr(arr,len){
 //arr目标数组 len 拆分规则，每个小组中有几个子元素的个数
 var arr_len=arr.length;
 var res=[]
 for(var i=0;i<arr_len;i+=len){
      res.push(arr.slice(i,i+len))
       }
 

 
  }
  
  * 例子
  arr=[1,2,3,4,5,6]
  res=splitArr(arr,3)
  
  res=[
  {1,2,3},
  {4,5,6}
  ]
       
       
 
             
