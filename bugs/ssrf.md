## SSRF:-
### TEST cases for SSRF attack:-
1:- # Basic SSRF against the local server. Craft a simple payload 'http://localhost/admin' where it takes a url as a parameter.
2:- # Basic SSRF against another back-end system. Another type of trust relationship that often arises with server-side request forgery is where the application server is able to interact with other back-end systems that are not directly reachable by users.hese systems often have non-routable private IP addresses. 
3:-# SSRF with blacklist-based input filter. if the localhost 127.0.0.1 is blaclisted we can use 127.1 as well.
4:- # SSRF with whitelist-based input filter. You can embed credentials in a URL before the hostname, using the  `@`  character. For example:  `https://expected-host@evil-host`.   You can use the  `#`  character to indicate a URL fragment. For example:  `https://evil-host#expected-host`. 
5:- # SSRF with filter bypass via open redirection vulnerability.
6:- # Blind SSRF with out-of-band detection.
