# YYS
a model of "yunhun"(a kind of equipment)in this game. 
package yys;

import java.util.Random;
import java.util.Scanner;

public class yuhun {
	public static void main(String[] args) {
		Scanner in=new Scanner(System.in);
		int input=in.nextInt();//御魂强化次数
		in.close();
		String type=null;
	    int max7=3;
	    int min7=1;
	        Random random7 = new Random();
	    int r7 = random7.nextInt(max7)%(max7-min7+1) + min7;/*御魂副属性条数*/
		for(int i=1;i<r7+1;i++) {
		int max1=3;
	    int min1=2;
	        Random random1 = new Random();
	    int r1 = random1.nextInt(max1)%(max1-min1+1) + min1;/*2-3的随机数(生命加成，攻击加成，防御加成，暴击，速度)*/
	    int max2=4;
	    int min2=3;
	        Random random2 = new Random();
	    int r2 = random2.nextInt(max2)%(max2-min2+1) + min2;/*3-4的随机数(暴击伤害，效果命中，效果抵抗)*/
	    int max3=30;
	    int min3=25;
	        Random random3 = new Random();
	    int r3 = random3.nextInt(max3)%(max3-min3+1) + min3;/*25-30的随机数(攻击)*/
	    int max4=5;
	    int min4=4;
	        Random random4 = new Random();
	    int r4 = random4.nextInt(max4)%(max4-min4+1) + min4;/*4-5的随机数(防御)*/
	    int max5=110;
	    int min5=90;
	        Random random5 = new Random();
	    int r5 = random5.nextInt(max5)%(max5-min5+1) + min5;/*90-110(生命)*/
	    int max6=11;
	    int min6=1;
	        Random random6 = new Random();
	    int r6 = random6.nextInt(max6)%(max6-min6+1) + min6;/*11种御魂种类随机*/
	    if(r6==1) {
		  type="生命加成";
		  System.out.println(type+" "+r1*input+"%");
	   }else if
	   	 (r6==2) {
		  type="攻击加成";	
		  System.out.println(type+" "+r1*input+"%");
		   }else if
	   	 (r6==3) {
		  type="防御加成";	
		  System.out.println(type+" "+r1*input+"%");
		   }else if
	   	 (r6==4) {
		  type="暴击";	 
		  System.out.println(type+" "+r1*input+"%");
		   }else if
	   	 (r6==5) {
		  type="速度";	
		  System.out.println(type+" "+r1*input);
		   }else if
	   	 (r6==6) {
		  type="暴击伤害";	
		  System.out.println(type+" "+r2*input+"%");
		   }else if
	   	 (r6==7) {
		  type="效果命中";	
		  System.out.println(type+" "+r2*input+"%");
	       }else if
	   	 (r6==8) {
		  type="效果抵抗";	
		  System.out.println(type+" "+r2*input+"%");
           }else if
	   	 (r6==9) {
		  type="攻击";	
		  System.out.println(type+" "+r3*input);
           }else if
		 (r6==10) {
		  type="防御";	
		  System.out.println(type+" "+r4*input);
           }else if
		 (r6==11) {
     	  type="生命";	
     		  System.out.println(type+" "+r5*input);
           }
	   }
	}
}
