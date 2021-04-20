miniWebRTC
===

A tiny serverless* WebRTC boilerplate with automatic P2P connection,
<br>
forked from https://github.com/xem/miniWebRTC
<br>
inspired by https://github.com/cjb/serverless-webrtc and https://github.com/webrtc/samples
<br>
Using https://gitlab.com/jonas.jasas/httprelay to automate offer/answer exchange.

*no signaling server, but the STUN server is still necessary and used.

---

Principle
====

- bob asks his ip to a stun server and sends it to alice via an HTTP Relay (Create)
- alice receive bob offer and asks her ip to the stun server and sends it to bob via an HTTP Relay (Join)
- both can communicate with webrtc

