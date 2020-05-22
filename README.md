# fluent-bit-config
A small implementation of fluent-bit on my system

I used Windows 8.1, since I was receiving error on Ubuntu 18.04 LTS reported [here](https://github.com/fluent/fluent-bit/issues/2194)

1. Check the version.
<img src="./images/version.png">

2. Built the configuration File as [fluent-basic](/fluent-basic.conf)
I have used the required easy format to not to overload this file by including different [input.conf](/input.conf) and 
[output.conf](/output.conf)


3. Generated the random stream at the output 
<img src="./images/config.png">


4. Streams are visible and port listening of 445 is also visible at 
<img src="./images/port_listening.png">

5. ```CMD``` output after ```curl -s http://127.0.0.1:445 | jq``` was

```
{
  "fluent-bit": {
    "version": "1.4.4",
    "edition": "Community",
    "flags": [
      "FLB_HAVE_PARSER",
      "FLB_HAVE_RECORD_ACCESSOR",
      "FLB_HAVE_STREAM_PROCESSOR",
      "FLB_HAVE_TLS",
      "FLB_HAVE_SIGNV4",
      "FLB_HAVE_SQLDB",
      "FLB_HAVE_METRICS",
      "FLB_HAVE_HTTP_SERVER",
      "FLB_HAVE_FORK",
      "FLB_HAVE_TIMESPEC_GET",
      "FLB_HAVE_GMTOFF",
      "FLB_HAVE_UNIX_SOCKET",
      "FLB_HAVE_PROXY_GO",
      "FLB_HAVE_SYSTEM_STRPTIME",
      "FLB_HAVE_LIBBACKTRACE",
      "FLB_HAVE_REGEX",
      "FLB_HAVE_UTF8_ENCODER",
      "FLB_HAVE_LUAJIT",
      "FLB_HAVE_C_TLS",
      "FLB_HAVE_ACCEPT4",
      "FLB_HAVE_INOTIFY"
    ]
  }
}
```
