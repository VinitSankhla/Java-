import java.util.Arrays;
import java.util.Scanner;

class Basic{



    public static void printjava() {
        System.out.println("Hello Java");
    }

    public static void main(String[] args) {
        System.out.println("Hello world");
        String name1 = "Vinit S.";
        System.out.println(name1.length());
        String name2 = "Sankhla";
        System.out.println(name1 + " " + name2);
        System.out.println(name1.charAt(0));
        // replace function does not update the original value
        String name3 = name1.replace("i","I");
        System.out.println("after replacing "+ name3+ "Before Replacing " + name1);
        System.out.println(name1.substring(0,4));
        int english = 98;
        int physics = 96;
        int chemistry = 93;
        int maths = 89;
        int cse = 99;
        int[] marks = new int[5];
        marks[0]=english;
        marks[1]=physics;
        marks[2]=chemistry;
        marks[3]=maths;
        marks[4]=cse;
        // we can not print array directly, we can only print it's particular elements
        System.out.println(marks);
        System.out.println(marks[2]);
        // sorting of array by converting it into string
        System.out.println(Arrays.toString(marks));
        
        int[] marks1 = {98,65,35,35,87};
        // also a method to make an array
        System.out.println(Arrays.toString(marks1));
        // nested array 
        int[][] finalmark = {{98,97,96},{65,68,69}};
        for (int[] row : finalmark){
            System.out.println(Arrays.toString(row));
        }
        System.out.println(finalmark[0][0]);
        // Casting (If we not justify 18.99 to int then it will show error because int is small and double is big in size so this conversion is not possible so we need to do casting )
        int p = 100;
        int fp = p + (int)18.99;
        System.out.println(fp);
        // declaring final constants which cannot be changed further
        final double pi = 3.14;
        System.out.println(pi);
        int numb = 1;
        System.out.println(numb++);// numb value is first printed and then updated to 2
        System.out.println(numb);// here numb value is 2
        System.out.println(++numb);//here initially the value is increased by 1 and then printed 
        // math class
        System.out.println(Math.max(7,8));// can take only 2 values 
        System.out.println((int)(Math.random())*100); // by default random can only give values between 1 and 0
        
        
        // INPUT (Ensure Scanner class is imported)
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter your age");
        int age = sc.nextInt();
        System.out.println("Your age is : "+age); 
        // input string -------------------------------
        System.out.println("Enter your name");
        String name = sc.next();//takes only one word -------------
        System.out.println("Your name is "+name);
        sc.nextLine();
        System.out.println("Enter the sentence you wanna print");
        String sen = sc.nextLine();
        System.out.println("You Entered this sentence : "+sen);

        boolean issunup = true;
        if (issunup == true)
            System.out.println("DAY");
            
        else 
            System.out.println("NIGHT");
        int day = 1 ;// 1 monday, 2 tuesday 3 wednesday 4 thu-sun
        switch ((day)) {
            case 1:
                System.out.println("Monday");
                // agr iske baad break nhi likha toh ek chiz true hote he neeche ke saare cases print ho jayenge Toh iss liye break laga do 
            case 2:
                System.out.println("Tuesday");
                break;
            case 3:
                System.out.println("Wednesday");
                
                break;
        
            default:
                System.out.println("Thu-Sun");
                break;
            }
        for (int i = 1; i<=5; i++){
            System.out.println(i);
        }
        // for while loop we need to define the variable first
        int a=0;
        while (a<=10){
            System.out.println(a);
            a++;
        }

        // do while 
        int b = 0;
        do{
            System.out.println(b);
            b++;
        }while (b<=7);

        //Exception Handling
        System.out.println(Arrays.toString(marks));
        try{
            System.out.println(marks[6]);//marks only contain 5 elements
        } catch (Exception exception){
            System.out.println("Kuch gadbad hai bhai");
        }
        System.out.println("Hello");


        // METHODS defining a function see lines 8 9
        printjava();
        printjava();
        printjava();
        
    
    }


    }
