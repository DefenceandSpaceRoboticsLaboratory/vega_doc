# vega_doc
<h><b>Documentation of vega board</b></h>
<p>
  <li>open terminal</li>
  <li>connect the vega board to the laptop</li>
  <li>goto vega-sdk/examples/<path to the file ou want to upload></li>
  <li>suppose: $ cd home/vega-sdk/examples/gpio/led_breathing/</li>
  <li>$ make</li>
  <li>if the above step shows make done, great!</li>
  <li>if shows something in 3 line : 
    <ul>probably it is already complied, try uploading directly</ul>
    <ul>reconnect the board, close all the terminal and repeat the process again</ul>
  </li>
  <li>after compilation open another tab on the terminal</li>
  <li>$ sudo minicom thejas32</li>
  <li>if shows error dev/tty USB1 locked, then try
    <ul>$ sudo killall -9 minicom</ul>
    <ul>then run $ sudo minicom thejas32, if this yet doesn't work</ul>
    <ul>$ sudo minicom -s -c on</ul>
    <ul>in minicom check if port is dev/tty//USB1 and baud rate is 115200 8N1, if not change to these</ul>
    <ul>save this setup as dfl and exit</ul>
   </li>
  <li>this should run the upload console if not then run $ sudo minicom thejas32</li>
  <li>check if continuous c is coming</li>
  <li>if yes, then press cntrl A S</li>
  <li>xmodem</li>
  <li>select the .bin file of the program (use space tab)</li>
  <li>enter. Program should be uploaded. Don't do it too fast, you might have repeat this all over again :D</li>
  <li>after uploading press enter and to start the execution press enter again</li>
  <li>if you get any error inbetween, restart the process again</li>
  -------------------note down any new error below-------------------------------------
  
    
