# restuarant-bill
calculates a restaraunt bill



import java.util.Scanner;
public class RestaurantBill
{
    public static void main(String[] args)
    {
        // Name the variables
        double price;       //price of meal
        double tax;         //tax on meal
        double tip;         // tip amount
        double total;       //total amount owed

        Scanner keyboard = new Scanner(System.in);


        // Prompt the user to enter charge for meal
        System.out.print("What is the price of your meal? "
                            + "$");
        price = keyboard.nextDouble();

        //Calculations
        tax = price * .0675;
        tip = (tax + price) * .2;
        total = price + tax + tip;

        System.out.println("The Meal price is $"
                            +  price );
        System.out.println("Tax on your bill is $"
                            + tax );
        System.out.println("The amount you should tip is $"
                            + tip );
        System.out.println("The total bill is $"
                            + total );
    }

}
