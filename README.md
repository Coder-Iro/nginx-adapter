Caddy NGINX Config Adapter
==========================

This is a [config adapter](https://github.com/caddyserver/caddy/wiki/v2:-Documentation#config-adapters) for Caddy which converts [NGINX config files](https://www.nginx.com/resources/wiki/start/topics/examples/full/) into Caddy's native format.

**This project is not complete, and we are asking the community to help finish its development.** Due to resource constraints, we are unable to do all the development on our own at this time. However, we hope you will pick it up and collaborate on it together as a community. We'll be happy to coordinate efforts from the community. Start by opening issues and pull requests, then reviewing pull requests and testing changes!

Thank you, and we hope you have fun with it!

## Install

**Note: This module is only compatible with Caddy 2, which is currently in beta.**

First, go get this module:

```
$ go get github.com/caddyserver/nginx-adapter
```

To compile, simply `go build` Caddy 2 with this adapter plugged in. Add this to the list of imports:

```
	_ "github.com/caddyserver/nginx-adapter"
```

Then run:

```
$ go build
```


## Use

Using this config adapter is the same as all the other config adapters.

- [Learn about config adapters in the Caddy docs](https://github.com/caddyserver/caddy/wiki/v2:-Documentation#config-adapters)
- You can adapt your config with the [`adapt` command](https://github.com/caddyserver/caddy/wiki/v2:-Documentation#adapt)

You can also run Caddy directly with an nginx config using [`caddy run|start --config nginx.conf --adapter nginx`](https://github.com/caddyserver/caddy/wiki/v2:-Documentation#run) (however, we do not recommend this until the config adapter is completed).


## Disclaimer

This project is not affiliated with F5 Networks or NGINX, Inc. NGINX is a registered trademark of NGINX, Inc.
