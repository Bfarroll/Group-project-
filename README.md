# Group-project-
This repository will be for our group project 

<?php
define("DB_SERVER", "localhost");
define("DB_USER", "bfarroll");
define("DB_PASS", "AWD4CY4DQQs=");
define("DB_NAME", "bfarroll");



$connection = mysqli_connect(DB_SERVER, DB_USER, DB_PASS, DB_NAME);

if(mysqli_connect_errno()) 

{
die("Database connection failed: " . 
mysqli_connect_error() . 
" (" . mysqli_connect_errno() . ")"
);
}

?>

<?php

$query ="SELECT FROM * users " ;
$result = mysqli_query ($connect , $query)); 

if (!$result) {
    
    
}


?>

<?php

 function redirectTo($newlocation) {
     header("Location: " . $newlocation);
     exit;
 }

?>

<?php
 session_start(); 

function message () {
    if(isset($_SESSION["message"])) {
        $output = "<div class=\"message-box\">";
        
        $output .= $_SESSION["message"]; 
        $output .= "</div>";
        
        $_SESSION["message"] = null;
            
            return $output;
        
    } 
    
}

?>

