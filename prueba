package Main;

import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.ResultSet;
import java.sql.Statement;

public class Main {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

		Connection con = null;
		Statement st = null;
		ResultSet rs = null;
		try
		{
			String driverClassName = "com.mysql.jdbc.Driver";
			String driverUrl = "jdbc:mysql://localhost/curso";
			String user = "root";
			String password = "1111";
			Class.forName(driverClassName);
			con = DriverManager.getConnection(driverUrl,user,password);
			st = con.createStatement();
			String query = "SELECT * FROM alumnos";
			rs = st.executeQuery(query);
			
			while(rs.next()) {
				System.out.println("Col1: " + rs.getString(4));
			}
		}
		catch (Exception a){
			System.out.println("error es " +a.getMessage());
		}
		
	
	}
	
