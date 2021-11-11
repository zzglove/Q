```java
import java.text.DecimalFormat;
import java.util.Arrays;
import java.util .*;
public class Text02 {

    private static Object student;
    int class1;
    String name;

    public static void main(String[] args) {

        int u;
        int score;
        Scanner input = new Scanner(System.in);
        System.out.print("请输入姓名");
        int N = input.nextInt();
        StringBuffer buffer = new StringBuffer();
        student[][] students = new student[3][];
        students[1] = new student[N];
        students[2] = new student[N];
        students[3] = new student[N];
        for (int i = 0; i < students.length; i++) {
            if (input.hasNext()) {
                students[1][i] = new student(input.nextInt());
                students[2][i] = new student(input.next());
                students[3][i] = new student(input.nextDouble());
            } else {
                System.out.println("你输错了东西了");
            }
        }
        System.out.print(new student[N]);

        double[] j = new double[N];
        for (int k = 0; k < j.length; ) {
            j[k] = input.nextDouble();
        System.out.println(j);
        }

            double q = average(j);
            Arrays.sort(students[3]);
            System.out.println(q);
            System.out.println(Arrays.toString(students[3]));
            System.out.println(String.format("%.2f", q));
            Arrays.sort(students[3]);
            System.out.println(Arrays.toString(students[3]));
            if (q < 60) {
                System.out.print("不及格");
            }
            if (60 < q & q < 80) {
                System.out.print("良好");
            }
            if (80 < q & q <= 100) {
                System.out.println("优秀");
            }

        }
    }


    private static double average (double[] array ){
        double sum = 0;
        for(int i=0;i<array.length;i++){
            sum +=array[i] ;
        }return sum/array.length;
    }
    }
        class student{
         private int age;
         private String name;
         private double score;

            public student(int age, String name, double score){
                this.age = age;
            }
            public student(String name){
                this.name = name;
            }
            public student(double score){

                this.score = score;
            }

            @Override
            public String toString() {
                return "student{" +
                        "age=" + age +
                        ", name='" + name + '\'' +
                        ", score=" + score +
                        '}';
            }public String getname(){
                return name;
            }
            public void setname(String name ){
                this.name =name;
            }
            public int getAge(){
                return age;
            }
             public void setAge(int age){
                this.age =age;
             }
public double getScore(){
                return score;}
                public void setScore(double score){
                    this.score =score;
    }

        private static double average (int[] array){
    int sum = 0;
    for(int x:array){
        sum += x;
        }return (double)sum/(double)array.length;
        }
```

