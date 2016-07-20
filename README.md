# convert
public class Convert {
	

		String reverse(String source) {
			if (source == null || source.isEmpty()) {
				return source;
			}
			String rever = "";
			for (int i = source.length() - 1; i >= 0; i--) {
				rever += source.charAt(i);
			}
			return rever;
		}

		public static void main (String[] args)

		{
			Convert obj = new Convert();
			
			String input1 = "Wipro Technologies, Bangalore";

			String[] parts = input1.split(" ");

			String part = " ";

			for (int i = 0; i < parts.length; i++) {
				part = part + " " + obj.reverse(parts[i]);
			}
			String output1 = part.trim();
			System.out.println(output1);


}
}
