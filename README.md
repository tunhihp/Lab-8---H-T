# Lab-8---H-T
import java.util.Scanner;
interface Moveable{
	void moveUp();
	void moveDown();
	void moveLeft();
	void moveRight();
}
class MoveableCircle implements Moveable{
	@Override
	public void moveUp(){
		System.out.println("Up");
	}
	public void moveDown(){
		System.out.println("Down");
	}
	public void moveLeft(){
		System.out.println("Left");
	}
	public void moveRight(){
		System.out.println("Right");
	}
}
public class QQ2{
	public static void main(String[] args){
		MoveableCircle m = new MoveableCircle();
		m.moveUp();
		m.moveDown();
		m.moveLeft();
		m.moveRight();
	}
} // cau 1

interface shape {
    void draw ();
}
class rectangle implements shape {
    @Override
    public void draw (){
        System.out.println(" draw ");
    }
}
class cricle implements shape {
    @Override
    public void draw (){
        System.out.println(" draw ");
    }
}
public class Bai2 {
    public static void main ( String[] args) {
        rectangle r = new rectangle ();
        cricle c = new cricle ();
        r.draw();
        c.draw();
    }
} // cau 2

package BaiTapLab8;
interface car{
    String color();
    double speed();
    void accelerate();
    String getColor();
    double getSpeed();
        
}
class BMW implements car{

    @Override
    public void accelerate() {
        System.out.println("BMW accelerate");
        
    }

    @Override
    public String color() {
        String color;
        color = "Red";
        return "color: "+ color;
    }

    @Override
    public String getColor() {
        String getcolor;
        getcolor = "blue";
        return "getcolor: "+ getcolor ;
    }

    @Override
    public double getSpeed() {
        
        return 200;
    }

    @Override
    public double speed() {
        
        return 100;
    }
    public String toString(){
        accelerate();
        return  "speed: "+ speed()+ "\ngetspeed: "+getSpeed()+ "\n"+ getColor() + "\n"+ color() ;
    }

}
class Civic implements car{

    @Override
    public void accelerate() {
        System.out.println("Civic accelerate");
        
    }

    @Override
    public String color() {
        String color;
        color = "black";
        return "color: "+ color;
    }

    @Override
    public String getColor() {
        String getcolor;
        getcolor = "pink";
        return "getcolor: "+ getcolor ;
    }

    @Override
    public double getSpeed() {
        
        return 300;
    }

    @Override
    public double speed() {
        
        return 200;
    }
    public String toString(){
        accelerate();
        return  "speed: "+ speed()+ "\ngetspeed: "+getSpeed()+ "\n"+ getColor() + "\n"+ color() ;
    }
}  // cau 3

