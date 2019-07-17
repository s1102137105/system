<?php
    session_start();
    if($_SESSION['id']==null)
    {
        header("Location:login.html");
    }
        else {

    $Receipt_ID=$_POST['Receipt_ID'];
    $username='s1102137116';
    $passwd='S223660940';
    $dsn='mysql:dbname=s1102137116;host=db.mis.kuas.edu.tw;charset=utf8';
    try{
        $conn=new PDO($dsn, $username, $passwd);
        for($i=0;$i<count($Receipt_ID);$i++){
            $sql="DELETE FROM `db_receipt` WHERE `Receipt_ID` = '$Receipt_ID[$i]'";
            $count=$conn->exec($sql);
        }
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
