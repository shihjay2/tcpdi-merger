# tcpdi-merger
TCPDI-merger. Merge PDF files using the TCPDI library.

###Make it work!
1. `composer require shihjay2/tcpdi-merger`
2. Copy the example directory.
3. Run it!

###Example code
```
<?php

    require 'vendor/autoload.php';

    use shihjay2\tcpdi_merger\MyTCPDI;
    use shihjay2\tcpdi_merger\Merger;            

    $m = new Merger(true);
    $m->addFromFile("example/A.pdf");
    $m->addFromFile("example/lorem.pdf");
    $m->addFromFile("example/PDF17.pdf");
    $m->addFromFile("example/PDF16.pdf");
    $m->merge();
    $m->save("example/merged-document.pdf");

?>
```
