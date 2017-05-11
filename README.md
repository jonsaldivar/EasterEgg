# EasterEgg
creates an easteregg

/*
*Jonathan Saldivar
*ITSE 1302-011
*EasterEgg*pregenerated egg shells that the pattern changes.
*/

public class EasterEgg {

   private char chrOutput = '*';
   private static int intEggCount = 1;
   public EasterEgg(){
   UserInput();
   intEggCount++;
   }
   
   private void UserInput(){
   Scanner objInput = new Scanner(System.in);
   System.out.println("Add a character: ");
   setSymbol(objInput.next().charAt(0));
   }
   
   public int EggCounter(){
   return intEggCount - 1;
   }
   
   private char getSymbol(){
   return chrOutput;
   }
   
   private void setSymbol(char pchrOutput){
   chrOutput = pchrOutput;
   }
   
   public String toString(){
   return
   (" /" + getSymbol() + getSymbol() + "\\ \n" +
   "/" + getSymbol()  + getSymbol()  + getSymbol()  + getSymbol()  + "\\ \n" +
   "|" + getSymbol() + getSymbol() + getSymbol() + getSymbol() + "|  \n" +    "\\____/ \n\n");
   }
}
