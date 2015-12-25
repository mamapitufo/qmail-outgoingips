# qmail-outgoingips

With this patch `qmail-remote` is modified to bind to different local ip
addresses depending on the domain part in the sender argument. The mapping
between ip addresses and domains is specified in a new control file:
`control/outgoingips`. The HELO string will be set to the domain part if there
is a match.

Based on [outgoingip.patch](http://qmail.org./outgoingip.patch). Let me know if
you find it useful.

This software is in the public domain.

