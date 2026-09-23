<html>
<body>
<form method="post">
Enter Birth Year: <input type="text" name="year">
<input type="submit" value="Calculate">
</form>

<?php
if(isset($_POST['year'])){
    $age = date("Y") - $_POST['year'];
    $remain = 60 - $age;

    echo "Age: $age years<br>";
    echo "Years for Retirement: ".max(0,$remain);
}
?>
</body>
</html>


output:
Employee Age and Retirement Calculator

Enter Birth Year: 2004
[ Calculate ]

Age: 22 years
Years for Retirement: 38
