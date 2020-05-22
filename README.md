# fluent-bit-config
A small implementation of fluent-bit on my system

I used Windows package, since I was receiving error on Ubuntu 18.04 LTS reported [here](https://github.com/fluent/fluent-bit/issues/2194)

Check the <img src="./images/version.png">

Built the configuration File as fluent-basic <img src="/fluent-basic.conf">
I have used the required easy format to not to overload this file by opening different [input.conf](/input.conf) and 
[output.conf](/output.conf)


Generated the random stream at the output <img src="./images/config.png">


Streams are visible and port listening of 445 is also visible at <img src="./images/port_listening.png">
