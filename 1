<?php 


date_default_timezone_set("Asia/Kolkata");
include("../db_inc1.php");//database connection
session_start();


setcookie("PHPSESSID","",time()-3600,"","",TRUE,TRUE);


$_SESSION['csrf'] = md5(uniqid(rand(), TRUE));
$key=$_SESSION['csrf'];
$_SESSION['user'];
$_SESSION['location'];
$leveladd=$_SESSION['level_level'];
$localadmin=$_SESSION['localadmin'];
$main_id=$_SESSION['main_id'];
$schemas=htmlspecialchars($_SESSION['schema_name']);
$userid=$_SESSION['id'];

// This code not use next time .......	Schema session create Hear....


if($_SESSION['user'] == '' and $_SESSION['location'] =='')
{
echo "Access Problem....."; 
header("Location: ../login.php");
die();
}

$_SESSION['menuaccess_codeall'];
if($_SESSION['menuaccess_codeall'] =='')
{
	echo "You Are Not Access This Page......";
	die();
}



setcookie("PHPSESSID","",time()-3600,"","",TRUE,TRUE);


$_SESSION['csrf'] = md5(uniqid(rand(), TRUE));
$key=$_SESSION['csrf'];

// At the top of the page we check to see whether the user is logged in or not
if(empty($_SESSION['user']) and $_SESSION['location']=='')
{
	die("redirecting to login.php");
}
?>
<?php include_once("../_layout/_allmenu.php")?>
<script language="javascript">
 
 function pageRefesh(){
	  with(document.frm){
		  action="agewise_report.php";
		  submit();
	  }
  }
  
function valided() {

			if(schemas.options[schemas.selectedIndex].value =='0')
 				{
 			alert("Please Select DRAT !");
 			schemas.focus();
			return false;
 				
  				}

			if(schemaname.options[schemaname.selectedIndex].value =='0')
 				{
 			alert("Please Select DRT !");
 			schemaname.focus();
			return false;
 				
  				}
		
		 if(case_type.options[case_type.selectedIndex].value =='0')
 				{
 			alert("Please Select Case Type !");
 			case_type.focus();
			return false;
 				}
			
}



    function isNumberKey(evt)
    {
       var charCode = (evt.which) ? evt.which : event.keyCode
       if (charCode > 31 &&(charCode < 48 || charCode > 57))
          return false;
       
       return true;
    }
    
</script>
       <script type="text/javascript">
var alpha = "[ A-Za-z]";
var numeric = "[0-9]"; 
var alphanumeric = "[ A-Za-z0-9]"; 

function onKeyValidate(e,charVal){
    var keynum;
    var keyChars = /[\x00\x08]/;
    
    var validChars = new RegExp(charVal);
    if(window.event)
    {
        keynum = e.keyCode;
    }
    else if(e.which)
    {
        keynum = e.which;
    }
    var keychar = String.fromCharCode(keynum);
    if (!validChars.test(keychar) && !keyChars.test(keychar))  
         {
        return false
    } else{
        return keychar;
    }
    
    
	
}

    </script>



<!-- All DRt name -->

<h4 class="text-center">
<b>Age-wise Pending OA/SA Cases (Yearly)</b><br/>
  <small class="text-muted text-sm">Fields
        marked as <span class="text-danger">*</span> are mandatory</small>
</h4>
<hr/>

  <!-- Tab panes -->
  	
	<br><br> <div  class="content_resize" style="height:100%;" >
<div style="margin-left:200px;">
				<form method="post"  name="frm" action="./agewise_report.php" onSubmit="return valided();">
		
				<table width="100%" class="table table-bordered table-condensed" cellpadding="1" cellspacing="1">
				<?php if($userid=="31" or $userid=='1458' or $userid=='1465' or $userid=='1467' or $userid=='1468' or $userid=='1469') {?>
				 <tr><td colspan="2">
				 <?php $schemas = isset($_REQUEST['schemas']) ? $_REQUEST['schemas'] :''; ?>

<label><font color="red">*</font>Select DRAT :</label>
<select name="schemas" id="schemas" class="form-control form-control-sm" onChange="return pageRefesh();">
<?php if($userid=="31"){ ?>
<option value="0">SELECT DRAT NAME</option>  
<option value="1" <?php if($schemas=="1") {?> selected <?php } ?>>ALL</option>        
                        <?php
          
            $st = $db->prepare("select DISTINCT(ms.drat_id),i.name from master_schema ms,initilization as i where ms.schema_id=i.schema_id and i.display='T' and i.schema_id > '99' order by name");
            //$st->bindParam(1, $schema_idrun, PDO::PARAM_STR);
			}
		  else if ($userid=='1458' or $userid=='1465' or $userid=='1467' or $userid=='1468' or $userid=='1469'){
			  		$schemaname = $db->prepare("select schema_id from users where id='$userid'");
					$schemaname->execute();
					$scid = $schemaname->fetchColumn();	
	
			  $st = $db->prepare("select DISTINCT(ms.drat_id),i.name from master_schema ms,initilization as i where ms.schema_id=i.schema_id and i.display='T' and i.schema_id = '$scid' order by name");
		  }
            $st->execute();
            while ($row = $st->fetch(PDO::FETCH_ASSOC,PDO::FETCH_ORI_NEXT))
            {
                   
            		$c_type = htmlspecialchars($row['drat_id']);
            		$short_name = htmlspecialchars(ucwords($row['name']));
            		$short_name = htmlspecialchars(ucwords(strtoupper($short_name)));
 			if($schemas == $c_type )
                {
		print "<option value=".htmlspecialchars($row['drat_id'])." selected>".htmlspecialchars(ucwords(strtoupper($short_name)))."</option>";
                }
           else
                {
                print "<option value=".htmlspecialchars($row['drat_id']).">".htmlspecialchars(ucwords(strtoupper($short_name)))."</option>";
		}
            }
         
            ?></select>
            </td></tr>
			<?php if ($userid=='1458' or $userid=='1465' or $userid=='1467' or $userid=='1468' or $userid=='1469') {$schemas=$c_type;} ?>
			<tr><td colspan="2"><?php if($schemas!='1'){ ?>
						<label><font color="#FF0000">*</font>Select DRT :</label>
				
				<?php  $schemaname = isset($_REQUEST['schemaname']) ? $_REQUEST['schemaname'] :'';?>														
				<select name ="schemaname" class="form-control form-control-sm"  id="schemaname">
				<option value="0">PLEASE SELECT DRT NAME :</option>
				<option value="222" <?php if($schemaname=="222") {?> selected <?php } ?>>ALL</option>								<?php
								if($schemas > 0)
									{
								$sql="select a.schema_id,a.schema_name,b.name,a.drat_id from master_schema as a,initilization as b
								where a.display='Y' and a.schema_id=b.schema_id and a.schema_id!='$schemas' and a.drat_id = '$schemas' order by name";
								$schemaName = $db -> prepare($sql);
								$schemaName -> execute();
								while ($row =$schemaName->fetch(PDO::FETCH_ASSOC, PDO::FETCH_ORI_NEXT))
								{
									
								$ctc=$row['schema_id'];
								if($schemaname == $ctc)
								{
			print "<option value=".htmlspecialchars($row['schema_id'])." selected>".htmlspecialchars($row['name'])."</option>";
								}
								else
								{
			print "<option value=".htmlspecialchars($row['schema_id']).">".htmlspecialchars($row['name'])."</option>";
								}
								
								}
								}
								
								?>	
								
		      </select>	
					<?php } ?>
				 </td></tr><?php }?>
				  <?php if($userid=='1458' or $userid=='1465' or $userid=='1467' or $userid=='1468' or $userid=='1469') { } elseif($userid!="31") {
				 //echo $schemas;
				
				 ?>
				 <tr><td colspan="2">
						<label><font color="#FF0000">*</font>DRT NAME :</label>
				
				<?php  $schemaname = isset($_REQUEST['schemaname']) ? $_REQUEST['schemaname'] :'';?>														
				<select name ="schemaname" class="form-control form-control-sm"  id="schemaname">
															                            <?php
								
								$sql="select a.schema_id,a.schema_name,b.name,a.drat_id from master_schema as a,initilization as b
								where a.display='Y' and a.schema_id=b.schema_id and a.schema_name='$schemas' order by NAME";
								$schemaName = $db -> prepare($sql);
								$schemaName -> execute();
								while ($row =$schemaName->fetch(PDO::FETCH_ASSOC, PDO::FETCH_ORI_NEXT))
								{
									
								$ctc=$row['schema_id'];
								if($schemaname == $ctc)
								{
			print "<option value=".htmlspecialchars($row['schema_id'])." selected>".htmlspecialchars($row['name'])."</option>";
								}
								else
								{
			print "<option value=".htmlspecialchars($row['schema_id']).">".htmlspecialchars($row['name'])."</option>";
								}
								
								}
								
								
								?>	
								
		      </select>	
					
				 </td></tr>
				 <?php }?>
				
			<tr><td colspan="2">
			<?php  $date_type = isset($_REQUEST['date_type']) ? $_REQUEST['date_type'] :'';?>
			
				<label><font color="#FF0000">*</font>Select Report Type:</label>		
				<select name="date_type" id="date_type" class="form-control form-control-sm">
				<option value="0">Select</option>
				<option value="11" <?php if($date_type=="11") {?> selected <?php } ?>>Report With Diary No.</option>
				<option value="22" <?php if($date_type=="22") {?> selected <?php } ?>>Report With Case Registration No.</option>
				</select>
				
			</td></tr>
			
				<tr><td>
				<?php  $annualy = isset($_REQUEST['annualy']) ? $_REQUEST['annualy'] :'';?>

					<label><font color="#FF0000">*</font>Select Financial Year:</label>
				<select name="annualy" class="form-control" id="annualy">
                		<option value="0">Select</option>
                		<?php
                			for($i=date('Y'); $i>=1950; $i--){
                				//echo '<option value="'.$i.'">'.$i.'</option>';
								$x=$i+1;
								
                		?>
						<option value="<?php echo $i." - ".$x;?>"<?php if($annualy==$i) {?> selected <?php } ?>><?php echo $i." - ".$x; ?></option>
                	<?php }?>
               	  </select>
		 		</td></tr>
				
					<tr><td colspan="2">
			<?php  $case_type = isset($_REQUEST['case_type']) ? $_REQUEST['case_type'] :'';?>
			
				<label><font color="#FF0000">*</font>Select Case Type:</label>		
				<select name="case_type" id="case_type" class="form-control form-control-sm">
				<option value="0">Select</option>
				<option value="1" <?php if($case_type=="1") {?> selected <?php } ?>>Original Application (OA)</option>
				<option value="7" <?php if($case_type=="7") {?> selected <?php } ?>>Securitisation Application (SA)</option>
				</select>
				
			</td></tr>
			
				<tr><td align="Right">
				<input type="submit" name="btnSubmit" id="btnSubmit" value="Search" class="btn btn-primary"/>
				</td></tr>
				<?php 
				
				if($annualy!='0' and $case_type!='0' and ($schemas >'0' or $schemaname!='0')) { ?>	
				<tr><td> 
				<br/>
				<div>
				<button  class="btn btn-primary d-print-none" onclick="window.print()"> <i class="fa fa-print fa-lg"></i>&nbsp;Print</button></div>
				<div><b>Report Prepared On <font color="red">  <?php echo date("d-m-Y h:i:sa"); ?></font></b></div>
				</td></tr>
				<?php }?>
		</table>
					<?php if($annualy!='0' and $case_type!='0' and ($schemas!='' or $schemaname!='')) { ?>
		<div align="center">
				
		<b>Age-wise list of Pending
		  <?php 
			if($case_type=="1") { echo "Original Applications(OAs)"; }
			if($case_type=="7") { echo "Securitization Applications(SAs)"; }
			?>	
				For The Financial Year <?php  $annualy; ?> 
				<?php 
				 $abbb = substr($annualy,7);
				 $edateeeee='31/03/'.$abbb;
				//echo " ".$edateeeee ;
				$dt=date('Y');
					  $edate=date('d-m-Y');
					  if($abbb > $dt)
					  {
				  
			echo $annualy." (As on ".$edate.")";
			}
			else
			{
			echo $annualy." (As on ".$edateeeee.")";
			}
				
				?> 
				</div></br>
		</div></div></div>
	<?php 
			$schemas=htmlentities(htmlspecialchars($schemas));
				$annualy1=htmlentities(htmlspecialchars($annualy));	
				$case_type1=htmlentities(htmlspecialchars($case_type));
				$schemaname1=htmlentities(htmlspecialchars($schemaname));
					
	if($userid=="31" or $userid=='1458' or $userid=='1465' or $userid=='1467' or $userid=='1468' or $userid=='1469'){				
	if($schemas=='1' or $schemas > '100'){
	if($schemaname1!='' and !is_numeric($schemaname1))
	{
		echo "error : Not Valid Entry11....";
		session_unset();     // unset $_SESSION variable for the run-time
		session_destroy();
		//$aaz='108';
		header("Location: ../login.php");
			die();
	} }
	}
	if($case_type1!=''){
	if(!is_numeric($case_type1))
	{
		echo "error : Not Valid Entry22....";
		session_unset();     // unset $_SESSION variable for the run-time
		session_destroy();
		//$aaz='108';
		header("Location: ../login.php");
			die();
	}}
	
					$end=strlen($annualy);
  					 if($end > '11')
					{
					echo "error : Not Valid Entry33....";
					session_unset();     // unset $_SESSION variable for the run-time
					session_destroy();
					//$aaz='108';
					header("Location: ../login.php");
					die();
					}													
	$cur_yr=date("Y");
	?>			
		<div class ="row" style="margin-left:10px;">	
		<div class="table-responsive">
			<table width="90%" class="table table-bordered" cellpadding="1" cellspacing="1">
                    <thead>
                        <tr><?php if ($schemas!= '1' and ($userid=="31" or $userid=='1458' or $userid=='1465' or $userid=='1467' or $userid=='1468' or $userid=='1469')) {?>
                            <th width="64" align="center">DRAT Name</th>
			    			<?php }?>
                            <th width="86" align="center">DRT Name</th>
							
	<th width="167" align="center">upto 6 Months
             <table width="146" cellspacing="1" cellpadding="1" class="table table-condensed table-bordered">
	<th width="31"> No. of Cases Pending</th>
	<th width="31"> Amount Involved(Rs. in Cr.)</th>
	</table>	
							
						  </th> 
							<th width="167" align="center">Above 6 Months to 1 Year
							  <table width="146" cellspacing="1" cellpadding="1" class="table table-condensed table-bordered">
	<th width="31"> No. of Cases Pending</th>
	<th width="31"> Amount Involved(Rs. in Cr.)</th>
	</table>
	
		
	<th width="167" align="center">Above 1 Year to 3 Years
	  <table width="146" cellspacing="1" cellpadding="1" class="table table-condensed ">
	<th width="31"> No. of Cases Pending</th>
	<th width="31"> Amount Involved(Rs. in Cr.) </th>
	</table>	
	<th width="167" align="center">Above 3 to 5 Years 
	  <table width="146" cellspacing="1" cellpadding="1" class="table table-condensed table-bordered">
	<th width="31"> No. of Cases Pending</th>
	<th width="31"> Amount Involved(Rs. in Cr.)</th>
	</table>	
	<th width="167" align="center">Above 5 to 10 Years
	  <table width="146" cellspacing="1" cellpadding="1" class="table table-condensed table-bordered">
	<th width="31"> No. of Cases Pending</th>
	<th width="31"> Amount Involved(Rs. in Cr.)</th>
	</table>	
	<th width="167" align="center">Above 10 Years
	<table width="146" cellspacing="1" cellpadding="1" class="table table-condensed table-bordered">
	<th width="31"> No. of Cases Pending</th>
	<th width="31"> Amount Involved(Rs. in Cr.)</th>
	</table>	
	<th width="167" align="center">Total
	<table width="146" cellspacing="1" cellpadding="1" class="table table-condensed table-bordered">
	<th width="31"> No. of Cases Pending</th>
	<th width="31"> Amount Involved(Rs. in Cr.)</th>
	</table></th>	
	                </tr>
                    </thead>
                    <tbody>	
					<?php 
					
					if($userid=="31" or $userid=='1458' or $userid=='1465' or $userid=='1467' or $userid=='1468' or $userid=='1469') {
					if ($schemas == '1') {		
				  $sql_all = "select i.short_name,m.schema_name from initilization as i,master_schema as m where m.display='Y' and i.schema_id=m.schema_id and m.schema_id <100 order by i.short_name  ASC";
						}
						elseif($schemaname == '222')
					{
				 $sql_all = "select i.short_name,m.schema_name from initilization as i,master_schema as m where m.display='Y' and i.schema_id=m.schema_id and  m.schema_id!='$schemas' and m.drat_id = '$schemas' order by i.short_name  ASC";
							}else{
							
					$sql_all = "select i.short_name,m.schema_name from initilization as i,master_schema as m where m.display='Y' and i.schema_id=m.schema_id and  m.schema_id!='$schemas' and m.schema_id='$schemaname'";
					}}
					 if($userid=='1458' or $userid=='1465' or $userid=='1467' or $userid=='1468' or $userid=='1469') { } elseif($userid!="31") {
						 $sql_all = "select schema_name from master_schema where display='Y' and schema_id='$schemaname'";
							}
							$allSchema = $db->prepare($sql_all);
							$allSchema->execute();
							while ($row = $allSchema->fetch(PDO::FETCH_ASSOC, PDO::FETCH_ORI_NEXT))
							 {
						 $allSchemaNmae = $row['schema_name'];
						 $allSchemaNmae1 = $row['short_name'];
					
					list($dd,$mm,$yyyy)=explode('/',$c_date);
   					 $startDate="$yyyy-$mm-$dd";
   
 				  list($dd,$mm,$yyyy)=explode('/',$t_date);
    				 $endDate="$yyyy-$mm-$dd";

					 if($case_type=='1'){
						$case_type_in="case_type in ('1','6')";

					}
					if($case_type=='7'){
						$case_type_in="case_type in ('11','7')";
					}
					if($date_type=='11')
					{
						$case_no_in="filing_no is  null";
					}
				  if($date_type=='22')
				  {
					 $case_no_in="case_no is not null";
				} 	
					   
					
					 
/********************************************   CURRENT YEAR   *****************************************************/
					
					  $ab = substr($annualy,7);
						//$sdate=date("Y-m-d", strtotime("-6 months"));
					  $dt=date('Y');
					  if($ab > $dt){
					 
					  $edate=date('Y-m-d');
					  $sdate = date("Y-m-d", strtotime('-6 months', strtotime($edate)) );
					  }
					  else
					  {		
					 				
					     $edate=$ab.'-03-31';
						 $sdate = date("Y-m-d", strtotime('-6 months', strtotime($edate)) );
						 }
						 
						 list($styear,$endyear)=explode('-',$annualy);
						 $styear=rtrim($styear);
						  $startDate="$styear-04-01";
						 $endDate="$endyear-03-31";
						
						  
						 
/********************************************   0 To 6 MONTHS   *****************************************************/
						
					if($case_type=='1')
					{
					if($date_type=='11')
					{	
				/*echo "select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('1','6')  and (a.dt_of_filing BETWEEN '$sdate' and '$edate') and b.suit_amount >= '1000000' and b.suit_amount is not NULL GROUP BY b.suit_amount";*/
					$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total
                     from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b
                      where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no 
                      and a.case_type IN ('1','6')  and (a.dt_of_filing BETWEEN '$sdate' and '$edate') 
                      and b.suit_amount >= '1000000' and b.suit_amount is not NULL GROUP BY b.suit_amount"); 
                      
                      
					}
					if($date_type=='22')
					{	
					/*$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total 
                    from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b 
                    where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no 
                    and a.case_type IN ('1','6')  and (a.regis_date BETWEEN '$sdate' and '$edate') 
                    and b.suit_amount :: DOUBLE PRECISION >= '1000000' and b.suit_amount is not NULL GROUP BY b.suit_amount");*/
					$stpp=$db->prepare("WITH cte_1 AS (
						SELECT
							( filing_no ),
							MAX ( suit_amount :: DOUBLE PRECISION ) AS suit_amount 
						FROM
							$allSchemaNmae.account_details 
						WHERE
							suit_amount IS NOT NULL 
							AND suit_amount != '0' 
							AND filing_no IS NOT NULL 
							AND suit_amount !=''
						GROUP BY
							filing_no 
						) SELECT  '1' as total ,A.suit_amount
					FROM
						$allSchemaNmae.case_detail
						AS C INNER JOIN cte_1 AS A ON C.filing_no = A.filing_no 
					WHERE
						( case_type IN ( '1', '6' ) AND LENGTH ( case_no )= '15' ) 
						AND regis_date IS NOT NULL 
						AND regis_date BETWEEN '$sdate' and '$edate' 
						AND C.case_no != '' 
						AND ( UPPER ( status ) = 'P' ) 
						");

					
                   
                    }
					
					}
					if($case_type=='7')
					{
					if($date_type=='11')
					{
					$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total 
                    from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where
                     b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type
                      IN ('7','11')  and (a.dt_of_filing BETWEEN '$sdate' and '$edate') 
                      and b.suit_amount >= '100000' and b.suit_amount is not NULL GROUP BY b.suit_amount"); 
					}
					
					if($date_type=='22')
					{
					/*$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total
                     from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b 
                     where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no 
                     and a.case_type IN ('7','11')  and (a.regis_date BETWEEN '$sdate' and '$edate') 
                     and b.suit_amount >= '100000' and b.suit_amount is not NULL GROUP BY b.suit_amount"); 
                     */
					$stpp=$db->prepare("WITH cte_1 AS (
						SELECT
							( filing_no ),
							MAX ( suit_amount :: DOUBLE PRECISION ) AS suit_amount 
						FROM
							$allSchemaNmae.account_details 
						WHERE
							suit_amount IS NOT NULL 
							AND suit_amount != '0' 
							AND filing_no IS NOT NULL 
							AND suit_amount !=''
						GROUP BY
							filing_no 
						) SELECT  '1' as total ,A.suit_amount
					FROM
						$allSchemaNmae.case_detail
						AS C INNER JOIN cte_1 AS A ON C.filing_no = A.filing_no 
					WHERE
						( case_type IN ( '7', '11' ) AND LENGTH ( case_no )= '15' ) 
						AND regis_date IS NOT NULL 
						AND regis_date BETWEEN '$sdate' and '$edate' 
						AND C.case_no != '' 
						AND ( UPPER ( status ) = 'P' )");
				}
					
					}
					   $stpp->execute();
							while ($row = $stpp->fetch(PDO::FETCH_ASSOC,PDO::FETCH_ORI_NEXT))
							{
							 $filing_no=$row['filing_no'];
							$suit_amount=$row['suit_amount'];
							$total = $row['total'];
							$total1=$total1+$suit_amount;
						  $totaldd2=$totaldd2+$total;
						  $tc=$tc+$total;
						  $ts=$ts+$suit_amount;
					}
					
/********************************************   6 To 1 YEAR   *****************************************************/

					 	 $sdate1 = date("Y-m-d", strtotime('-12 months', strtotime($edate)) );
							$s_date1 = date("Y-m-d", strtotime($sdate1) );
					 	  $sdate11 = date("Y-m-d", strtotime('+1 days', strtotime($s_date1)) );
						 $edate1 = date("Y-m-d", strtotime('-6 months', strtotime($edate)) );
						 $e_date1 = date("Y-m-d", strtotime($edate1) );
						  $edate11 = date("Y-m-d", strtotime('-1 days', strtotime($e_date1)) );
					 
		if($case_type=='1')
					{
			if($date_type=='11')
					{		
					$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('1','6')  and (a.dt_of_filing BETWEEN '$sdate11' and '$edate11') and b.suit_amount >= '1000000' and b.suit_amount is not NULL GROUP BY b.suit_amount"); 
					}
					if($date_type=='22')
					{		
					/*$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('1','6')  and (a.regis_date BETWEEN '$sdate11' and '$edate11') and b.suit_amount >= '1000000' and b.suit_amount is not NULL GROUP BY b.suit_amount");*/
					$stpp=$db->prepare("WITH cte_1 AS (
						SELECT
							( filing_no ),
							MAX ( suit_amount :: DOUBLE PRECISION ) AS suit_amount 
						FROM
							$allSchemaNmae.account_details 
						WHERE
							suit_amount IS NOT NULL 
							AND suit_amount != '0' 
							AND filing_no IS NOT NULL 
							AND suit_amount !=''
						GROUP BY
							filing_no 
						) SELECT  '1' as total ,A.suit_amount
					FROM
						$allSchemaNmae.case_detail
						AS C INNER JOIN cte_1 AS A ON C.filing_no = A.filing_no 
					WHERE
						( case_type IN ( '6', '1' ) AND LENGTH ( case_no )= '15' ) 
						AND regis_date IS NOT NULL 
						AND regis_date BETWEEN '$sdate11' and '$edate11' 
						AND C.case_no != '' 
						AND ( UPPER ( status ) = 'P' )");
					 
					}
					}
					if($case_type=='7')
					{
				if($date_type=='11')
					{	
					$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('7','11')  and (a.dt_of_filing BETWEEN '$sdate11' and '$edate11') and b.suit_amount >= '100000' and b.suit_amount is not NULL GROUP BY b.suit_amount"); 
					}
					if($date_type=='22')
					{	
					/*$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('7','11')  and (a.regis_date BETWEEN '$sdate11' and '$edate11') and b.suit_amount >= '100000' and b.suit_amount is not NULL GROUP BY b.suit_amount");*/
					$stpp=$db->prepare("WITH cte_1 AS (
						SELECT
							( filing_no ),
							MAX ( suit_amount :: DOUBLE PRECISION ) AS suit_amount 
						FROM
							$allSchemaNmae.account_details 
						WHERE
							suit_amount IS NOT NULL 
							AND suit_amount != '0' 
							AND filing_no IS NOT NULL 
							AND suit_amount !=''
						GROUP BY
							filing_no 
						) SELECT  '1' as total ,A.suit_amount
					FROM
						$allSchemaNmae.case_detail
						AS C INNER JOIN cte_1 AS A ON C.filing_no = A.filing_no 
					WHERE
						( case_type IN ( '7', '11' ) AND LENGTH ( case_no )= '15' ) 
						AND regis_date IS NOT NULL 
						AND regis_date BETWEEN '$sdate11' and '$edate11' 
						AND C.case_no != '' 
						AND ( UPPER ( status ) = 'P' )"); 
					}
					}
					$stpp->execute();
							while ($row = $stpp->fetch(PDO::FETCH_ASSOC,PDO::FETCH_ORI_NEXT))
							{
							 $filing_no=$row['filing_no'];
							$suit_amount=$row['suit_amount'];
							$ttotal = $row['total'];
							$ttotal1=$ttotal1+$suit_amount;
						 	$ttotaldd2=$ttotaldd2+$ttotal;
							$tc1=$tc1+$ttotal;
						 	$ts1=$ts1+$suit_amount;
							
					}
/********************************************   1 To 3 YEARS   *****************************************************/

					
						 $sdate2 = date("Y-m-d", strtotime('-36 months', strtotime($edate)) );
							$s_date2 = date("Y-m-d", strtotime($sdate2) );
						  $sdate12 = date("Y-m-d", strtotime('+1 days', strtotime($s_date2)) );
						 $edate2 = date("Y-m-d", strtotime('-12 months', strtotime($edate)) );
						 					
				if($case_type=='1')
					{
				if($date_type=='11')
					{
					$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('1','6')  and (a.dt_of_filing BETWEEN '$sdate12' and '$edate2') and b.suit_amount!='0' and b.suit_amount >= '1000000' and b.suit_amount is not NULL GROUP BY b.suit_amount"); 
					}
					if($date_type=='22')
					{
					/*$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('1','6')  and (a.regis_date BETWEEN '$sdate12' and '$edate2') and b.suit_amount!='0' and b.suit_amount >= '1000000' and b.suit_amount is not NULL GROUP BY b.suit_amount"); */
					
					$stpp=$db->prepare("WITH cte_1 AS (
						SELECT
							( filing_no ),
							MAX ( suit_amount :: DOUBLE PRECISION) AS suit_amount 
						FROM
							$allSchemaNmae.account_details 
						WHERE
							suit_amount IS NOT NULL 
							AND suit_amount != '0' 
							AND filing_no IS NOT NULL 
							AND suit_amount !=''
						GROUP BY
							filing_no 
						) SELECT  '1' as total ,A.suit_amount
					FROM
						$allSchemaNmae.case_detail
						AS C INNER JOIN cte_1 AS A ON C.filing_no = A.filing_no 
					WHERE
						( case_type IN ( '1', '6' ) AND LENGTH ( case_no )= '15' ) 
						AND regis_date IS NOT NULL 
						AND regis_date BETWEEN '$sdate12' and '$edate2' 
						AND C.case_no != '' 
						AND ( UPPER ( status ) = 'P' ) ");

					}
					}
					if($case_type=='7')
					{
					if($date_type=='11')
					{
					$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('7','11')  and (a.dt_of_filing BETWEEN '$sdate12' and '$edate2') and b.suit_amount!='0' and b.suit_amount >= '100000' and b.suit_amount is not NULL GROUP BY b.suit_amount"); 
					}
					if($date_type=='22')
					{
					/*$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('7','11')  and (a.regis_date BETWEEN '$sdate12' and '$edate2') and b.suit_amount!='0' and b.suit_amount >= '100000' and b.suit_amount is not NULL GROUP BY b.suit_amount"); 
					*/
					$stpp=$db->prepare("WITH cte_1 AS (
						SELECT
							( filing_no ),
							MAX ( suit_amount :: DOUBLE PRECISION) AS suit_amount 
						FROM
							$allSchemaNmae.account_details 
						WHERE
							suit_amount IS NOT NULL 
							AND suit_amount != '0' 
							AND filing_no IS NOT NULL 
							AND suit_amount !=''
						GROUP BY
							filing_no 
						) SELECT  '1' as total ,A.suit_amount
					FROM
						$allSchemaNmae.case_detail
						AS C INNER JOIN cte_1 AS A ON C.filing_no = A.filing_no 
					WHERE
						( case_type IN ( '7', '11' ) AND LENGTH ( case_no )= '15' ) 
						AND regis_date IS NOT NULL 
						AND regis_date BETWEEN '$sdate12' and '$edate2' 
						AND C.case_no != '' 
						AND ( UPPER ( status ) = 'P' ) ");
						
				
				}
					} 
							$stpp->execute();
							while ($row = $stpp->fetch(PDO::FETCH_ASSOC,PDO::FETCH_ORI_NEXT))
							{
							 $filing_no=$row['filing_no'];
							$suit_amount1=$row['suit_amount'];
							$total2 = $row['total'];
							$totall1=$totall1+$suit_amount1;
							$total3=$total3+$total2;
							$tc2=$tc2+$total2;
						 	$ts2=$ts2+$suit_amount1;
					}
					
/********************************************   3 To 5 YEARS   *****************************************************/
					
						 $sdate3 = date("Y-m-d", strtotime('-60 months', strtotime($edate)) );
							$s_date3 = date("Y-m-d", strtotime($sdate3) );
						  $sdate13 = date("Y-m-d", strtotime('+1 days', strtotime($s_date3)) );
						 $edate3 = date("Y-m-d", strtotime('-36 months', strtotime($edate)) );
						 
					
					if($case_type=='1')
					{
					if($date_type=='11')
					{
					$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('1','6')  and (a.dt_of_filing BETWEEN '$sdate13' and '$edate3') and b.suit_amount!='0' and b.suit_amount >= '1000000' and b.suit_amount is not NULL GROUP BY b.suit_amount"); 
					}
					if($date_type=='22')
					{
					/*$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('1','6')  and (a.regis_date BETWEEN '$sdate13' and '$edate3') and b.suit_amount!='0' and b.suit_amount >= '1000000' and b.suit_amount is not NULL GROUP BY b.suit_amount");*/
					$stpp=$db->prepare("WITH cte_1 AS (
						SELECT
							( filing_no ),
							MAX ( suit_amount :: DOUBLE PRECISION) AS suit_amount 
						FROM
							$allSchemaNmae.account_details 
						WHERE
							suit_amount IS NOT NULL 
							AND suit_amount != '0' 
							AND filing_no IS NOT NULL 
							AND suit_amount !=''
						GROUP BY
							filing_no 
						) SELECT  '1' as total ,A.suit_amount
					FROM
						$allSchemaNmae.case_detail
						AS C INNER JOIN cte_1 AS A ON C.filing_no = A.filing_no 
					WHERE
						( case_type IN ( '1', '6' ) AND LENGTH ( case_no )= '15' ) 
						AND regis_date IS NOT NULL 
						AND regis_date BETWEEN '$sdate13' and '$edate3' 
						AND C.case_no != '' 
						AND ( UPPER ( status ) = 'P' ) ");
 
					}
					}
					if($case_type=='7')
					{
					if($date_type=='11')
					{

					$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('7','11')  and (a.dt_of_filing BETWEEN '$sdate13' and '$edate3') and b.suit_amount!='0' and b.suit_amount >= '100000' and b.suit_amount is not NULL GROUP BY b.suit_amount"); 
					} 
					if($date_type=='22')
					{
					/*$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('7','11')  and (a.regis_date BETWEEN '$sdate13' and '$edate3') and b.suit_amount!='0' and b.suit_amount >= '100000' and b.suit_amount is not NULL GROUP BY b.suit_amount");*/
					$stpp=$db->prepare("WITH cte_1 AS (
						SELECT
							( filing_no ),
							MAX ( suit_amount :: DOUBLE PRECISION) AS suit_amount 
						FROM
							$allSchemaNmae.account_details 
						WHERE
							suit_amount IS NOT NULL 
							AND suit_amount != '0' 
							AND filing_no IS NOT NULL 
							AND suit_amount !=''
						GROUP BY
							filing_no 
						) SELECT  '1' as total ,A.suit_amount
					FROM
						$allSchemaNmae.case_detail
						AS C INNER JOIN cte_1 AS A ON C.filing_no = A.filing_no 
					WHERE
						( case_type IN ( '7', '11' ) AND LENGTH ( case_no )= '15' ) 
						AND regis_date IS NOT NULL 
						AND regis_date BETWEEN '$sdate13' and '$edate3' 
						AND C.case_no != '' 
						AND ( UPPER ( status ) = 'P' ) ");	 
					} 
					} 
					$stpp->execute();
							while ($row = $stpp->fetch(PDO::FETCH_ASSOC,PDO::FETCH_ORI_NEXT))
							{
							 $filing_no=$row['filing_no'];
							$suit_amount23=$row['suit_amount'];
							$total133 = $row['total'];
							$total123=$total123+$suit_amount23;
							$total43=$total43+$total133;
							$tc3=$tc3+$total133;
						 	$ts3=$ts3+$suit_amount23;
					}
/********************************************   5 To 10 YEARS   *****************************************************/
										 
					 $sdate4 = date("Y-m-d", strtotime('-120 months', strtotime($edate)) );
					 $s_date4 = date("Y-m-d", strtotime($sdate4) );
					 $sdate14 = date("Y-m-d", strtotime('+1 days', strtotime($s_date4)) );
					 $edate4 = date("Y-m-d", strtotime('-60 months', strtotime($edate)) );
					
					if($case_type=='1')
					{
					if($date_type=='11')
					{
					$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('1','6')  and (a.dt_of_filing BETWEEN '$sdate14' and '$edate4') and b.suit_amount!='0' and b.suit_amount >= '1000000' and b.suit_amount is not NULL GROUP BY b.suit_amount");
					} 
					if($date_type=='22')
					{
					/*$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('1','6')  and (a.regis_date BETWEEN '$sdate14' and '$edate4') and b.suit_amount!='0' and b.suit_amount >= '1000000' and b.suit_amount is not NULL GROUP BY b.suit_amount");*/
					$stpp=$db->prepare("WITH cte_1 AS (
						SELECT
							( filing_no ),
							MAX ( suit_amount :: DOUBLE PRECISION) AS suit_amount 
						FROM
							$allSchemaNmae.account_details 
						WHERE
							suit_amount IS NOT NULL 
							AND suit_amount != '0' 
							AND filing_no IS NOT NULL 
							AND suit_amount !=''
						GROUP BY
							filing_no 
						) SELECT  '1' as total ,A.suit_amount
					FROM
						$allSchemaNmae.case_detail
						AS C INNER JOIN cte_1 AS A ON C.filing_no = A.filing_no 
					WHERE
						( case_type IN ( '1', '6' ) AND LENGTH ( case_no )= '15' ) 
						AND regis_date IS NOT NULL 
						AND regis_date BETWEEN '$sdate14' and '$edate4' 
						AND C.case_no != '' 
						AND ( UPPER ( status ) = 'P' ) ");
					} 
					}
					if($case_type=='7')
					{
					if($date_type=='11')
					{
					$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('7','11')  and (a.dt_of_filing BETWEEN '$sdate14' and '$edate4') and b.suit_amount!='0' and b.suit_amount >= '100000' and b.suit_amount is not NULL GROUP BY b.suit_amount");
					} 
					if($date_type=='22')
					{
					/*	
					$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('7','11')  and (a.regis_date BETWEEN '$sdate14' and '$edate4') and b.suit_amount!='0' and b.suit_amount >= '100000' and b.suit_amount is not NULL GROUP BY b.suit_amount");*/
					$stpp=$db->prepare("WITH cte_1 AS (
						SELECT
							( filing_no ),
							MAX ( suit_amount :: DOUBLE PRECISION) AS suit_amount 
						FROM
							$allSchemaNmae.account_details 
						WHERE
							suit_amount IS NOT NULL 
							AND suit_amount != '0' 
							AND filing_no IS NOT NULL 
							AND suit_amount !=''
						GROUP BY
							filing_no 
						) SELECT  '1' as total ,A.suit_amount
					FROM
						$allSchemaNmae.case_detail
						AS C INNER JOIN cte_1 AS A ON C.filing_no = A.filing_no 
					WHERE
						( case_type IN ( '7', '11' ) AND LENGTH ( case_no )= '15' ) 
						AND regis_date IS NOT NULL 
						AND regis_date BETWEEN '$sdate14' and '$edate4' 
						AND C.case_no != '' 
						AND ( UPPER ( status ) = 'P' ) ");
					} 
					}  
					$stpp->execute();
							while ($row = $stpp->fetch(PDO::FETCH_ASSOC,PDO::FETCH_ORI_NEXT))
							{
							 $filing_no=$row['filing_no'];
							$suit_amount2=$row['suit_amount'];
							$ttotal13 = $row['total'];
							$total12=$total12+$suit_amount2;
							$ttotal4=$ttotal4+$ttotal13;
							$tc4=$tc4+$ttotal13;
						 	$ts4=$ts4+$suit_amount2;
					}
					
/********************************************   ABOVE 10 YEARS   *****************************************************/

					 
					 $edate4 = date("Y-m-d", strtotime('-120 months', strtotime($edate)) );
					 
					if($case_type=='1')
					{
					if($date_type=='11')
					{
					$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('1','6')  and (a.dt_of_filing <= '$edate4' ) and b.suit_amount!='0' and b.suit_amount >= '1000000' and b.suit_amount is not NULL GROUP BY b.suit_amount"); 
					}
					if($date_type=='22')
					{
					
					// $stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('1','6')  and (a.regis_date <= '$edate4' ) and b.suit_amount!='0' and b.suit_amount >= '1000000' and b.suit_amount is not NULL GROUP BY b.suit_amount");
					$stpp=$db->prepare("WITH cte_1 AS (
						SELECT
							( filing_no ),
							MAX ( suit_amount :: DOUBLE PRECISION) AS suit_amount 
						FROM
							$allSchemaNmae.account_details 
						WHERE
							suit_amount IS NOT NULL 
							AND suit_amount != '0' 
							AND filing_no IS NOT NULL 
							AND suit_amount !=''
						GROUP BY
							filing_no 
						) SELECT  '1' as total ,A.suit_amount
					FROM
						$allSchemaNmae.case_detail
						AS C INNER JOIN cte_1 AS A ON C.filing_no = A.filing_no 
					WHERE
						( case_type IN ( '1', '6' ) AND LENGTH ( case_no )= '15' ) 
						AND regis_date IS NOT NULL 
						AND regis_date <= '$edate4' 
						AND C.case_no != '' 
						AND ( UPPER ( status ) = 'P' ) "); 
					}
					}
					if($case_type=='7')
					{
					if($date_type=='11')
					{
					$stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('7','11')  and (a.dt_of_filing <= '$edate4' ) and b.suit_amount!='0' and b.suit_amount >= '100000' and b.suit_amount is not NULL GROUP BY b.suit_amount"); 
					}
					if($date_type=='22')
					{
					// $stpp = $db->prepare("select b.suit_amount,count(DISTINCT a.filing_no) as total from $allSchemaNmae.case_detail as a, $allSchemaNmae.account_details as b where b.suit_amount is not NULL and a.status='P' and a.filing_no=b.filing_no and a.case_type IN ('7','11')  and (a.regis_date <= '$edate4' ) and b.suit_amount!='0' and b.suit_amount >= '100000' and b.suit_amount is not NULL GROUP BY b.suit_amount"); 
					$stpp=$db->prepare("WITH cte_1 AS (
						SELECT
							( filing_no ),
							MAX ( suit_amount :: DOUBLE PRECISION) AS suit_amount 
						FROM
							$allSchemaNmae.account_details 
						WHERE
							suit_amount IS NOT NULL 
							AND suit_amount != '0' 
							AND filing_no IS NOT NULL 
							AND suit_amount !=''
						GROUP BY
							filing_no 
						) SELECT  '1' as total ,A.suit_amount
					FROM
						$allSchemaNmae.case_detail
						AS C INNER JOIN cte_1 AS A ON C.filing_no = A.filing_no 
					WHERE
						( case_type IN ( '7', '11' ) AND LENGTH ( case_no )= '15' ) 
						AND regis_date IS NOT NULL 
						AND regis_date <= '$edate4' 
						AND C.case_no != '' 
						AND ( UPPER ( status ) = 'P' ) ");
					}
					}  
					$stpp->execute();
							while ($row = $stpp->fetch(PDO::FETCH_ASSOC,PDO::FETCH_ORI_NEXT))
							{
							 $filing_no=$row['filing_no'];
							$suit_amount3=$row['suit_amount'];
							$total4 = $row['total'];
							$total13=$total13+$suit_amount3;
							$total21=$total21+$total4;
							$tc5=$tc5+$total4;
						 	$ts5=$ts5+$suit_amount3;
					}
					

					if($date_type=='11')
					{



					$sqlp=$db->prepare("select count(a.filing_no) from (select  filing_no from $allSchemaNmae.case_detail where  $case_type_in and dt_of_filing < '$startDate' and (UPPER(status)='P' or (status= 'D' and disposal_date >= '$startDate')) 
				   union all
					select  filing_no from $allSchemaNmae.case_detail where   $case_type_in and (dt_of_filing between '$startDate' and '$endDate') and (UPPER(status) in ('P', 'D'))
				   except
					select filing_no  from $allSchemaNmae.case_detail where  $case_type_in and UPPER(status)='D' and (disposal_date between '$startDate' and '$endDate'))as a");		
					$sqlp->execute();
					$final_total= $sqlp->fetchColumn(); 

					
					
				/*$stpp11211 = $db->prepare
				("WITH cte_1 AS (
					SELECT
						(filing_no),		
						MAX ( CAST ( suit_amount AS DOUBLE PRECISION ) ) AS suit_amount 
					FROM
					$allSchemaNmae.account_details 
					WHERE
						suit_amount IS NOT NULL 
						AND suit_amount != '0' 
						AND filing_no IS NOT NULL 
						AND suit_amount != '' 
					GROUP BY
						filing_no
					)	
				SELECT sum
					( A.suit_amount ) 
				FROM
					(
					SELECT
						c.filing_no,aa.suit_amount 
					FROM
					$allSchemaNmae.case_detail AS C INNER JOIN cte_1 AS aa ON C.filing_no = aa.filing_no 
					WHERE
					(C.filing_no IS NOT NULL AND LENGTH ( C.filing_no ) = '15') 
						
						AND dt_of_filing IS NOT NULL  AND dt_of_filing <= '$edate'
						AND ( UPPER ( status ) = 'P' OR ( status = 'D' AND disposal_date >= '$endDate' ) ) UNION ALL
					SELECT
						c.filing_no ,aa.suit_amount
					FROM
					$allSchemaNmae.case_detail AS C INNER JOIN cte_1 AS aa ON C.filing_no = aa.filing_no 
					WHERE
						(C.filing_no IS NOT NULL AND LENGTH (C.filing_no ) = '15')
						AND $case_type_in
						AND ( dt_of_filing BETWEEN '$startDate' and '$endDate' ) 
						AND ( UPPER ( status ) IN ( 'P', 'D' ) ) EXCEPT
					SELECT
						c.filing_no ,aa.suit_amount
					FROM
					$allSchemaNmae.case_detail AS C INNER JOIN cte_1 AS aa ON C.filing_no = aa.filing_no 
					WHERE
						(C.filing_no IS NOT NULL AND LENGTH (C.filing_no ) = '15') 
						AND $case_type_in
						AND UPPER ( status ) = 'D' 
					AND ( disposal_date BETWEEN '$startDate' and '$endDate' ) 
					) AS A");*/
				 
						$stpp11211 = $db->prepare("WITH cte_1 AS (
	SELECT
		( filing_no ),
		MAX ( CAST ( suit_amount AS DOUBLE PRECISION ) ) AS suit_amount 
	FROM
		$allSchemaNmae.account_details 
	WHERE
		suit_amount IS NOT NULL 
		AND suit_amount != '0' 
		AND filing_no IS NOT NULL 
		AND suit_amount != '' 
	GROUP BY
		filing_no 
	) SELECT SUM
	( A.suit_amount ) 
FROM
	(
	SELECT C
		.filing_no,
		aa.suit_amount 
	FROM
		$allSchemaNmae.case_detail
		AS C INNER JOIN cte_1 AS aa ON C.filing_no = aa.filing_no 
	WHERE
		( C.filing_no IS NOT NULL AND LENGTH ( C.filing_no ) = '15' ) and 
		--AND regis_date IS NOT NULL 
		 case_type IN ( '1', '6' ) 
		--AND regis_date IS NOT NULL 
		AND dt_of_filing <= '$edate'
		AND ( UPPER ( status ) = 'P' OR ( status = 'D' AND disposal_date  >= '$endDate'  ) ) UNION ALL
	SELECT C
		.filing_no,
		aa.suit_amount 
	FROM
		siliguri.case_detail
		AS C INNER JOIN cte_1 AS aa ON C.filing_no = aa.filing_no 
	WHERE
	( C.filing_no IS NOT NULL AND LENGTH (C.filing_no ) = '15' ) 
		--AND regis_date IS NOT NULL 
		AND $case_type_in
		AND ( dt_of_filing BETWEEN '$startDate' and '$endDate' )  
		AND ( UPPER ( status ) IN ( 'P', 'D' ) ) EXCEPT
	SELECT C
		.filing_no,
		aa.suit_amount 
	FROM
		siliguri.case_detail
		AS C INNER JOIN cte_1 AS aa ON C.filing_no = aa.filing_no 
	WHERE
		(C.filing_no IS NOT NULL AND LENGTH (C.filing_no ) = '15' )
		---AND regis_date IS NOT NULL 
	AND $case_type_in
		AND UPPER ( status ) = 'D' 
	AND ( disposal_date BETWEEN '$startDate' and '$endDate' )  
	) AS A");






				  

				$stpp11211->execute();
				$final_suit = $stpp11211->fetchColumn();
		   

					}   
					
					if($date_type=='22')
					{

					$sqlp=$db->prepare("select count(a.filing_no) from (select  filing_no from $allSchemaNmae.case_detail where ($case_no_in and LENGTH(case_no)='15') and regis_date is not null 
					and $case_type_in and regis_date < '$startDate' and (UPPER(status)='P' or (status= 'D' and disposal_date >= '$startDate')) 
				   union all
					select  filing_no from $allSchemaNmae.case_detail where (case_no is not null and case_no!='' and LENGTH(case_no)='15') and regis_date is not null 
					and $case_type_in and (regis_date between '$startDate' and '$endDate') and (UPPER(status) in ('P', 'D'))
				   except
					select filing_no  from $allSchemaNmae.case_detail where (case_no is not null and LENGTH(case_no)='15') and regis_date is not null 
					and $case_type_in and UPPER(status)='D' and (disposal_date between '$startDate' and '$endDate'))as a");		
					$sqlp->execute();
					$final_total= $sqlp->fetchColumn(); 
					                       
				/* 	$stpp11211 = $db->prepare("with cte_1 as (SELECT( filing_no ),
					MAX ( suit_amount :: DOUBLE PRECISION) AS suit_amount 
				FROM
					$allSchemaNmae.account_details 
				WHERE
				 suit_amount IS NOT NULL AND suit_amount != '0' and filing_no is not null AND suit_amount !=''
				GROUP BY
					filing_no)
				
					SELECT sum(a.suit_amount :: DOUBLE PRECISION )FROM $allSchemaNmae.case_detail  as c inner join cte_1 as a on  c.filing_no=a.filing_no
				WHERE ($case_type_in AND LENGTH (case_no)='15') 
				AND regis_date IS NOT NULL  AND regis_date <= '$edate' and  c.case_no!=''
				AND ( UPPER ( status ) = 'P') "); 
 */

				$stpp11211 = $db->prepare("WITH cte_1 AS (
					SELECT
						( filing_no ),		
						MAX ( CAST ( suit_amount AS DOUBLE PRECISION ) ) AS suit_amount 
					FROM
					$allSchemaNmae.account_details 
					WHERE
						suit_amount IS NOT NULL 
						AND suit_amount != '0' 
						AND filing_no IS NOT NULL 
						AND suit_amount != '' 
					GROUP BY
						filing_no
					)	
				SELECT sum
					( A.suit_amount ) 
				FROM
					(
					SELECT
						c.filing_no,aa.suit_amount 
					FROM
					$allSchemaNmae.case_detail AS C INNER JOIN cte_1 AS aa ON C.filing_no = aa.filing_no 
					WHERE
						( case_no IS NOT NULL AND LENGTH ( case_no ) = '15' ) 
						AND regis_date IS NOT NULL 
						AND $case_type_in
						AND regis_date IS NOT NULL  AND regis_date <= '$edate'
						AND ( UPPER ( status ) = 'P' OR ( status = 'D' AND disposal_date >= '$endDate' ) ) UNION ALL
					SELECT
						c.filing_no ,aa.suit_amount
					FROM
					$allSchemaNmae.case_detail AS C INNER JOIN cte_1 AS aa ON C.filing_no = aa.filing_no 
					WHERE
						( case_no IS NOT NULL AND LENGTH ( case_no ) = '15' ) 
						AND regis_date IS NOT NULL 
						AND $case_type_in
						AND ( regis_date BETWEEN '$startDate' and '$endDate' ) 
						AND ( UPPER ( status ) IN ( 'P', 'D' ) ) EXCEPT
					SELECT
						c.filing_no ,aa.suit_amount
					FROM
					$allSchemaNmae.case_detail AS C INNER JOIN cte_1 AS aa ON C.filing_no = aa.filing_no 
					WHERE
						( case_no IS NOT NULL AND LENGTH ( case_no ) = '15' ) 
						AND regis_date IS NOT NULL 
						AND $case_type_in
						AND UPPER ( status ) = 'D' 
					AND ( disposal_date BETWEEN '$startDate' and '$endDate' ) 
					) AS A");
				 
				  

				$stpp11211->execute();
				$final_suit = $stpp11211->fetchColumn();
		   
					}



					
					//$final_suit=$total1+$ttotal1+$totall1+$total123+$total12+$total13;
					//$final_total=$totaldd2+$ttotaldd2+$total3+$total43+$ttotal4+$total21;
					$t_suit=$t_suit+$final_suit;
					$t_total=$t_total+$final_total;
				
					?>
					<tr><?php if ($schemas!= '1' and  ( $userid=="31" or $userid=='1458' or $userid=='1465' or $userid=='1467' or $userid=='1468' or $userid=='1469')) {?>
					<td><?php 
					$sql="select short_name from initilization where  schema_id=?";
					$sth = $db->prepare($sql);
					$sth->bindParam(1, $schemas, PDO::PARAM_INT);
					$sth->execute();
					$drat_name = htmlentities(htmlspecialchars($sth->fetchColumn()));	
					echo strtoupper($drat_name);
					?></td><?php }?>
					
					<td><?php 
					if ($userid=="31"  or $userid=='1458' or $userid=='1465' or $userid=='1467' or $userid=='1468' or $userid=='1469') {
					if($allSchemaNmae=='delhi'){
					echo strtoupper('DELHI DRT 1');
					}else{
					echo strtoupper($allSchemaNmae1);
					}
					}
					else
					{
					echo strtoupper($allSchemaNmae);
					}
					?></td>
					
					<td><table width="146" class="table table-condensed table-bordered">
							<td width="33" align="right">
						<?php echo htmlspecialchars($totaldd2) ;?>
						</td>
						<td width="33" align="right">
						<?php echo htmlspecialchars(htmlentities(number_format((float)$total1 / 10000000, 2, '.', '')));
					$totaldd2="";
					$total1="";
					?></td></table>
					</td>
					<td><table width="146" class="table table-condensed table-bordered">
							<td width="33" align="right">
						<?php echo htmlspecialchars($ttotaldd2) ;?>
						</td>
						<td width="33" align="right">
						<?php echo htmlspecialchars(htmlentities(number_format((float)$ttotal1 / 10000000, 2, '.', '')));
					$ttotaldd2="";
					$ttotal1="";
					?></td></table>
					</td>
					<td><table width="146" class="table table-condensed table-bordered">
							<td width="33" align="right">
						<?php echo htmlspecialchars($total3) ;?>
						</td>
						<td width="33" align="right">
						<?php echo htmlspecialchars(htmlentities(number_format((float)$totall1 / 10000000, 2, '.', '')));
					$total3="";
					$totall1="";
					?></td></table>
					</td>
					<td>
					<table width="146" class="table table-condensed table-bordered">
							<td width="33" align="right">
						<?php echo htmlspecialchars($total43) ;?>
						</td>
						<td width="33" align="right">
						<?php echo htmlspecialchars(htmlentities(number_format((float)$total123 / 10000000, 2, '.', '')));
					$total43="";
					$total123="";
					?></td></table>
					</td>
					<td>
					<table width="146" class="table table-condensed table-bordered">
							<td width="33" align="right">
						<?php echo htmlspecialchars($ttotal4) ;?>
						</td>
						<td width="33" align="right">
						<?php echo htmlspecialchars(htmlentities(number_format((float)$total12 / 10000000, 2, '.', '')));
					$ttotal4="";
					$total12="";
					?></td></table>
					</td>
					<td>
					<table width="146" class="table table-condensed table-bordered">
							<td width="33" align="right">
                                        <?php 
    						 $endDate=$edate4;
		$filing_no1=($endDate.'/'.$allSchemaNmae.'/'.$final_total.'/'.$case_type.'/'.$date_type);
							$filing_no=base64_encode($filing_no1);
							
					?>


<a href="#" onClick="javascript:void window.open('../mis/agewise_report_above_10.php?diary_no=<?php echo $filing_no; ?>','1','width=700,height=500,scrollbars=1,resizable=1,left=0,top=0,');return false;">
<?php echo htmlspecialchars($total21) ;?></a>
						</td>
						<td width="33" align="right">
						<?php echo htmlspecialchars(htmlentities(number_format((float)$total13 / 10000000, 2, '.', '')));
					$total21="";
					$total13="";
					?></td></table>
					</td>
					<td>
					<table width="146" class="table table-condensed table-bordered">
					<?php 
							list($dd,$mm,$yyyy)=explode('/',$edateeeee);
    						 $endDate="$yyyy-$mm-$dd";
							
							$filing_no1=($endDate.'/'.$allSchemaNmae.'/'.$final_total.'/'.$case_type.'/'.$date_type);
							$filing_no=base64_encode($filing_no1);
							
					?>
							<td width="33" align="right">
						
						<a href="#" onClick="javascript:void window.open('../order/age_report.php?diary_no=<?php echo $filing_no; ?>','1','width=700,height=500,scrollbars=1,resizable=1,left=0,top=0,');return false;">
				<?php echo htmlspecialchars($final_total) ;?></a>
						</td>
						<td width="33" align="right">
						<?php echo htmlspecialchars(htmlentities(number_format((float)$final_suit / 10000000, 2, '.', '')));
					$final_total="";
					$final_suit="";
					?></td></table>
					</td>
					<!--<td>
					<table width="146" class="table table-condensed table-bordered">
							<th width="33" align="center">
						<?php echo htmlspecialchars($total22) ;?>
						</th>
						<th width="33" align="center">
						<?php echo htmlspecialchars(htmlentities(number_format((float)$total14 / 10000000, 2, '.', '')));
					$total22="";
					$total14="";
					?></th></table>
					</td>-->
					</tr>
					<?php } ?>
					<tr><?php if ($schemas!= '1' and ( $userid=="31" or $userid=='1458' or $userid=='1465' or $userid=='1467' or $userid=='1468' or $userid=='1469')) {?><td>&nbsp;</td><?php }?>
						<td><font color="#0000FF"><b>GRAND TOTAL</b></font></td>
						<td>
						<table width="146" id="content" class="table table-bordered table-condensed">
							<td width="33" align="right"><?php echo $tc;?></td>
<td width="33" align="right"><?php echo htmlspecialchars(htmlentities(number_format((float)$ts / 10000000, 2, '.', '')));
$ts="";
$tc="";
?></td>
							</table>
					  </td><td>
							<table width="146" id="content" class="table table-bordered table-condensed">
							<td width="33" align="right"><?php echo $tc1;?></td>
							<td width="33" align="right"><?php echo htmlspecialchars(htmlentities(number_format((float)$ts1 / 10000000, 2, '.', '')));
				$tc1="";
				$ts1="";?></td>
							
							</table>
		</td><td><b>
		<table width="146" id="content" class="table table-bordered table-condensed">
							<td width="33" align="right"><?php echo $tc2;?></td>
							<td width="33" align="right"><?php echo htmlspecialchars(htmlentities(number_format((float)$ts2 / 10000000, 2, '.', '')));
				$tc2="";
				$ts2="";?></td>
							
			</table>
							</b></td>
							<td><b>
		<table width="146" id="content" class="table table-bordered table-condensed">
							<td width="33" align="right"><?php echo $tc3;?></td>
							<td width="33" align="right"><?php echo htmlspecialchars(htmlentities(number_format((float)$ts3 / 10000000, 2, '.', '')));
				$tc3="";
				$ts3="";?></td>
							
							</table>
							</b></td>
							<td><b>
		<table width="146" id="content" class="table table-bordered table-condensed">
							<td width="33" align="right"><?php echo $tc4;?></td>
							<td width="33" align="right"><?php echo htmlspecialchars(htmlentities(number_format((float)$ts4 / 10000000, 2, '.', '')));
				$tc4="";
				$ts4="";?></td>
							
							</table>
							</b></td>
							<td><b>
		<table width="146" id="content" class="table table-bordered table-condensed">
							<td width="33" align="right"><?php echo $tc5;?></td>
							<td width="33" align="right"><?php echo htmlspecialchars(htmlentities(number_format((float)$ts5 / 10000000, 2, '.', '')));
				$tc5="";
				$ts5="";?></td>
							
							</table>
							</b></td>
							<td><b>
		<table width="146" id="content" class="table table-bordered table-condensed">
							<td width="33" align="right"><?php echo $t_total;?></td>
							<td width="33" align="right"><?php echo htmlspecialchars(htmlentities(number_format((float)$t_suit / 10000000, 2, '.', '')));
				$t_total="";
				$t_suit="";			?></td>
							
							</table>
							</b></td>
							
					  </tr>
					</tbody>
					
			<?php }?>	
		  </table>	
		  </div>
		</div>
</form> 
				
				 <br><br>  <br><br> 
<?php include_once("./_layout/_footer.php")?>

