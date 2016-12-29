# MCP39F521
This is simple SIP client to make SIP calls to local ASTERISK VoIP server.
Desigend as backgroud daemon for MythTV frontend.
Script is controlled by semaphore files located in '/tmp/ dir.

Script checks for following semaphore files:

  '/tmp/make-call-<num>.sem'   - make call to <num>

  '/tmp/pickup.sem'            - answer incomming call

  '/tmp/voice-mail.sem'        - answer call with voide mail

  '/tmp/voice-mail-listen.sem' - answer call with voice mail and listen when records

  '/tmp/reject.sem'            - reject call

  '/tmp/hangup.sem'            - end call

  '/tmp/exit.sem'              - deregister from server and exit

Script requires pjsip and pjsip-python
