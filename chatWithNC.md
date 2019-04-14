You can use netcat,

On box1: nc -l 3333

On box2: nc $IP 3333, where $IP equals the local IP address of the first system.

Once you do this, in the same box (box2) , type something and press enter. Take a look on your other box.


