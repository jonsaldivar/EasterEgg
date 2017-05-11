# EasterEgg
creates an easteregg

/*
*Jonathan Saldivar
*ITSE 1302-011
*EasterEgg
*Basket that holds the eggs. 
*/

import java.util.ArrayList;

public class Basket {
    ArrayList<EasterEgg> aryBasket = new ArrayList<EasterEgg>();

    public void add(EasterEgg objEgg) {
    aryBasket.add(objEgg);
    }
    
    public void drop(EasterEgg objEgg) {
    aryBasket.remove(objEgg);
    }
    
    public String toString() {
    return aryBasket.toString();
    }
}
