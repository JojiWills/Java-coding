# Java-coding

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
