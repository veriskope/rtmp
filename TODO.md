
# document different transports in more detail

Notes from RTMFP Spec, clarify in RTMP Spec?
* An RTMP message is mapped onto a lower transport layer, such as RTMP Chunk Stream [RTMP] or RTMFP.
* RTMP Chunk Stream Protocol Control messages (message types 1, 2, 3, 5, and 6) are not used when transporting RTMP messages in RTMFP


RTMP details

* connect (section 7.2.1.1 in [RTMP spec](https://www.adobe.com/content/dam/acom/en/devnet/rtmp/pdf/rtmp_specification_1.0.pdf))
* `tcUrl` needs clarification, currently listed as "URL of the Server" but it also specifies the protocol and app path `protocol://servername:port/appName/appInstance` with the only example given as `rtmp://localhost:1935/testapp/instance1`
  * clarify protocol must be `rtmp` or `rtmps`
  * explain app name and instance






