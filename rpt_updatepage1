<?php
    session_start();
    if($_SESSION['id']==null)
    {
        header("Location:login.html");
    }
        else {
    $Receipt_ID=$_POST['Receipt_ID'];
    $Receipt_Project=$_POST['Receipt_Project'];
    $Receipt_Money=$_POST['Receipt_Money'];
    $Receipt_Date=$_POST['Receipt_Date'];
    $Employee_ID=$_POST['Employee_ID'];
    $Student_Name=$_POST['Student_Name'];
    $username='s1102137116';
    $passwd='S223660940';
    $dsn='mysql:dbname=s1102137116;host=db.mis.kuas.edu.tw;charset=utf8';
    try{
        $conn=new PDO($dsn, $username, $passwd);
        $sql="SELECT `Student_ID` FROM `db_student` WHERE `Student_Name`='$Student_Name'";
        $stmt=$conn->query($sql);
        foreach ($stmt ->fetchAll(PDO::FETCH_ASSOC) as $row) {
            $Student_ID=$row['Student_ID'];
        }
        
        $sql1="UPDATE `db_receipt` SET `Stu_ID`='$Student_ID',`Emp_ID`='$Employee_ID',`Receipt_Project`='$Receipt_Project',`Receipt_Money`='$Receipt_Money',`Receipt_Date`='$Receipt_Date' WHERE `Receipt_ID`='$Receipt_ID'";
        $stmt=$conn->query($sql1);
    }  catch (Exception $ex){
        echo $ex->getMessage();
    }
?>
<!DOCTYPE html> 
<html lang="zh-tw">
    <head>
        <meta http-equiv="refresh" content="0;url=http://fs.mis.kuas.edu.tw/~s1102137148/sys/receipt.php" />
    </head>
<body>
    <?php
        if($_SESSION['position']!="總務"  &&  $_SESSION['position']!="管理者" && $_SESSION['position']!="會計")
        {
            echo "你的權限不足無法瀏覽";
        }
        else{
?>
</body>
</html>
<?php }?> <?php }?>
