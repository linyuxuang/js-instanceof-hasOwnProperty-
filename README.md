# js-instanceof-hasOwnProperty-
instanceof    hasOwnProperty



1）   hasOwnProperty() 检查是不是自身对象的属性（非继承）-->如果都是自身对象属性  返回true 否则 false
      
     
        var obj={
        	name:"121",
        	age:23,
        	__proto__:{
        		lasName:"haha"
        	}
        }
        for(var key in obj){
        	
        	if(obj.hasOwnProperty(key)){
        		console.log(obj[key])   //  121   23
        	}
        }
    

2)
       instanceof  作用: 
                    如: A   instanceof  B-->A对象 是不是 B构造函数构造出来的                       
                         
                  注意: 看A对象的原型链上  有没有 B的原型      
    
      function Person(){
      	
      }
      var person=new Person();
    
       person instanceof Person      //true
    
       [] instanceof Array  // true
     
       [] instanceof Person   //false
    
     
