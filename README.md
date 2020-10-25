# Java
学生选课模拟系统
#阅读程序

##实验目的
初步了解分析系统需求，从学生选课角度了解系统中的实体以及其关系，学会定义类中的属性以及方法；
掌握面向对象的类设计方法（属性、方法）；
掌握类的继承用法，通过构造方法实例化对象；
学会使用super(),用于实例化子类；
掌握使用Object根类的toString()方法，应用在相关对象的信息输出中。

##实验过程
1.人员（编号、姓名、性别）
2.教师（编号、姓名、性别、所授课程）
3.学生（编号、姓名、性别、所选课程）
4.课程（编号、课程名称、上课地点、时间、授课教师）

##核心方法
1.方法1
 //显示学生所选的课程
    public void displayCourse(){
        System.out.println("学生"+this.stuName+"所选课程有：");
        for(Course c:courses){
            if(c!=null){
                System.out.print(c.getName()+" ");
            }
        }
        System.out.println();
    }
2.方法2
 //子方法1：课是否被选过
    public boolean isSelectedCourse(Course course){
        boolean flag=false;
        for(Course c:courses){
            if(c==course){
                flag=true;
                break;
            }
        }
        return flag;
    }
3.方法3
    //子方法2：学生是否还有选修课位置
    public boolean isNullCourse(Course course){
        boolean flag=false;
        for(Course c:courses){
            if(c==null){
                flag=true;
                break;
            }
        }
        return flag;
    }



}


##实验结果
https://github.com/wangchen2019311152/Java/blob/main/%E5%AE%9E%E9%AA%8C%E7%BB%93%E6%9E%9C.png


##实验感想
在这一系列的实验中，我基本掌握了Java的编程规则、知识要点和一些小技巧，特别是对面向对象的编程思想和风格有了进一步的认识和体会。同时，因正确的编出程序而带来的成就感让我对编程更加感兴趣。对于在这些实验过程中，请教老师、同学互助、查阅资料等基本的学习方式，使我更加领悟到集体和团队的力量，也树立了敢于攻坚的信心。
说起来编程的经验应该是多了很多。但是在上机调试的时候还是遇到了相当多的问题。很多的错误都很难体会，有的时候是输入的错误，这种错误还是比较容易找出来的，但是有些问题，比如一些题目需要导入一些包，这一点就没有办法了。发现JAVA虽然看起来比C或C++要容易一点，但是由于它自身带有相当多的方法定义，这些个方法虽然不用我们自己再去编写了但是需要花相当多的时间去记忆那些方法是需要导入的，还有方法名……所以对我来说这真的是比C里简单几个文件的导入还要难上很多……还是觉得自己编的方法（函数）自己用的习惯。不过现在的编程的方向已经是面向对象和面向数据的了，所以我需要时间去适应这样的编程思想。
