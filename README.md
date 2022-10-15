# Java-coding


Write a simple Java program that consists of the followings:
3 attributes, 2 constructors (default, normal), setters, getters, 1 method.
Attached your answer here with screenshot of output. Please refer to your answer in previous question.



The Output : 


![2022-10-13](https://user-images.githubusercontent.com/109582424/195994346-402055c6-0909-4e13-83f5-ca29cfb268e0.png)











public class AlarmClock
{
   
    private String brand;
    private String color;
    private int price;

    public AlarmClock()
    {
         brand = "";
         color = "";
         price = 0;
    }
    
    public AlarmClock(String b ,String c, int p)
    {
        brand = b;
        color = c;
        price = p;
    }
    //copy constructor 
    public AlarmClock(AlarmClock a)
    {
      this.brand = a.brand;
      this.color = a.color;
      this.price = a.price;
    }
    
   //setters
   public void setAlarmClock (String brand ,String color ,int price)
  {
      brand = brand;
      color = color;
      price = price;
     
  }
//getters
public String getBrand() {return brand;}
public String getColor() {return color;}
public int getPrice() {return price;}

public String toString()
{
    return ("\n Brand :" +brand +"\n Color:"+color + "\n price:"+price ); 
}
}










IN MAIN 

public class AlarmClockTest
{
     public static void main (String [] args)
    {
        AlarmClock c = new AlarmClock ();
        AlarmClock c1 = new AlarmClock ("Casio","RED",50);
        
        System.out.println (c1.toString());
    }
}
