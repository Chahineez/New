# GitTP
package Vect;
import java.util.Scanner;


/**
 * @author sara
 * Binome : Mehenni/Slatnia
 * TP : Module IGL SARA

 */

public class VectorHelper {
	
	public int vect[] = new int[10];
	
	
	
	
	/************************METHODE TRIER_VECT***********************************/
	
	 
	/**
	 *  VectorHelpere() est un constructeur sans parametre qui donne des valeurs a notre tableau 2
	 */
	
	public VectorHelper(){
		 this.vect[0]=5;
		 this.vect[1]=6;
		 this.vect[2]=2;
	     this.vect[3]=3;
	     this.vect[4]=15;
	     this.vect[5]=4;
		 this.vect[6]=8;
	     this.vect[7]=9;
		 this.vect[8]=7;
		 this.vect[9]=12;
		
	}
	/**
	 * cette methode  permet de trier un vecteur en ordre croissant
	 *  de ses elements et retourne le tableau trié
	 */
	public void Trier_Vect(){
		
		int i=0;
		
	    int x;
	    
		
	    
	             while( i< vect.length-1){
      	    	
	    
	                   if (vect[i]> vect[i+1]) { 
	    
	                     x=vect[i];  //PERMUTATION DES DEUX CASES
	    		         vect[i]= vect[i+1];
	    		         vect[i+1]=x;
	    		         i=0;
	    	                                   }
	                   else {i++;}
	  
	    
	                                      }
		
		
                         	}

	/*************************************METHODE MAXMIN***********************************/
	
	/**
	 * cette methode  permet de donner le maximum d'un tableau ainsi que son minimum en meme temps 
	 */
	
	/**
	 * @return
	 */
	/**
	 * @param max representera le maximum de notre tableau
	 * @param min representera le minimum de notre tableau
	 * @return de  plus du message affichant simultanément le max et le min on retourne la somme de ces 2 derniers pour
	 *  les testes
	 */
	public int  MaxMin(int max,int min){
		
		
	
	int k=1; int l=1;	
	max=vect[0];
	min=vect[0];
	
   while(k<vect.length & l < vect.length){
	  
	   if(vect[k]>=  max){
		   max= vect[k];
		   k++;
	   }
	   else{k++;}
	   if(vect[l]<= min){
		   min= vect[l];
		   l++;
	   }else{l++;}
	   
	   
	   
   }
	System.out.println(" valeurrrr du maximumm est "+max);	
	System.out.println(" valeurrrr du minimum   est "+min);	
	return max+min;

	
	
		
	}
	
	
	
	
	
	
	
	
	
	

                          }
