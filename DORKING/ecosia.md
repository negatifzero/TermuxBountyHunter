```text

General info:

The same query might return different results: The sequence and amount of results can be different. It seems to depend on how many were found, if there are only few, then results shall be the same.
It looks like the inurl: operator is not supported. There is a chance though that it has some unusual name.
Operator site:
Does not accept * wildcard (neither in subdomains nor in path). Searches in subdomains: Eg site:google.com would return www.google.com, support.google.com, etc.

Operator filetype:
Returns results for at least some extensions (eg pdf, txt, zip). It either does not recognize or blocks requests for some extensions (eg csv).

Operator intitle:
Put compound strings into quotes for better results (eg intitle:"some good title" instead of intitle:some good title). Seems to search for related strings (eg can add/replace delimeters). Sometimes returns unrelated results.
´´´
