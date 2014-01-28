xinetd is a wonderfully solid old tool for protecting hosts.

In the ipv6 age, it seems needed again, and in the hostile
environment of today's ipv4 internet, and the fact that
many essential services startup and maintain their own
ports (web servers), it seems like a good idea to
be able to detect various forms of attack and do
something protective to protect the whole router.

Most firewall implementations merely drop packets
they don't want, but do nothing to block the offending
host.

The thought at the moment is merely to be able to
call a script that "does something" upon receiving
a connection attempt on a port that denys access
for some reason.

A simple implementation would use ipsets to manage
a list of blocked hosts, which the firewall would
leverage to protect access to other vulnerable
services and networks.

