This tutorial is written to help people understand some of the basics of shell script programming (aka shell scripting), and hopefully to introduce some of the possibilities of simple but powerful programming available. 
To start the project , use any text editor and save it as .sh file.

#!/bin/bash
echo "Hello World!"

To run
cd src/
$ chmod +x ./hello_world.sh
$ ./hello_world.sh

Variable declaration
intVar="233"

To run
echo $intVar

Basic Operations
a=233
b=666

val1=`expr $a + $b`
echo "Total value: $val1"
