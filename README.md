class Mythread68 extends Thread {
public void run() {
    System.out.println(10/0);
        for (int i = 0; i < 10; i++) {
        System.out.println("mythread" + i);
        }
        }
        }
public class multithr02 {
    public static void main(String[] args) {
        Mythread68 obj = new Mythread68();
        Thread obj1= Thread.currentThread();
        obj1.setPriority(Thread.MAX_PRIORITY);
        System.out.println(obj1.getPriority());
        obj1.setName("sharmaji");
        System.out.println(obj1.isAlive());
        System.out.println(obj1.isDaemon());
        System.out.println(10/0);
        obj.start();
        for(int i=0;i<10;i++){
            System.out.println("my"+i);
        }


    }
}


