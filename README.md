# /etc/knot-resolver

Basic config for knot-resolver, pieced togheter from various sources.

Needs an additional file in kresd.conf.d where we define hostname, ipv4 and ipv6
addresses to bind to.

kresd.conf.d/10-local.conf

fqdn = ''
ipv4 = ''
ipv6 = ''

