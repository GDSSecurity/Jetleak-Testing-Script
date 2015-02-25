# Jetleak Testing Script

This tool is intended to provide a quick-and-dirty way for organizations to test whether their Jetty web server versions are vulnerable to JetLeak. Currently, this script does not handle sites with invalid SSL certs. This will be fixed in a future iteration.

For additional details on the Jetleak vulnerability refer to our blog post:
ADD URL HERE

Sample Usage: python jetleak_tester.py [url] [port]

Sample Output for a server that is not vulnerable:

```
$ python jetleak_tester.py http://[ENTER HOSTNAME] 80

This version of Jetty is NOT vulnerable to JetLeak.
```

Sample Output for a server that is vulnerable

```
$ python jetleak_tester.py http://[ENTER HOSTNAME] 80

This version of Jetty is VULNERABLE to JetLeak!
```
