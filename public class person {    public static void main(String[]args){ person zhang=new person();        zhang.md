```java
public class person {
    public static void main(String[]args){ person zhang=new person();
        zhang.setName("sss");zhang.setAge(30);zhang.eat();

    }
    private String name; int age;public void setName(String name){
        this.name=name;} public void setAge(int age){
       this.age=age;}

    public int getAge() {
        return age;
    }

    void eat(){
        System.out.print(String.format("%s,ta%d岁",name,age));
    }
}
```

