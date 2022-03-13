```java
char grade='';
switch (grade){
    case 'A':
        System.out.println("优秀");
        break;//可选
    case 'B':
        System.out.println("良好");
        break;
    case'C':
        System.out.println("及格");
        break;
    case'D':
        System.out.println("再接再厉");
        break;
    case'E':
        System.out.println("挂科");
        break;
    default:
        System.out.println("未知等级");
        break;
```

switch(       ){

case   value:

//语句

break；//可选

case  value：

//语句

break;//可选

//可以有任意数量的case语句

default：//可选

//语句

}

```java
    String  name ="狂神";
        switch (name){
            case "秦疆" :
                System.out.println("秦疆");
                break;
            case "狂神":
                System.out.println("狂神");
                break;
            default:
                System.out.println("输入信息有误");
        }
```

//JDK7之后可以输入字符串

