# A simple tls <-> unix socket proxy

This will verify all incoping tls connections again the provided
ca, and proxy valid connection onward to the unix socket.

UsagE:
```
Usage of ./tlsproxy:
  -ca string
    	Path to CA to auth clients against (default "ca.pem")
  -cert string
    	Path to cert (default "cert.pem")
  -key string
    	Path to key (default "key.pem")
  -listen string
    	host:port to listen on (default ":6658")
  -no-verify
    	Disable verification, (voids the entire point of this, just for testing)
  -sock string
    	Path to unix socket to proxy to
  -tcp string
    	TCP remote end point to connect to
```
