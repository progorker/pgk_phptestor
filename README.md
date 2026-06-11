```
=======_========_____=======_============
  _ __| |_  _ _|_   _|__ __| |_ ___ _ _ 
 | '_ \ ' \| '_ \| |/ -_|_-<  _/ _ \ '_|
 | .__/_||_| .__/|_|\___/__/\__\___/_|  
=|_|=======|_|===========================
     Unit testing framework for PHP
=========================================


-|_|-----------|___/----------------------
             Alpha Testing
------------------------------------------


-|_|-------|_|---------------------------
      Using unit testing framework
-----------------------------------------

+ Simple sample from phpTestorCheck [ https://github.com/progorker/phptestorcheck ]
-----
global $g_testor_dir, $g_token, $g_suite_id;

require_once __DIR__ . '/tests-config.php';
require_once $g_testor_dir . '/testor.php';

\phptestor\api_testor_startup();
require_once __DIR__ . '/tests-source.php';
require_once __DIR__ . '/tests-setup.php';

function g_run_tests() {
  global $g_token, $g_suite_id;
  test_numbers( $g_token, $g_suite_id );
  test_strings( $g_token, $g_suite_id );
}

g_run_tests();
\phptestor\api_testor_shutdown();
-----


-|_|-------|_|---------------------------
         Getting manual page
-----------------------------------------

$) export PHP_TESTOR_DIR=""
$) export MODULE="mytestor"
$) export KIND="procedure"
$) export CODE="api_testor_suite"
$) cd $PHP_TESTOR_DIR && php ./man.php $MODULE $KIND $CODE

 
-|_|-------|_|---------------------------
         Getting code pattern
-----------------------------------------

$) export PHP_TESTOR_DIR=""
$) export MODULE="mytestor"
$) export KIND="procedure"
$) export CODE="api_testor_suite"
$) export VARIANT="scrp"
$) cd $PHP_TESTOR_DIR && php ./pattern.php $MODULE $KIND $CODE $VARIANT

```
