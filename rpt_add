<?php
    session_start();
    if($_SESSION['id']==null)
    {
        header("Location:login.html");
    }
        else {
    $username='s1102137116';
    $passwd='S223660940';
    $dsn='mysql:dbname=s1102137116;host=db.mis.kuas.edu.tw;charset=utf8';
    try{
        $conn=new PDO($dsn, $username, $passwd);
        $sql1="SELECT * FROM `db_employee`";
        $stmt1=$conn->query($sql1);
        $sql2="SELECT * FROM `db_student`";
        $stmt2=$conn->query($sql2);
    }  catch (Exception $ex){
        echo $ex->getMessage();
    }
?>
<!DOCTYPE html> 
<html lang="zh-tw">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>收據 | 補習班管理系統</title>
    <!-- css no delete -->
    <link rel='stylesheet' id='all-css-0' href='https://s1.wp.com/_static/??-eJx9jlEOwiAQRC8korbBL+NZEFaE7rKkQIi3lzYxxmj6t7N5LzOyJWE4FohFUhUJq/Mxy0we4ZlmDmDKd9qbnHfyv4Z+giwDlKTNJNb0g9+Q3Udg58ByLeLOiNxk89bBZofhGfqfki4LQWC9BgTq2JZGSb2t5Xz0geu2K12O43AYlDqN5/ACNydlMA==' type='text/css' media='all' />
    <link rel='stylesheet' id='hemingway-rewritten-raleway-css'  href='https://fonts.googleapis.com/css?family=Raleway%3A400%2C300%2C700&#038;ver=4.2-RC4-32277' type='text/css' media='all' />
    <link rel='stylesheet' id='hemingway-rewritten-latos-css'  href='https://fonts.googleapis.com/css?family=Lato%3A400%2C700%2C400italic%2C700italic&#038;subset=latin%2Clatin-ext&#038;ver=4.2-RC4-32277' type='text/css' media='all' />
    <link rel='stylesheet' id='all-css-4' href='https://s2.wp.com/_static/??-eJyFjuEKwjAMhF/IGoYb+Ed8lq3EmtEmpc0oe/tVijAR55/wHXfHBUo0VliRFfSJATPEZYJKxK6Mq0lYEmn1Ievq8WxzPsGuFBYT/eKIMzhkTFSNH/jV/TNIbNuoKdFKOJrGIDO122IELNoeeMPx62K82FFJ+EOYhx8pHVUTTl5cRQc1tZOv0j3cuv7SDf0wXPt5AwQ9iZg=' type='text/css' media='all' />
    <link rel='stylesheet' id='print-css-5' href='https://s0.wp.com/wp-content/mu-plugins/global-print/global-print.css?m=1387483371g' type='text/css' media='print' />
    <link rel='stylesheet' id='all-css-6' href='https://s0.wp.com/wp-content/themes/h4/global.css?m=1420737423g' type='text/css' media='all' />
    <!-- css no delete -->
    <!-- bannerpicture no delete -->
    <style type="text/css">
        .site-title a,.site-description 
        {
            color: #ffffff;
        }
        .site-header-image 
        {
            background-image: url(http://img.taopic.com/uploads/allimg/110209/1716-1102091F04092.jpg);
        }
    </style>
    <!-- bannerpicture no delete -->
    <style type="text/css" id="syntaxhighlighteranchor"></style>
    <SCRIPT type="text/javascript">
        function check()
        {
            var rdate=document.a.Receipt_Date.value;
            var DateStamp = new Date();
            var now = DateStamp.getFullYear() + "/" + (DateStamp.getMonth() +1) + "/" + (DateStamp.getDate()+1);
            if(Date.parse(rdate)>Date.parse(now))
            {
                alert("收據日期有誤，請重新輸入");
                return false;
            }
        }
</SCRIPT>
</head>


<body class="page page-id-27 page-template-default mp6 customizer-styles-applied one-column highlander-enabled highlander-light">
    
    <div id="page" class="hfeed site">
			<header id="masthead" class="site-header" role="banner">
		<div class="site-header-image">
			<div class="site-branding-wrapper">
				<div class="site-branding">
					<h1 class="site-title"><a href="http://fs.mis.kuas.edu.tw/~s1102137148/sys/home.php" rel="home">補習班管理系統</a></h1>
					<h2 class="site-description">某一補習班</h2>
				</div>
			</div>
		</div>
	</header><!-- #masthead -->
	<nav id="site-navigation" class="main-navigation clear" role="navigation">
		<h1 class="menu-toggle" title="選單"><span class="screen-reader-text">選單</span></h1>
		<a class="skip-link screen-reader-text" href="#content">Skip to content</a>

		<div><ul  class="menu"><li id="menu-item-22" class="menu-item menu-item-type-post_type menu-item-object-page current-menu-item page_item page-item-17 current_page_item menu-item-22"><a href="http://fs.mis.kuas.edu.tw/~s1102137148/sys/home.php">首頁</a></li>
<li id="menu-item-23" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-has-children menu-item-23"><a>基本資料</a>
<ul class="sub-menu">
	<li id="menu-item-24" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-24"><a href="http://fs.mis.kuas.edu.tw/~s1102137148/sys/personal.php">個人資料</a></li>
	<li id="menu-item-33" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-33"><a href="http://fs.mis.kuas.edu.tw/~s1102137148/sys/student.php">學生資料</a></li>
	<li id="menu-item-34" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-34"><a href="http://fs.mis.kuas.edu.tw/~s1102137148/sys/teacher.php">老師資料</a></li>
	<li id="menu-item-35" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-35"><a href="http://fs.mis.kuas.edu.tw/~s1102137148/sys/employee.php">員工資料</a></li>

</ul>
</li>
<li id="menu-item-46" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-has-children menu-item-46"><a>設備管理</a>
<ul class="sub-menu">
	<li id="menu-item-43" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-43"><a href="http://fs.mis.kuas.edu.tw/~s1102137148/sys/maintain.php">設備報修總表</a></li>
	<li id="menu-item-44" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-44"><a href="http://fs.mis.kuas.edu.tw/~s1102137148/sys/stationery.php">文具總表</a></li>
	<li id="menu-item-45" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-45"><a href="http://fs.mis.kuas.edu.tw/~s1102137148/sys/Equipment.php">設備總表</a></li>
</ul>
</li>
<li id="menu-item-53" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-has-children menu-item-53"><a>財務管理</a>
<ul class="sub-menu">
	<li id="menu-item-51" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-51"><a href="http://fs.mis.kuas.edu.tw/~s1102137148/sys/receipt.php">收據</a></li>
	<li id="menu-item-52" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-52"><a href="http://fs.mis.kuas.edu.tw/~s1102137148/sys/expenditure.php">支出</a></li>
</ul>
</li>

<li id="menu-item-99" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-has-children menu-item-99"><a>員工記錄</a>
<ul class="sub-menu">
	<li id="menu-item-97" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-97"><a href="http://fs.mis.kuas.edu.tw/~s1102137148/sys/rotationrecord.php">輪調記錄</a></li>
	<li id="menu-item-98" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-98"><a href="http://fs.mis.kuas.edu.tw/~s1102137148/sys/workrecord.php">任職記錄</a></li>
</ul>
</li>
<li id="menu-item-102" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-102"><a href="http://fs.mis.kuas.edu.tw/~s1102137148/sys/course.php">課程管理</a></li>
<li id="menu-item-100" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-100"><a href="http://fs.mis.kuas.edu.tw/~s1102137148/sys/repairorders.php">報修單</a></li>

</ul></div><li id="menu-item-101" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-101"><a href="http://fs.mis.kuas.edu.tw/~s1102137148/sys/logout.php">登出</a></li>
	</nav><!-- #site-navigation -->
        
	<div id="content" class="site-content">

	<!--<div id="primary" class="content-area">
		<main id="main" class="site-main" role="main">-->
        
<article id="post-25" class="post-25 page type-page status-publish hentry">
    <!-- <div align="right">
        <form action="stu_search.php" method="POST">
            <select name="search">
                <option value="Class_Name">班級</option>
                <option value="Student_Name">姓名</option>
                <option value="Student_Phone">電話</option>
                <option value="Student_Cellphone">手機</option>
                <option value="Student_Address">地址</option>
                <option value="Student_Birthday">生日</option>
                <option value="Student_School">學校</option>
                <option value="Student_Major">科系</option>
                <option value="Guardian_Name">監護人</option>
                <option value="Guardian_Cellphone">監護人電話</option>
            </select>
            <input type="text" name="searchtext"/>
            <input type="submit" value="查詢"/><br>
        </form>
    </div>-->
	<header class="entry-header">
		<h1 class="entry-title">收據</h1>	</header><!-- .entry-header -->

	<div class="entry-content">
		<p></p>
               <div align="right">
                    <select onchange="location.href=this.options[this.selectedIndex].value">
                    <option>動作選單</option>
                    <option value="http://fs.mis.kuas.edu.tw/~s1102137148/sys/receipt.php" >瀏覽</option>
                    <option value="http://fs.mis.kuas.edu.tw/~s1102137148/sys/rpt_add.php" >新增</option>
                    <option value="http://fs.mis.kuas.edu.tw/~s1102137148/sys/rpt_del.php" >刪除</option>
                    <option value="http://fs.mis.kuas.edu.tw/~s1102137148/sys/rpt_update.php">修改</option>
                    </select>
               </div><br>
                <?php
        if($_SESSION['position']!="總務"  &&  $_SESSION['position']!="管理者" && $_SESSION['position']!="會計")
        {
            echo "你的權限不足無法瀏覽";
        }
        else{
?>
                <form action="rpt_addpage.php " method="post" name="a" onsubmit="return check()">
        <table>
            <tr>
                <td>項目  <font color="red">*</font></td>
                <td><input type="text" name="Receipt_Project" required/></td>
            </tr>
            <tr>
                <td>金額  <font color="red">*</font></td>
                <td><input type="text" name="Receipt_Money" required/></td>
            </tr>
            <tr>
                <td>日期  <font color="red">*</font></td>
                <td><input type="date" name="Receipt_Date" required /></td>
            </tr>
            <tr>
                <td>收款人  <font color="red">*</font></td>
                <td>
                    <select name="Employee_ID" required>
                        <option hidden></option><?php foreach ($stmt1 ->fetchAll(PDO::FETCH_ASSOC) as $row1) { ?>
                        <option><?php echo $row1['Employee_ID']; echo $row1['Employee_Name'];?></option><?php } ?>
                    </select></td>
            </tr>
            <tr>
                <td>繳款人  <font color="red">*</font></td>
                <td>
                    <select name="Student_Name" required>
                        <option hidden></option><?php foreach ($stmt2 ->fetchAll(PDO::FETCH_ASSOC) as $row2) { ?>
                        <option><?php  echo $row2['Student_Name'];?></option><?php } ?>
                    </select>
                </td>
            </tr>
        </table>  
        <div align="right">
        <input type="submit" value="送出"/>
        <input type="reset" value="清除"/>
        </div> 
        </form>
                
        </div><!-- .entry-content -->
	</article><!-- #post-## -->			
	</main><!-- #main -->
	</div><!-- #primary -->
	</div><!-- #content -->
	<footer id="colophon" class="site-footer" role="contentinfo">
	<div class="site-info">	四資二甲-某一補習班 | 補習班管理系統</div><!-- .site-info -->
	</footer><!-- #colophon -->
</div><!-- #page -->
</body>
</html>
<?php }?> <?php }?>
