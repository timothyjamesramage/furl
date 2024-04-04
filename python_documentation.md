# furl/common.py


# Comments
| Comment | File | Line |
|---------|------|------|
| **# -*- coding: utf-8 -*-** | furl/common.py | 1 |
| **#** | furl/common.py | 3 |
| **# furl - URL manipulation made simple.** | furl/common.py | 4 |
| **#** | furl/common.py | 5 |
| **# Ansgar Grunseid** | furl/common.py | 6 |
| **# grunseid.com** | furl/common.py | 7 |
| **# grunseid@gmail.com** | furl/common.py | 8 |
| **#** | furl/common.py | 9 |
| **# License: Build Amazing Things (Unlicense)** | furl/common.py | 10 |
| **#** | furl/common.py | 11 |

## Function Names and Associated Docstring
```python
def callable_attr(obj, attr):
"""

"""
```
```python
def is_iterable_but_not_string(v):
"""

"""
```
# furl/compat.py



# Comments
| Comment | File | Line |
|---------|------|------|
| **# -*- coding: utf-8 -*-** | furl/compat.py | 1 |
| **#** | furl/compat.py | 3 |
| **# furl - URL manipulation made simple.** | furl/compat.py | 4 |
| **#** | furl/compat.py | 5 |
| **# Ansgar Grunseid** | furl/compat.py | 6 |
| **# grunseid.com** | furl/compat.py | 7 |
| **# grunseid@gmail.com** | furl/compat.py | 8 |
| **#** | furl/compat.py | 9 |
| **# License: Build Amazing Things (Unlicense)** | furl/compat.py | 10 |
| **#** | furl/compat.py | 11 |

## Function Names and Associated Docstring
```python
def __str__(self):
"""

"""
```
# furl/furl.py



# Comments
| Comment | File | Line |
|---------|------|------|
| **# -*- coding: utf-8 -*-** | furl/furl.py | 1 |
| **#** | furl/furl.py | 3 |
| **# furl - URL manipulation made simple.** | furl/furl.py | 4 |
| **#** | furl/furl.py | 5 |
| **# Ansgar Grunseid** | furl/furl.py | 6 |
| **# grunseid.com** | furl/furl.py | 7 |
| **# grunseid@gmail.com** | furl/furl.py | 8 |
| **#** | furl/furl.py | 9 |
| **# License: Build Amazing Things (Unlicense)** | furl/furl.py | 10 |
| **#** | furl/furl.py | 11 |
| **# Map of common protocols, as suggested by the common protocols included in** | furl/furl.py | 33 |
| **# urllib/parse.py, to their default ports. Protocol scheme strings are** | furl/furl.py | 34 |
| **# lowercase.** | furl/furl.py | 35 |
| **#** | furl/furl.py | 36 |
| **# TODO(Ans): Is there a public map of schemes to their default ports? If not,** | furl/furl.py | 37 |
| **# create one? Best I (Ansgar) could find is** | furl/furl.py | 38 |
| **#** | furl/furl.py | 39 |
| **#   https://gist.github.com/mahmoud/2fe281a8daaff26cfe9c15d2c5bf5c8b** | furl/furl.py | 40 |
| **#** | furl/furl.py | 41 |
| **# TODO(grun): Support IDNA2008 via the third party idna module. See** | furl/furl.py | 117 |
| **# https://github.com/gruns/furl/issues/73#issuecomment-226549755.** | furl/furl.py | 118 |
| **# Prune duplicates and characters not in <safe_charset>.** | furl/furl.py | 155 |
| **#** | furl/furl.py | 167 |
| **# TODO(grun): Update some of the regex functions below to reflect the fact that** | furl/furl.py | 168 |
| **# the valid encoding of Path segments differs slightly from the valid encoding** | furl/furl.py | 169 |
| **# of Fragment Path segments. Similarly, the valid encodings of Query keys and** | furl/furl.py | 170 |
| **# values differ slightly from the valid encodings of Fragment Query keys and** | furl/furl.py | 171 |
| **# values.** | furl/furl.py | 172 |
| **#** | furl/furl.py | 173 |
| **# For example, '?' and '#' don't need to be encoded in Fragment Path segments** | furl/furl.py | 174 |
| **# but they must be encoded in Path segments. Similarly, '#' doesn't need to be** | furl/furl.py | 175 |
| **# encoded in Fragment Query keys and values, but must be encoded in Query keys** | furl/furl.py | 176 |
| **# and values.** | furl/furl.py | 177 |
| **#** | furl/furl.py | 178 |
| **# Perhaps merge them with URLPath, FragmentPath, URLQuery, and** | furl/furl.py | 179 |
| **# FragmentQuery when those new classes are created (see the TODO** | furl/furl.py | 180 |
| **# currently at the top of the source, 02/03/2012).** | furl/furl.py | 181 |
| **#** | furl/furl.py | 182 |
| **# RFC 3986 (https://www.ietf.org/rfc/rfc3986.txt)** | furl/furl.py | 184 |
| **#** | furl/furl.py | 185 |
| **#   unreserved  = ALPHA / DIGIT / "-" / "." / "_" / "~"** | furl/furl.py | 186 |
| **#** | furl/furl.py | 187 |
| **#   pct-encoded = "%" HEXDIG HEXDIG** | furl/furl.py | 188 |
| **#** | furl/furl.py | 189 |
| **#   sub-delims  = "!" / "$" / "&" / "'" / "(" / ")"** | furl/furl.py | 190 |
| **#                 / "*" / "+" / "," / ";" / "="** | furl/furl.py | 191 |
| **#** | furl/furl.py | 192 |
| **#   pchar       = unreserved / pct-encoded / sub-delims / ":" / "@"** | furl/furl.py | 193 |
| **#** | furl/furl.py | 194 |
| **#   === Path ===** | furl/furl.py | 195 |
| **#   segment     = *pchar** | furl/furl.py | 196 |
| **#** | furl/furl.py | 197 |
| **#   === Query ===** | furl/furl.py | 198 |
| **#   query       = *( pchar / "/" / "?" )** | furl/furl.py | 199 |
| **#** | furl/furl.py | 200 |
| **#   === Scheme ===** | furl/furl.py | 201 |
| **#   scheme      = ALPHA *( ALPHA / DIGIT / "+" / "-" / "." )** | furl/furl.py | 202 |
| **#** | furl/furl.py | 203 |
| **# Avoid incorrect scheme extraction with url.find(':') when other URL** | furl/furl.py | 248 |
| **# components, like the path, query, fragment, etc, may have a colon in** | furl/furl.py | 249 |
| **# them. For example, the URL 'a?query:', whose query has a ':' in it.** | furl/furl.py | 250 |
| **# 'netloc' in Python parlance, 'authority' in RFC 3986 parlance.** | furl/furl.py | 278 |
| **# urlsplit() parses URLs differently depending on whether or not the URL's** | furl/furl.py | 296 |
| **# scheme is in any of** | furl/furl.py | 297 |
| **#** | furl/furl.py | 298 |
| **#   urllib.parse.uses_fragment** | furl/furl.py | 299 |
| **#   urllib.parse.uses_netloc** | furl/furl.py | 300 |
| **#   urllib.parse.uses_params** | furl/furl.py | 301 |
| **#   urllib.parse.uses_query** | furl/furl.py | 302 |
| **#   urllib.parse.uses_relative** | furl/furl.py | 303 |
| **#** | furl/furl.py | 304 |
| **# For consistent URL parsing, switch the URL's scheme to 'http', a scheme** | furl/furl.py | 305 |
| **# in all of the aforementioned uses_* lists, and afterwards revert to the** | furl/furl.py | 306 |
| **# original scheme (which may or may not be in some, or all, of the the** | furl/furl.py | 307 |
| **# uses_* lists).** | furl/furl.py | 308 |
| **# Detect and preserve the '//' before the netloc, if present. E.g. preserve** | furl/furl.py | 314 |
| **# URLs like 'http:', 'http://', and '///sup' correctly.** | furl/furl.py | 315 |
| **# For consistent URL joining, switch the base URL's scheme to** | furl/furl.py | 339 |
| **# 'http'. urllib.parse.urljoin() behaves differently depending on the** | furl/furl.py | 340 |
| **# scheme. E.g.** | furl/furl.py | 341 |
| **#** | furl/furl.py | 342 |
| **#   >>> urllib.parse.urljoin('http://google.com/', 'hi')** | furl/furl.py | 343 |
| **#   'http://google.com/hi'** | furl/furl.py | 344 |
| **#** | furl/furl.py | 345 |
| **# vs** | furl/furl.py | 346 |
| **#** | furl/furl.py | 347 |
| **#   >>> urllib.parse.urljoin('asdf://google.com/', 'hi')** | furl/furl.py | 348 |
| **#   'hi'** | furl/furl.py | 349 |
| **# Example #1: ['a',''] + ['b'] == ['a','b']** | furl/furl.py | 389 |
| **# Example #2: ['a',''] + ['','b'] == ['a','','b']** | furl/furl.py | 390 |
| **# Example: ['a'] + ['','b'] == ['a','b']** | furl/furl.py | 393 |
| **# ('/a/b/c', 'b/c') -> '/a/'** | furl/furl.py | 407 |
| **# ('/a/b/c', '/b/c') -> '/a'** | furl/furl.py | 409 |
| **# [''] means a '/', which is properly represented by ['', ''].** | furl/furl.py | 417 |
| **# From RFC 3986:** | furl/furl.py | 483 |
| **#   segment       = *pchar** | furl/furl.py | 484 |
| **#   pchar         = unreserved / pct-encoded / sub-delims / ":" / "@"** | furl/furl.py | 485 |
| **#   unreserved    = ALPHA / DIGIT / "-" / "." / "_" / "~"** | furl/furl.py | 486 |
| **#   sub-delims    = "!" / "$" / "&" / "'" / "(" / ")"** | furl/furl.py | 487 |
| **#                       / "*" / "+" / "," / ";" / "="** | furl/furl.py | 488 |
| **# Preserve the opening '/' if one exists already (self.segments** | furl/furl.py | 542 |
| **# == ['']).** | furl/furl.py | 543 |
| **# In Python 3, utf8() returns Bytes objects that must be decoded into** | furl/furl.py | 681 |
| **# strings before they can be passed to unquote(). In Python 2, utf8()** | furl/furl.py | 682 |
| **# returns strings that can be passed directly to urllib.unquote().** | furl/furl.py | 683 |
| **# From RFC 3986:** | furl/furl.py | 895 |
| **#   query       = *( pchar / "/" / "?" )** | furl/furl.py | 896 |
| **#   pchar       = unreserved / pct-encoded / sub-delims / ":" / "@"** | furl/furl.py | 897 |
| **#   unreserved  = ALPHA / DIGIT / "-" / "." / "_" / "~"** | furl/furl.py | 898 |
| **#   sub-delims  = "!" / "$" / "&" / "'" / "(" / ")"** | furl/furl.py | 899 |
| **#                     / "*" / "+" / "," / ";" / "="** | furl/furl.py | 900 |
| **# Single key to remove.** | furl/furl.py | 945 |
| **# Dictionary or multivalue dictionary of items to remove.** | furl/furl.py | 947 |
| **# List of keys or items to remove.** | furl/furl.py | 950 |
| **# Multivalue Dictionary-like interface. e.g. {'a':1, 'a':2,** | furl/furl.py | 1084 |
| **# 'b':2}** | furl/furl.py | 1085 |
| **# Dictionary-like interface. e.g. {'a':1, 'b':2, 'c':3}** | furl/furl.py | 1090 |
| **# Encoded query string. e.g. 'a=1&b=2&c=3'** | furl/furl.py | 1095 |
| **# Default to list of key:value items interface. e.g. [('a','1'),** | furl/furl.py | 1098 |
| **# ('b','2')]** | furl/furl.py | 1099 |
| **# Empty value without a '=', e.g. '?sup'.** | furl/furl.py | 1123 |
| **# Does this fragment look like a path or a query? Default to** | furl/furl.py | 1214 |
| **# path.** | furl/furl.py | 1215 |
| **# Does toks[1] actually look like a query? Like 'a=a' or** | furl/furl.py | 1221 |
| **# 'a=' or '=a'?** | furl/furl.py | 1222 |
| **# If toks[1] doesn't look like a query, the user probably** | furl/furl.py | 1226 |
| **# provided a fragment string like 'a?b?' that was intended** | furl/furl.py | 1227 |
| **# to be adopted as-is, not a two part fragment with path 'a'** | furl/furl.py | 1228 |
| **# and query 'b?'.** | furl/furl.py | 1229 |
| **# If there is no query or self.separator is False, decode all** | furl/furl.py | 1287 |
| **# '?' characters in the path from their percent encoded form** | furl/furl.py | 1288 |
| **# '%3F' to '?'. This allows for fragment strings containg '?'s,** | furl/furl.py | 1289 |
| **# like '#dog?machine?yes'.** | furl/furl.py | 1290 |
| **# urlsplit() raises a ValueError on malformed IPv6 addresses in** | furl/furl.py | 1404 |
| **# Python 2.7+.** | furl/furl.py | 1405 |
| **# Invalid IPv6 literal.** | furl/furl.py | 1437 |
| **# Invalid host string.** | furl/furl.py | 1440 |
| **# Raises ValueError on malformed IPv6 addresses.** | furl/furl.py | 1503 |
| **# IPv6 address literal.** | furl/furl.py | 1516 |
| **# Avoid side effects by assigning self.port before self.host so** | furl/furl.py | 1531 |
| **# that if an exception is raised when assigning self.port,** | furl/furl.py | 1532 |
| **# self.host isn't updated.** | furl/furl.py | 1533 |
| **# Guard against side effects on exception.** | furl/furl.py | 1712 |
| **# Raises ValueError on invalid port or malformed IP.** | furl/furl.py | 1720 |
| **# Raises ValueError on invalid port or malformed IP.** | furl/furl.py | 1723 |
| **# Raises ValueError on invalid host or malformed IP.** | furl/furl.py | 1728 |
| **# Differentiate between '' and None values for scheme and netloc.** | furl/furl.py | 1834 |

## Function Names and Associated Docstring
```python
def lget(lst, index, default):
"""

"""
```
```python
def attemptstr(o):
"""

"""
```
```python
def utf8(o, default):
"""

"""
```
```python
def non_string_iterable(o):
"""

"""
```
```python
def idna_encode(o):
"""

"""
```
```python
def idna_decode(o):
"""

"""
```
```python
def is_valid_port(port):
"""

"""
```
```python
def static_vars():
"""

"""
```
```python
def create_quote_fn(safe_charset, quote_plus):
"""

"""
```
```python
def is_valid_encoded_path_segment(segment):
"""

"""
```
```python
def is_valid_encoded_query_key(key):
"""

"""
```
```python
def is_valid_encoded_query_value(value):
"""

"""
```
```python
def is_valid_scheme(scheme):
"""

"""
```
```python
def is_valid_host(hostname):
"""

"""
```
```python
def get_scheme(url):
"""

"""
```
```python
def strip_scheme(url):
"""

"""
```
```python
def set_scheme(url, scheme):
"""

"""
```
```python
def has_netloc(url):
"""

"""
```
```python
def urlsplit(url):
"""
Parameters:
  url: URL string to split.
Returns: urlparse.SplitResult tuple subclass, just like
  urlparse.urlsplit() returns, with fields (scheme, netloc, path,
  query, fragment, username, password, hostname, port). See
    http://docs.python.org/library/urlparse.html#urlparse.urlsplit
  for more details on urlsplit().
"""
```
```python
def urljoin(base, url):
"""
Parameters:
  base: Base URL to join with <url>.
  url: Relative or absolute URL to join with <base>.

Returns: The resultant URL from joining <base> and <url>.
"""
```
```python
def join_path_segments():
"""
Join multiple lists of path segments together, intelligently
handling path segments borders to preserve intended slashes of the
final constructed path.

This function is not encoding aware. It doesn't test for, or change,
the encoding of path segments it is passed.

Examples:
  join_path_segments(['a'], ['b']) == ['a','b']
  join_path_segments(['a',''], ['b']) == ['a','b']
  join_path_segments(['a'], ['','b']) == ['a','b']
  join_path_segments(['a',''], ['','b']) == ['a','','b']
  join_path_segments(['a','b'], ['c','d']) == ['a','b','c','d']

Returns: A list containing the joined path segments.
"""
```
```python
def remove_path_segments(segments, remove):
"""
Removes the path segments of <remove> from the end of the path
segments <segments>.

Examples:
  # ('/a/b/c', 'b/c') -> '/a/'
  remove_path_segments(['','a','b','c'], ['b','c']) == ['','a','']
  # ('/a/b/c', '/b/c') -> '/a'
  remove_path_segments(['','a','b','c'], ['','b','c']) == ['','a']

Returns: The list of all remaining path segments after the segments
in <remove> have been removed from the end of <segments>. If no
segments from <remove> were removed from <segments>, <segments> is
returned unmodified.
"""
```
```python
def quacks_like_a_path_with_segments(obj):
"""

"""
```
```python
def decorator(func):
"""

"""
```
```python
def quote_fn(s, dont_quote):
"""

"""
```
```python
def __init__(self, url, args, path, fragment, scheme, netloc, origin, fragment_path, fragment_args, fragment_separator, host, port, query, query_params, username, password, strict):
"""
Raises: ValueError on invalid URL or invalid URL component(s) provided.
"""
```
```python
def load(self, url):
"""
Parse and load a URL.

Raises: ValueError on invalid URL, like a malformed IPv6 address
or invalid port.
"""
```
```python
def add(self, args, path, fragment_path, fragment_args, query_params):
"""
Add components to a URL and return this furl instance, <self>.

If both <args> and <query_params> are provided, a UserWarning is
raised because <args> is provided as a shortcut for
<query_params>, not to be used simultaneously with
<query_params>. Nonetheless, providing both <args> and
<query_params> behaves as expected, with query keys and values
from both <args> and <query_params> added to the query - <args>
first, then <query_params>.

Parameters:
  args: Shortcut for <query_params>.
  path: A list of path segments to add to the existing path
    segments, or a path string to join with the existing path
    string.
  query_params: A dictionary of query keys and values or list of
    key:value items to add to the query.
  fragment_path: A list of path segments to add to the existing
    fragment path segments, or a path string to join with the
    existing fragment path string.
  fragment_args: A dictionary of query keys and values or list
    of key:value items to add to the fragment's query.

Returns: <self>.

Raises: UserWarning if redundant and possibly conflicting <args> and
<query_params> were provided.
"""
```
```python
def set(self, args, path, fragment, query, scheme, username, password, host, port, netloc, origin, query_params, fragment_path, fragment_args, fragment_separator):
"""
Set components of a url and return this furl instance, <self>.

If any overlapping, and hence possibly conflicting, parameters
are provided, appropriate UserWarning's will be raised. The
groups of parameters that could potentially overlap are

  <scheme> and <origin>
  <origin>, <netloc>, and/or (<host> or <port>)
  <fragment> and (<fragment_path> and/or <fragment_args>)
  any two or all of <query>, <args>, and/or <query_params>

In all of the above groups, the latter parameter(s) take
precedence over the earlier parameter(s). So, for example

  furl('http://google.com/').set(
    netloc='yahoo.com:99', host='bing.com', port=40)

will result in a UserWarning being raised and the url becoming

  'http://bing.com:40/'

not

  'http://yahoo.com:99/

Parameters:
  args: Shortcut for <query_params>.
  path: A list of path segments or a path string to adopt.
  fragment: Fragment string to adopt.
  scheme: Scheme string to adopt.
  netloc: Network location string to adopt.
  origin: Scheme and netloc.
  query: Query string to adopt.
  query_params: A dictionary of query keys and values or list of
    key:value items to adopt.
  fragment_path: A list of path segments to adopt for the
    fragment's path or a path string to adopt as the fragment's
    path.
  fragment_args: A dictionary of query keys and values or list
    of key:value items for the fragment's query to adopt.
  fragment_separator: Boolean whether or not there should be a
    '?' separator between the fragment path and fragment query.
  host: Host string to adopt.
  port: Port number to adopt.
  username: Username string to adopt.
  password: Password string to adopt.
Raises:
  ValueError on invalid port.
  UserWarning if <scheme> and <origin> are provided.
  UserWarning if <origin>, <netloc> and/or (<host> and/or <port>) are
    provided.
  UserWarning if <query>, <args>, and/or <query_params> are provided.
  UserWarning if <fragment> and (<fragment_path>,
    <fragment_args>, and/or <fragment_separator>) are provided.
Returns: <self>.
"""
```
```python
def remove(self, args, path, fragment, query, scheme, username, password, host, port, netloc, origin, query_params, fragment_path, fragment_args):
"""
Remove components of this furl's URL and return this furl
instance, <self>.

Parameters:
  args: Shortcut for query_params.
  path: A list of path segments to remove from the end of the
    existing path segments list, or a path string to remove from
    the end of the existing path string, or True to remove the
    path portion of the URL entirely.
  query: A list of query keys to remove from the query, if they
    exist, or True to remove the query portion of the URL
    entirely.
  query_params: A list of query keys to remove from the query,
    if they exist.
  port: If True, remove the port from the network location
    string, if it exists.
  fragment: If True, remove the fragment portion of the URL
    entirely.
  fragment_path: A list of path segments to remove from the end
    of the fragment's path segments or a path string to remove
    from the end of the fragment's path string.
  fragment_args: A list of query keys to remove from the
    fragment's query, if they exist.
  username: If True, remove the username, if it exists.
  password: If True, remove the password, if it exists.
Returns: <self>.
"""
```
```python
def normalize(self):
"""
Normalize the path. Turn '//a/./b/../c//' into '/a/c/'.

Returns: <self>.
"""
```
```python
def asdict(self):
"""

"""
```
```python
def isabsolute(self, isabsolute):
"""
Raises: AttributeError if _force_absolute(self) returns True.
"""
```
```python
def isdir(self):
"""
Returns: True if the path ends on a directory, False
otherwise. If True, the last segment is '', representing the
trailing '/' of the path.
"""
```
```python
def isfile(self):
"""
Returns: True if the path ends on a file, False otherwise. If
True, the last segment is not '', representing some file as the
last segment of the path.
"""
```
```python
def __truediv__(self, path):
"""

"""
```
```python
def __eq__(self, other):
"""

"""
```
```python
def __ne__(self, other):
"""

"""
```
```python
def __bool__(self):
"""

"""
```
```python
def __str__(self):
"""

"""
```
```python
def __repr__(self):
"""

"""
```
```python
def _segments_from_path(self, path):
"""
Returns: The list of path segments from the path string <path>.

Raises: UserWarning if <path> is an improperly encoded path
string and self.strict is True.

TODO(grun): Accept both list values and string values and
refactor the list vs string interface testing to this common
method.
"""
```
```python
def _path_from_segments(self, segments):
"""
Combine the provided path segments <segments> into a path string. Path
segments in <segments> will be quoted.

Returns: A path string with quoted path segments.
"""
```
```python
def path(self):
"""

"""
```
```python
def pathstr(self):
"""
This method is deprecated. Use str(furl.path) instead.
"""
```
```python
def _force_absolute(self, path):
"""

"""
```
```python
def __setattr__(self, attr, value):
"""

"""
```
```python
def params(self, params):
"""

"""
```
```python
def encode(self, delimiter, quote_plus, dont_quote, delimeter):
"""
Examples:

  Query('a=a&b=#').encode() == 'a=a&b=%23'
  Query('a=a&b=#').encode(';') == 'a=a;b=%23'
  Query('a+b=c@d').encode(dont_quote='@') == 'a+b=c@d'
  Query('a+b=c@d').encode(quote_plus=False) == 'a%20b=c%40d'

Until furl v0.4.6, the 'delimiter' argument was incorrectly
spelled 'delimeter'. For backwards compatibility, accept both
the correct 'delimiter' and the old, misspelled 'delimeter'.

Keys and values are encoded application/x-www-form-urlencoded if
<quote_plus> is True, percent-encoded otherwise.

<dont_quote> exempts valid query characters from being
percent-encoded, either in their entirety with dont_quote=True,
or selectively with dont_quote=<string>, like
dont_quote='/?@_'. Invalid query characters -- those not in
self.SAFE_KEY_CHARS, like '#' and '^' -- are always encoded,
even if included in <dont_quote>. For example:

  Query('#=^').encode(dont_quote='#^') == '%23=%5E'.

Returns: A URL encoded query string using <delimiter> as the
delimiter separating key:value pairs. The most common and
default delimiter is '&', but ';' can also be specified. ';' is
W3C recommended.
"""
```
```python
def _items(self, items):
"""
Extract and return the key:value items from various
containers. Some containers that could hold key:value items are

  - List of (key,value) tuples.
  - Dictionaries of key:value items.
  - Multivalue dictionary of key:value items, with potentially
    repeated keys.
  - Query string with encoded params and values.

Keys and values are passed through unmodified unless they were
passed in within an encoded query string, like
'a=a%20a&b=b'. Keys and values passed in within an encoded query
string are unquoted by urlparse.parse_qsl(), which uses
urllib.unquote_plus() internally.

Returns: List of items as (key, value) tuples. Keys and values
are passed through unmodified unless they were passed in as part
of an encoded query string, in which case the final keys and
values that are returned will be unquoted.

Raises: UserWarning if <path> is an improperly encoded path
string and self.strict is True.
"""
```
```python
def _extract_items_from_querystr(self, querystr):
"""

"""
```
```python
def query(self):
"""

"""
```
```python
def querystr(self):
"""
This method is deprecated. Use str(furl.query) instead.
"""
```
```python
def args(self):
"""
Shortcut method to access the query parameters, self._query.params.
"""
```
```python
def fragment(self):
"""

"""
```
```python
def fragmentstr(self):
"""
This method is deprecated. Use str(furl.fragment) instead.
"""
```
```python
def scheme(self, scheme):
"""

"""
```
```python
def host(self, host):
"""
Raises: ValueError on invalid host or malformed IPv6 address.
"""
```
```python
def port(self, port):
"""
The port value can be 1-65535 or None, meaning no port specified. If
<port> is None and self.scheme is a known scheme in DEFAULT_PORTS,
the default port value from DEFAULT_PORTS will be used.

Raises: ValueError on invalid port.
"""
```
```python
def netloc(self, netloc):
"""
Params:
  netloc: Network location string, like 'google.com' or
    'user:pass@google.com:99'.
Raises: ValueError on invalid port or malformed IPv6 address.
"""
```
```python
def origin(self, origin):
"""

"""
```
```python
def url(self, url):
"""

"""
```
```python
def tostr(self, query_delimiter, query_quote_plus, query_dont_quote):
"""

"""
```
```python
def join(self):
"""

"""
```
```python
def copy(self):
"""

"""
```
```python
def __unicode__(self):
"""

"""
```
```python
def present(v):
"""

"""
```
# furl/omdict1D.py


# Comments
| Comment | File | Line |
|---------|------|------|
| **# -*- coding: utf-8 -*-** | furl/omdict1D.py | 1 |
| **#** | furl/omdict1D.py | 3 |
| **# furl - URL manipulation made simple.** | furl/omdict1D.py | 4 |
| **#** | furl/omdict1D.py | 5 |
| **# Ansgar Grunseid** | furl/omdict1D.py | 6 |
| **# grunseid.com** | furl/omdict1D.py | 7 |
| **# grunseid@gmail.com** | furl/omdict1D.py | 8 |
| **#** | furl/omdict1D.py | 9 |
| **# License: Build Amazing Things (Unlicense)** | furl/omdict1D.py | 10 |
| **#** | furl/omdict1D.py | 11 |
| **# <values> is not a list or an empty list.** | furl/omdict1D.py | 78 |
| **# If the value is [], remove any existing leftovers with** | furl/omdict1D.py | 84 |
| **# key <key> and set the list of values itself to [],** | furl/omdict1D.py | 85 |
| **# which in turn will later delete <key> when [] is** | furl/omdict1D.py | 86 |
| **# passed to omdict.setlist() in** | furl/omdict1D.py | 87 |
| **# omdict._update_updateall().** | furl/omdict1D.py | 88 |
| **# If there are existing items with key <key> that have** | furl/omdict1D.py | 92 |
| **# yet to be marked for replacement, mark that item's** | furl/omdict1D.py | 93 |
| **# value to be replaced by <value> by appending it to** | furl/omdict1D.py | 94 |
| **# <replacements>.** | furl/omdict1D.py | 95 |

## Function Names and Associated Docstring
```python
def add(self, key, value):
"""

"""
```
```python
def set(self, key, value):
"""

"""
```
```python
def __setitem__(self, key, value):
"""

"""
```
```python
def _bin_update_items(self, items, replace_at_most_one, replacements, leftovers):
"""
Subclassed from omdict._bin_update_items() to make update() and
updateall() process lists of values as multiple values.

<replacements> and <leftovers> are modified directly, ala pass by
reference.
"""
```
```python
def _set(self, key, value):
"""

"""
```
# setup.py



# Comments
| Comment | File | Line |
|---------|------|------|
| **#!/usr/bin/env python** | setup.py | 1 |
| **# -*- coding: utf-8 -*-** | setup.py | 2 |
| **#** | setup.py | 4 |
| **# furl - URL manipulation made simple.** | setup.py | 5 |
| **#** | setup.py | 6 |
| **# Ansgar Grunseid** | setup.py | 7 |
| **# grunseid.com** | setup.py | 8 |
| **# grunseid@gmail.com** | setup.py | 9 |
| **#** | setup.py | 10 |
| **# License: Build Amazing Things (Unlicense)** | setup.py | 11 |
| **#** | setup.py | 12 |

## Function Names and Associated Docstring
```python
def initialize_options(self):
"""

"""
```
```python
def finalize_options(self):
"""

"""
```
```python
def run(self):
"""

"""
```
```python
def run_tests(self):
"""

"""
```
# tests/test_furl.py



# Comments
| Comment | File | Line |
|---------|------|------|
| **# -*- coding: utf-8 -*-** | tests/test_furl.py | 1 |
| **#** | tests/test_furl.py | 3 |
| **# furl - URL manipulation made simple.** | tests/test_furl.py | 4 |
| **#** | tests/test_furl.py | 5 |
| **# Ansgar Grunseid** | tests/test_furl.py | 6 |
| **# grunseid.com** | tests/test_furl.py | 7 |
| **# grunseid@gmail.com** | tests/test_furl.py | 8 |
| **#** | tests/test_furl.py | 9 |
| **# License: Build Amazing Things (Unlicense)** | tests/test_furl.py | 10 |
| **#** | tests/test_furl.py | 11 |
| **#** | tests/test_furl.py | 31 |
| **# TODO(grun): Add tests for furl objects with strict=True. Make sure** | tests/test_furl.py | 32 |
| **# UserWarnings are raised when improperly encoded path, query, and** | tests/test_furl.py | 33 |
| **# fragment strings are provided.** | tests/test_furl.py | 34 |
| **#** | tests/test_furl.py | 35 |
| **# Keys and values get unquoted. i.e. 'a=a%20a' -> ['a', 'a a']. Empty** | tests/test_furl.py | 100 |
| **# values without '=' have value None.** | tests/test_furl.py | 101 |
| **# Valid path segment characters should not be encoded.** | tests/test_furl.py | 205 |
| **# Invalid path segment characters should be encoded.** | tests/test_furl.py | 211 |
| **# Encode '/' within a path segment.** | tests/test_furl.py | 217 |
| **# Encode percent signs in path segment stings.** | tests/test_furl.py | 224 |
| **# Percent-encodings should be capitalized, as per RFC 3986.** | tests/test_furl.py | 228 |
| **# URL paths.** | tests/test_furl.py | 252 |
| **# Fragment paths.** | tests/test_furl.py | 313 |
| **# Remove lists of path segments.** | tests/test_furl.py | 327 |
| **# Remove a path string.** | tests/test_furl.py | 358 |
| **# Remove True.** | tests/test_furl.py | 397 |
| **# A URL path's isabsolute attribute is mutable if there's no** | tests/test_furl.py | 405 |
| **# netloc.** | tests/test_furl.py | 406 |
| **# A URL path's isabsolute attribute is read-only if there's** | tests/test_furl.py | 422 |
| **# a netloc.** | tests/test_furl.py | 423 |
| **# Netloc, no scheme -> isabsolute is read-only if path** | tests/test_furl.py | 425 |
| **# is non-empty.** | tests/test_furl.py | 426 |
| **# Netloc and scheme -> isabsolute is read-only if path** | tests/test_furl.py | 428 |
| **# is non-empty.** | tests/test_furl.py | 429 |
| **# A Fragment path's isabsolute attribute is never read-only.** | tests/test_furl.py | 445 |
| **# Sanity checks.** | tests/test_furl.py | 458 |
| **# Path not modified.** | tests/test_furl.py | 472 |
| **# Path modified.** | tests/test_furl.py | 477 |
| **# Path objects should be joinable with other Path objects.** | tests/test_furl.py | 547 |
| **# Joining paths with __truediv__ should not modify the original, even** | tests/test_furl.py | 552 |
| **# if <isabsolute> is True.** | tests/test_furl.py | 553 |
| **# All interaction with parameters is unquoted unless that** | tests/test_furl.py | 576 |
| **# interaction is through an already encoded query string. In the** | tests/test_furl.py | 577 |
| **# case of an already encoded query string, like 'a=a%20a&b=b',** | tests/test_furl.py | 578 |
| **# its keys and values will be unquoted.** | tests/test_furl.py | 579 |
| **# Basics.** | tests/test_furl.py | 605 |
| **# Various quoted and unquoted parameters and values that** | tests/test_furl.py | 608 |
| **# will be unquoted.** | tests/test_furl.py | 609 |
| **# Only keys, no values.** | tests/test_furl.py | 615 |
| **# Repeated parameters.** | tests/test_furl.py | 618 |
| **# Empty keys and/or values.** | tests/test_furl.py | 620 |
| **# Semicolon delimiter is not allowed per default after bpo#42967** | tests/test_furl.py | 622 |
| **# encode() accepts both 'delimiter' and 'delimeter'. The** | tests/test_furl.py | 642 |
| **# latter was incorrectly used until furl v0.4.6.** | tests/test_furl.py | 643 |
| **# __nonzero__().** | tests/test_furl.py | 647 |
| **# The examples.** | tests/test_furl.py | 679 |
| **# Further manual tests.** | tests/test_furl.py | 689 |
| **# Remove one key at a time.** | tests/test_furl.py | 697 |
| **# Remove multiple keys at a time (in this case all of them).** | tests/test_furl.py | 704 |
| **# Remove the whole query string with True.** | tests/test_furl.py | 712 |
| **# List of keys to remove.** | tests/test_furl.py | 719 |
| **# List of items to remove.** | tests/test_furl.py | 724 |
| **# Dictionary of items to remove.** | tests/test_furl.py | 729 |
| **# Multivalue dictionary of items to remove.** | tests/test_furl.py | 734 |
| **# Basics.** | tests/test_furl.py | 741 |
| **# Blanks keys and values are kept.** | tests/test_furl.py | 751 |
| **# ';' is no longer a valid query delimiter, though it was prior to furl** | tests/test_furl.py | 759 |
| **# v2.1.3. See https://bugs.python.org/issue42967.** | tests/test_furl.py | 760 |
| **# Non-string parameters are coerced to strings in the final** | tests/test_furl.py | 764 |
| **# query string.** | tests/test_furl.py | 765 |
| **# Spaces are encoded as '+'s. '+'s are encoded as '%2B'.** | tests/test_furl.py | 773 |
| **# Params is an omdict (ordered multivalue dictionary).** | tests/test_furl.py | 779 |
| **# Assign various things to Query.params and make sure** | tests/test_furl.py | 786 |
| **# Query.params is reinitialized, not replaced.** | tests/test_furl.py | 787 |
| **# Value of '' -> '?param='. Value of None -> '?param'.** | tests/test_furl.py | 796 |
| **# encode() and __str__().** | tests/test_furl.py | 834 |
| **# Accept both percent-encoded ('a=b%20c') and** | tests/test_furl.py | 837 |
| **# application/x-www-form-urlencoded ('a=b+c') pairs as input.** | tests/test_furl.py | 838 |
| **# Encode '/' consistently across quote_plus=True and quote_plus=False.** | tests/test_furl.py | 843 |
| **# dont_quote= accepts both True and a string of safe characters not to** | tests/test_furl.py | 848 |
| **# percent-encode. Unsafe query characters, like '^' and '#', are always** | tests/test_furl.py | 849 |
| **# percent-encoded.** | tests/test_furl.py | 850 |
| **# Calculate the expected querystring with proper query encoding.** | tests/test_furl.py | 899 |
| **#   Valid query key characters: "/?:@-._~!$'()*,;"** | tests/test_furl.py | 900 |
| **#   Valid query value characters: "/?:@-._~!$'()*,;="** | tests/test_furl.py | 901 |
| **# Don't hide duplicate Warnings. Test for all of them.** | tests/test_furl.py | 1158 |
| **# urlsplit() only parses the query for schemes in urlparse.uses_query,** | tests/test_furl.py | 1162 |
| **# so switch to 'http' (a scheme in urlparse.uses_query) for** | tests/test_furl.py | 1163 |
| **# urlparse.urlsplit().** | tests/test_furl.py | 1164 |
| **# Note: urlparse.urlsplit() doesn't separate the query from the path** | tests/test_furl.py | 1168 |
| **# for all schemes, only those schemes in the list urlparse.uses_query.** | tests/test_furl.py | 1169 |
| **# So, as a result of using urlparse.urlsplit(), this little helper** | tests/test_furl.py | 1170 |
| **# function only works when provided URLs whos schemes are also in** | tests/test_furl.py | 1171 |
| **# urlparse.uses_query.** | tests/test_furl.py | 1172 |
| **# Accept unicode without raising an exception.** | tests/test_furl.py | 1226 |
| **# Accept unicode paths.** | tests/test_furl.py | 1230 |
| **# Accept unicode queries.** | tests/test_furl.py | 1236 |
| **# Lowercase.** | tests/test_furl.py | 1253 |
| **# No scheme.** | tests/test_furl.py | 1256 |
| **# Protocol relative URLs.** | tests/test_furl.py | 1261 |
| **# Schemes without slashes, like 'mailto:'.** | tests/test_furl.py | 1271 |
| **# Ignore invalid schemes.** | tests/test_furl.py | 1289 |
| **# Empty scheme.** | tests/test_furl.py | 1293 |
| **# Empty usernames and passwords.** | tests/test_furl.py | 1298 |
| **# Username only.** | tests/test_furl.py | 1307 |
| **# Password only.** | tests/test_furl.py | 1328 |
| **# Username and password.** | tests/test_furl.py | 1349 |
| **# Username and password in the network location string.** | tests/test_furl.py | 1375 |
| **# Unicode.** | tests/test_furl.py | 1408 |
| **# URL paths are optionally absolute if scheme and netloc are** | tests/test_furl.py | 1459 |
| **# empty.** | tests/test_furl.py | 1460 |
| **# Fragment paths are optionally absolute, and not absolute by** | tests/test_furl.py | 1467 |
| **# default.** | tests/test_furl.py | 1468 |
| **# URLs comprised of a netloc string only should not be prefixed** | tests/test_furl.py | 1475 |
| **# with '//', as-is the default behavior of** | tests/test_furl.py | 1476 |
| **# urlparse.urlunsplit().** | tests/test_furl.py | 1477 |
| **# furl('...') and furl.url = '...' are functionally identical.** | tests/test_furl.py | 1484 |
| **# Empty scheme and netloc.** | tests/test_furl.py | 1491 |
| **# Empty.** | tests/test_furl.py | 1561 |
| **# Scheme only.** | tests/test_furl.py | 1588 |
| **# Host only.** | tests/test_furl.py | 1612 |
| **# Port only.** | tests/test_furl.py | 1620 |
| **# urlparse.urlsplit() treats the first two '//' as the beginning** | tests/test_furl.py | 1627 |
| **# of a netloc, even if the netloc is empty.** | tests/test_furl.py | 1628 |
| **# TODO(grun): Test more odd URLs.** | tests/test_furl.py | 1633 |
| **# No host.** | tests/test_furl.py | 1636 |
| **# Valid IPv4 and IPv6 addresses.** | tests/test_furl.py | 1641 |
| **# Host strings are always lowercase.** | tests/test_furl.py | 1645 |
| **# Invalid IPv4 addresses shouldn't raise an exception because** | tests/test_furl.py | 1653 |
| **# urlparse.urlsplit() doesn't raise an exception on invalid IPv4** | tests/test_furl.py | 1654 |
| **# addresses.** | tests/test_furl.py | 1655 |
| **# Invalid, but well-formed, IPv6 addresses shouldn't raise an** | tests/test_furl.py | 1658 |
| **# exception because urlparse.urlsplit() doesn't raise an** | tests/test_furl.py | 1659 |
| **# exception on invalid IPv6 addresses.** | tests/test_furl.py | 1660 |
| **# Malformed IPv6 should raise an exception because urlparse.urlsplit()** | tests/test_furl.py | 1663 |
| **# raises an exception on malformed IPv6 addresses.** | tests/test_furl.py | 1664 |
| **# Invalid host strings should raise ValueError.** | tests/test_furl.py | 1670 |
| **# Malformed IPv6 should raise an exception because** | tests/test_furl.py | 1693 |
| **# urlparse.urlsplit() raises an exception** | tests/test_furl.py | 1694 |
| **# Invalid ports should raise an exception.** | tests/test_furl.py | 1700 |
| **# No side effects.** | tests/test_furl.py | 1706 |
| **# Empty netloc.** | tests/test_furl.py | 1710 |
| **# Username and password are unaffected.** | tests/test_furl.py | 1725 |
| **# Malformed IPv6 should raise an exception because urlparse.urlsplit()** | tests/test_furl.py | 1730 |
| **# raises an exception.** | tests/test_furl.py | 1731 |
| **# Invalid ports should raise an exception.** | tests/test_furl.py | 1737 |
| **# Default port values.** | tests/test_furl.py | 1744 |
| **# Override default port values.** | tests/test_furl.py | 1749 |
| **# Reset the port.** | tests/test_furl.py | 1754 |
| **# Invalid port raises ValueError with no side effects.** | tests/test_furl.py | 1765 |
| **# The port is inferred from scheme changes, if possible, but** | tests/test_furl.py | 1785 |
| **# only if the port is otherwise unset (self.port is None).** | tests/test_furl.py | 1786 |
| **# Hostnames are always lowercase.** | tests/test_furl.py | 1791 |
| **# Supplying both <args> and <query_params> should raise a** | tests/test_furl.py | 1817 |
| **# warning.** | tests/test_furl.py | 1818 |
| **# No conflict warnings between <host>/<port> and <netloc>, or** | tests/test_furl.py | 1834 |
| **# <query> and <params>.** | tests/test_furl.py | 1835 |
| **# Path as a list of path segments to join.** | tests/test_furl.py | 1841 |
| **# Set a lot of stuff (but avoid conflicts, which are tested** | tests/test_furl.py | 1847 |
| **# below).** | tests/test_furl.py | 1848 |
| **# No side effects.** | tests/test_furl.py | 1854 |
| **# Separator isn't reset with set().** | tests/test_furl.py | 1866 |
| **# Test warnings for potentially overlapping parameters.** | tests/test_furl.py | 1872 |
| **# Scheme, origin overlap. Scheme takes precedence.** | tests/test_furl.py | 1876 |
| **# Netloc, origin, host and/or port. Host and port take precedence.** | tests/test_furl.py | 1882 |
| **# Query, args, and query_params overlap - args and query_params** | tests/test_furl.py | 1903 |
| **# take precedence.** | tests/test_furl.py | 1904 |
| **# Fragment, fragment_path, fragment_args, and fragment_separator** | tests/test_furl.py | 1921 |
| **# overlap - fragment_separator, fragment_path, and fragment_args** | tests/test_furl.py | 1922 |
| **# take precedence.** | tests/test_furl.py | 1923 |
| **# Remove without parameters removes nothing.** | tests/test_furl.py | 1947 |
| **# username, password, and port must be True.** | tests/test_furl.py | 1950 |
| **# Basics.** | tests/test_furl.py | 1954 |
| **# scheme, host, port, netloc, origin.** | tests/test_furl.py | 1959 |
| **# No errors are thrown when removing URL components that don't exist.** | tests/test_furl.py | 1967 |
| **# Path as a list of paths to join before removing.** | tests/test_furl.py | 1978 |
| **# Join full URLs.** | tests/test_furl.py | 1993 |
| **# Absolute paths ('/foo').** | tests/test_furl.py | 2000 |
| **# Relative paths ('../foo').** | tests/test_furl.py | 2005 |
| **# Query included.** | tests/test_furl.py | 2010 |
| **# Fragment included.** | tests/test_furl.py | 2016 |
| **# Unicode.** | tests/test_furl.py | 2022 |
| **# Join other furl object, which serialize to strings with str().** | tests/test_furl.py | 2035 |
| **# Join multiple URLs.** | tests/test_furl.py | 2041 |
| **# In edge cases (e.g. URLs without an authority/netloc), behave** | tests/test_furl.py | 2047 |
| **# identically to urllib.parse.urljoin(), which changed behavior in** | tests/test_furl.py | 2048 |
| **# Python 3.9.** | tests/test_furl.py | 2049 |
| **# query_dont_quote ignores invalid query characters, like '$'.** | tests/test_furl.py | 2071 |
| **# Without any delimiters like '://' or '/', the input should be** | tests/test_furl.py | 2094 |
| **# treated as a path.** | tests/test_furl.py | 2095 |
| **# No changes to existing urlsplit() behavior for known schemes.** | tests/test_furl.py | 2101 |
| **# Properly split the query from the path for unknown schemes.** | tests/test_furl.py | 2110 |
| **# Empty.** | tests/test_furl.py | 2131 |
| **# Null strings.** | tests/test_furl.py | 2136 |
| **#   [''] means nothing, or an empty string, in the final path** | tests/test_furl.py | 2137 |
| **#     segments.** | tests/test_furl.py | 2138 |
| **#   ['', ''] is preserved as a slash in the final path segments.** | tests/test_furl.py | 2139 |
| **# Basics.** | tests/test_furl.py | 2152 |
| **# A trailing slash is preserved if no new slash is being added.** | tests/test_furl.py | 2158 |
| **#   ex: ['a', ''] + ['b'] == ['a', 'b'], or 'a/' + 'b' == 'a/b'** | tests/test_furl.py | 2159 |
| **# A new slash is preserved if no trailing slash exists.** | tests/test_furl.py | 2165 |
| **#   ex: ['a'] + ['', 'b'] == ['a', 'b'], or 'a' + '/b' == 'a/b'** | tests/test_furl.py | 2166 |
| **# A trailing slash and a new slash means that an extra slash** | tests/test_furl.py | 2174 |
| **# will exist afterwords.** | tests/test_furl.py | 2175 |
| **# ex: ['a', ''] + ['', 'b'] == ['a', '', 'b'], or 'a/' + '/b'** | tests/test_furl.py | 2176 |
| **#   == 'a//b'** | tests/test_furl.py | 2177 |
| **# Path segments blocks without slashes, are combined as** | tests/test_furl.py | 2192 |
| **# expected.** | tests/test_furl.py | 2193 |
| **# Putting it all together.** | tests/test_furl.py | 2200 |
| **# [''] represents a slash, equivalent to ['',''].** | tests/test_furl.py | 2213 |
| **# Basics.** | tests/test_furl.py | 2215 |
| **# Slash manipulation.** | tests/test_furl.py | 2223 |
| **# Remove a portion of the path from the tail of the original** | tests/test_furl.py | 2233 |
| **# path.** | tests/test_furl.py | 2234 |
| **# Attempt to remove valid subsections, but subsections not from** | tests/test_furl.py | 2252 |
| **# the end of the original path.** | tests/test_furl.py | 2253 |
| **# Attempt to remove segments longer than the original.** | tests/test_furl.py | 2276 |

## Function Names and Associated Docstring
```python
def allitems(self):
"""

"""
```
```python
def iterallitems(self):
"""

"""
```
```python
def original(self):
"""

"""
```
```python
def test_none(self):
"""

"""
```
```python
def test_isdir_isfile(self):
"""

"""
```
```python
def test_leading_slash(self):
"""

"""
```
```python
def test_encoding(self):
"""

"""
```
```python
def test_load(self):
"""

"""
```
```python
def test_set(self):
"""

"""
```
```python
def _test_set_load(self, path_set_or_load):
"""

"""
```
```python
def test_add(self):
"""

"""
```
```python
def test_remove(self):
"""

"""
```
```python
def test_isabsolute(self):
"""

"""
```
```python
def test_normalize(self):
"""

"""
```
```python
def test_equality(self):
"""

"""
```
```python
def test_nonzero(self):
"""

"""
```
```python
def test_unicode(self):
"""

"""
```
```python
def test_itruediv(self):
"""

"""
```
```python
def test_truediv(self):
"""

"""
```
```python
def test_asdict(self):
"""

"""
```
```python
def setUp(self):
"""

"""
```
```python
def test_various(self):
"""

"""
```
```python
def test_params(self):
"""

"""
```
```python
def test_encode(self):
"""

"""
```
```python
def test_value_encoding_empty_vs_nonempty_key(self):
"""

"""
```
```python
def test_special_characters(self):
"""

"""
```
```python
def _quote_items(self, items):
"""

"""
```
```python
def test_interface(self):
"""

"""
```
```python
def test_basics(self):
"""

"""
```
```python
def _param(self, url, key, val):
"""

"""
```
```python
def test_constructor_and_set(self):
"""

"""
```
```python
def test_idna(self):
"""

"""
```
```python
def test_scheme(self):
"""

"""
```
```python
def test_username_and_password(self):
"""

"""
```
```python
def test_basic_manipulation(self):
"""

"""
```
```python
def test_path_itruediv(self):
"""

"""
```
```python
def test_path_truediv(self):
"""

"""
```
```python
def test_odd_urls(self):
"""

"""
```
```python
def test_hosts(self):
"""

"""
```
```python
def test_netloc(self):
"""

"""
```
```python
def test_origin(self):
"""

"""
```
```python
def test_ports(self):
"""

"""
```
```python
def test_join(self):
"""

"""
```
```python
def test_tostr(self):
"""

"""
```
```python
def test_urlsplit(self):
"""

"""
```
```python
def test_join_path_segments(self):
"""

"""
```
```python
def test_remove_path_segments(self):
"""

"""
```
```python
def test_is_valid_port(self):
"""

"""
```
```python
def test_is_valid_scheme(self):
"""

"""
```
```python
def test_is_valid_encoded_path_segment(self):
"""

"""
```
```python
def test_is_valid_encoded_query_key(self):
"""

"""
```
```python
def test_is_valid_encoded_query_value(self):
"""

"""
```
```python
def test_metadata_varibles(self):
"""

"""
```
```python
def is_non_empty_string(s):
"""

"""
```
```python
def __init__(self):
"""

"""
```
```python
def __setattr__(self, attr, value):
"""

"""
```
# tests/test_omdict1D.py



# Comments
| Comment | File | Line |
|---------|------|------|
| **# -*- coding: utf-8 -*-** | tests/test_omdict1D.py | 1 |
| **#** | tests/test_omdict1D.py | 3 |
| **# furl - URL manipulation made simple.** | tests/test_omdict1D.py | 4 |
| **#** | tests/test_omdict1D.py | 5 |
| **# Ansgar Grunseid** | tests/test_omdict1D.py | 6 |
| **# grunseid.com** | tests/test_omdict1D.py | 7 |
| **# grunseid@gmail.com** | tests/test_omdict1D.py | 8 |
| **#** | tests/test_omdict1D.py | 9 |
| **# License: Build Amazing Things (Unlicense)** | tests/test_omdict1D.py | 10 |
| **#** | tests/test_omdict1D.py | 11 |
| **# All permutations of (self.keys, self.values) and (self.keys,** | tests/test_omdict1D.py | 34 |
| **# self.valuelists).** | tests/test_omdict1D.py | 35 |
| **# All updates of length one item, two items, and three items.** | tests/test_omdict1D.py | 39 |
| **# Test different empty list value locations.** | tests/test_omdict1D.py | 66 |
| **# Empty list of values adds nothing.** | tests/test_omdict1D.py | 123 |
| **# Empty list of values deletes that key and all its values,** | tests/test_omdict1D.py | 137 |
| **# equivalent to del omd[somekey].** | tests/test_omdict1D.py | 138 |
| **# Empty list of values deletes that key and all its values,** | tests/test_omdict1D.py | 164 |
| **# equivalent to del omd[somekey].** | tests/test_omdict1D.py | 165 |

## Function Names and Associated Docstring
```python
def setUp(self):
"""

"""
```
```python
def test_update_updateall(self):
"""

"""
```
```python
def test_add(self):
"""

"""
```
```python
def test_set(self):
"""

"""
```
```python
def test_setitem(self):
"""

"""
```
