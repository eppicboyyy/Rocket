# Rocket
Rocket private


public class  RocketLoop{ 
public static final int width = 10;
public static void main(String [] args){ 
cone(); 
border();
top();
bottom();
border();
bottom();
top();
border();
cone();
} 

public static void cone( ) { 
   for(int line=1;line< 2*width;line++){
      for(int space=2*width-line;space>0;space--){
         System.out.print(" "); 
      }
      for(int slash=1;slash<=line;slash++){
         System.out.print("/"); 
      }
      System.out.print("**"); 
      for(int backslash=1;backslash<=line;backslash++){
         System.out.print("\\"); 
      }
      System.out.println(); 
   }
} 

public static void border( ) { 
   System.out.print("+");
   for(int line=1;line<=2*width;line++){
      System.out.print("=*");
   }
   System.out.println("+");
}


public static void top(){
   for(int line=1;line<=width;line++){
       System.out.print("|");
      for (int hi=1;hi<=2;hi++){
         for(int dot=width-line;dot>0;dot--){
            System.out.print(".");
         }
         for(int triangle=line;triangle>0;triangle--){
            System.out.print("/\\");
         }
         for(int dot=width-line;dot>0;dot--){
            System.out.print(".");
         }
      }
      System.out.println("|");
   }
}
public static void bottom(){
   for(int line=width;line>=1;line--){
       System.out.print("|");
      for (int hi=1;hi<=2;hi++){
         for(int dot=width-line;dot>0;dot--){
            System.out.print(".");
         }
         for(int triangle=line;triangle>0;triangle--){
            System.out.print("\\/");
         }
         for(int dot=width-line;dot>0;dot--){
            System.out.print(".");
         }
      }
      System.out.println("|");
   }
}
}
     
