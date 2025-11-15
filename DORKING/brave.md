```text
General info:

There seems to be no () grouping operator, so AND/OR must be used to mimic it.
Combinations of single queries might return different results than single queries.
Example:
'site:sub.2ndld.tld ext:txt OR site:sub.2ndld.tld filetype:txt'
compound query may return more results than 2 separate:
'site:sub.2ndld.tld ext:txt', 'site:sub.2ndld.tld filetype:txt'
Apparently the engine supports inurl: operator to some degree. But there is no info about it in the official docs.
Operator site:
Searches in subdomains even if only 2nd level domain and TLD are provided.

The space between colon and host name plays a role:

site:news.google.com would return results, which have the "news" subdomain.
site: news.google.com would not just return different subdomains but also different hosts.
The * wildcard is supported:

site: *.google.com would return results with different subdomins. Note that there must be a space between colon and star, otherwise, if there is no space, the * itself would be considered a subdomain, hence there will be no results.
site: *.google.com/a* would return somewhat different results than the one from above. It looks like the * in the path is supported to some extent but it seems unreliable.
Operator filetype:
Returns results based on content rather than file extension.
If it does not find anything relevant it might suggest you smth similar:
site:2ndld.tld filetype:pps => Showing results for site:2ndld.tld filetype:ppt

Operator ext:
Returns results based on extension rather than file content.
If it does not find anything relevant it might suggest you smth similar:
site:2ndld.tld ext:xlsm => Showing results for site:2ndld.tld ext:xlsx
It looks like it not only tries to find a similar extension, but also uses the operator itself to find "similar" results:
site:2ndld.tld ext:action => Showing results for site:2ndld.tld extraction

Operator intitle:
Put compound strings into quotes for better results (eg intitle:"some good title" instead of intitle:some good title).
```
