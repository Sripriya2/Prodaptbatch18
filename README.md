# Prodaptbatch18

*********** index.jsp **********

<%@ page language="java" contentType="text/html; charset=ISO-8859-1"
	pageEncoding="ISO-8859-1"%>
<!DOCTYPE html>
<html>
<head>
<meta charset="ISO-8859-1">
<title>Insert title here</title>
</head>
<body style="background-color: black; color: Gold">
	<center>
		<form action="ValidatePswd.jsp" method="get">
			<br>
			<br>
			<h1>Login Page</h1>
			<br>
			<br>
			<div>
				Enter UserName: <input type="text" name="Username"><br>
				<br>
			</div>
			Enter Password: <input type="password" name="Password"><br>
			<br> <input type="submit">
		</form>
	</center>
</body>
</html>


*********** ValidatePswd.jsp **********
<%@ page language="java" contentType="text/html; charset=ISO-8859-1"
	pageEncoding="ISO-8859-1"%>
<!DOCTYPE html>
<html>
<head>
<meta charset="ISO-8859-1">
<title>Insert title here</title>
</head>
<body>
	<%
	String uname=request.getParameter("Username");
	String pswd=request.getParameter("Password");
	/* out.println(pswd); */
	if(pswd.equals("12345")) {
		out.println("<h1>Your a Valid User</h1>");
	}else {
		out.println("<h1>Your not a Valid User</h1>");
	}
	
	%>
</body>
</html>
