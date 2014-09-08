//By Non, Song
package homework2part1;
 
public class HomeWork2 {
 
	 
	public static void main(String[] args) {
		
		
		String a = "hi, My Name is, Non";
		String b;
		char c = a.charAt(0);
		if(c>96){ 
		
		
		c = (char)(c-32);}
		
		if(c=='a' || c==','){
			c= ' ';
		}
		
		
		a = a.replace(a.charAt(0),' ');
		
	    a = a.replaceAll("a", "");
	b=a.replaceAll(",", "");
		System.out.println(c + changeString(b));
 
	}
 
	public static String changeString(String x) {
		String sentence = "";
		for(int i=1; i<x.length(); i++){
			if (x.charAt(i) == ' '){
				sentence += " " + Character.toString(x.charAt(i+1)).toUpperCase();
				i++;
			}
			else{
				sentence += x.charAt(i);
			}
		}
		
		return sentence;
	}
}
