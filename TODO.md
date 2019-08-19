
# TO DO

This repo is a work-in-progress.  These are notes about parts of RTMP that aren't well-defined in public documentation

## Different transports

- [ ] Flow vs Chunk Stream
- [ ] HTTP/HTTPS

Notes from RTMFP Spec:
* An RTMP message is mapped onto a lower transport layer, such as RTMP Chunk Stream [RTMP] or RTMFP.
* RTMP Chunk Stream Protocol Control messages (message types 1, 2, 3, 5, and 6) are not used when transporting RTMP messages in RTMFP


## Data

- [ ] overview of command message syntax
- [ ] call vs send
- [ ] reference AMF encoding
- [ ] specific messages aren't clearly specified (see below)


### Connect
connect (section 7.2.1.1 in [RTMP spec](https://www.adobe.com/content/dam/acom/en/devnet/rtmp/pdf/rtmp_specification_1.0.pdf))
* `tcUrl` needs clarification, currently listed as "URL of the Server" but it also specifies the protocol and app path `protocol://servername:port/appName/appInstance` with the only example given as `rtmp://localhost:1935/testapp/instance1`
  * clarify that URL scheme must be `rtmp` -- this message should be the same no matter what the underlying transport is
  * TODO: explain app name and instance






