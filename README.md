# hello-world
Just another repositoey
import java.io.*;
sdsss
public class Demo05 {
    public static void main(String[] args) throws Exception {
        FileWriter f1 = new FileWriter("111-1.text");
        FileReader f2 = new FileReader("111.text");
        while (true) {
            int read = f2.read();
            if(read==-1){
                break;
            }else {
                f1.write(read);
            }
        }
        f1.close();
        f2.close();
        System.out.println("打印完毕！");
        System.out.println("=======================================");
        FileOutputStream f3= new FileOutputStream("111-2.text");
        FileInputStream f4 = new FileInputStream("111.text");
        while (true) {
            int read = f4.read();
            if(read==-1){
                break;
            }else {
                f3.write(read);
            }
        }
        f3.close();
        f4.close();
        System.out.println("打印完毕！");
        System.out.println("============================");
        FileWriter f7 = new FileWriter("111-3.text");
        FileReader f8 = new FileReader("111.text");
        BufferedWriter F5 = new BufferedWriter(f7);
        BufferedReader f6 = new BufferedReader(f8);
        while (true) {
            int read = f8.read();
            if(read==-1){
                break;
            }else {
                f7.write(read);
            }
        }
        f7.close();
        f8.close();
        System.out.println("打印完毕！");
        System.out.println("============================");
        FileOutputStream f9= new FileOutputStream("111-4.text");
        FileInputStream f10 = new FileInputStream("111.text");
        BufferedOutputStream f11 = new BufferedOutputStream(f9);
        BufferedInputStream f12 = new BufferedInputStream(f10);
        while (true) {
            int read = f12.read();
            if(read==-1){
                break;
            }else {
                f11.write(read);
            }
        }
        f11.close();
        f12.close();
        System.out.println("打印完毕！");
    }
