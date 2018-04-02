# Greatest
import java.util.*;
public class Greatest {
    public static void main(String[]args){
        Scanner in = new Scanner(System.in);
        int input1 = in.nextInt(); /// 7.รับ input เข้ามาสองตัว คือ input1  เเละ input2
        int input2 = in.nextInt();
            Greatest gr =new Greatest();/// 8.สร้าง object gr
           gr.printGcd(input1, input2); //9.เรียกใช้เมธอด printGrd เพื่อเเสดงผลออกมา 
        // System.out.println(gr.re(input1,input2));   
    }
   public void printGcd(int input1,int input2){ /// 4.สร้างเมธอดเพื่อรับค่ามาสองค่า เพื่อส่งไปแแสดงผลใน main
        int greatest=0;
        if(input1>0 && input2>0){ ///// 5.เช็คว่า input1 เเละ input2 ที่รับเข้ามามากกว่า 0  หรือไม่ 
     /*   while(input2>0){
            greatest=input1%input2;
            input1=input2;
            input2=greatest;
        }*/
        System.out.println("greatest common divisor "+reGcd(input1,input2));//// ถ้ามากกว่าก็จะเเสดงค่า ห.ร.ม ออกมาโดยไปเรียกใช้ฟังก์ชัน reGcd
   }else{
            System.err.println("Please check input > 0"); //// 6.ถ้าน้อยกว่า 0 ทำการเเสดงผล Error ว่า lease check input > 0
        }
   }  
       public int reGcd(int input1,int input2) {    ///// 1.สร้างฟังก์ชันรีเคอซีฟ ชื่อ re ที่รับค่า input1,input2 เข้ามา
             if(input2>0){   ///// 2.ทำการสลับตำเเหน่งให้ตำเเหน่งที่ input1=input2 และทำการ นำ input1%input2
                 return reGcd(input2,input1%input2); ///// จนกว่า ค่า input2 จะเท่ากับ 0 ก็จะได้คำตอบสุดท้ายคือ (input2,0)=input2
        }
                 else{
                     return input1; //// 3.ถ้ามันไม่มากกว่า 0 ก็ให้รีเทรินอะไรออกมาก็ได้ เพราะถ้าเข้าเงื่อนไขนี้ 
                     /////จะไปเช็คเงื่อนไขใน method printGcd อีกครั้งหนึ่งว่าตัวเลขที่รับเข้ามากมาก 0 หรือไม่
     }
     
}
   
   
   
   
   
   
   
   
   
   
   
   
}
    
    
