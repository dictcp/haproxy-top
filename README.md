haproxy-top
==============================

haproxy-top is a top-like monitoring tool for HAProxy 1.4 and has few package dependencies (socat, curl, watch, moreutils).

It support monitors mutliple haproxy instances.

Usage
------------------------------
- connect to local socket
  - `haproxy-top /var/run/haproxy/haproxy.sock`
- connect to remote http monitor-url
  - `haproxy-top http://127.0.0.1:20000/haproxy-monitor`
  - OR shorthand url `haproxy-top :20000/haproxy-monitor`
- connect to multiple instances
  - `haproxy-top :20000/haproxy-monitor :20001/haproxy-monitor`

