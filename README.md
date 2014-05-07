#PHP Barcode Generator Class Code 39

Here is an easy to use PHP barcode generator class for code 39 barcodes.


Requirements: PHP Web server and [GD Library](http://php.net/manual/en/book.image.php) (Graphics Library). 


The PHP class will create a GIF barcode image or save a GIF barcode image file, here is an example:

    // include Barcode39 class 
    include "Barcode39.php"; 
    
    // set Barcode39 object 
    $bc = new Barcode39("Shay Anderson"); 
    
    // display new barcode 
    $bc->draw();


This example will output this barcode: 

![barcode39](doc/barcode39.gif "barcode39")



You can also easily adjust the barcode bar sizes and text size:

    // set object 
    $bc = new Barcode39("123-ABC"); 
    
    // set text size 
    $bc->barcode_text_size = 5; 
    
    // set barcode bar thickness (thick bars) 
    $bc->barcode_bar_thick = 4; 
    
    // set barcode bar thickness (thin bars) 
    $bc->barcode_bar_thin = 2; 
    
    // save barcode GIF file 
    $bc->draw("barcode.gif");


This example will save this barcode as "barcode.gif": 

![barcode39](doc/php-barcode39.gif "barcode39")

