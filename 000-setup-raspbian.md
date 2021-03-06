# Setting up EOTK on Raspbian

exit 0 # just in case anyone thinks this is a script

# Tor Installation

EOTK requires Tor 0.2.9.9+

# NGINX Installation

EOTK requires recent `nginx` with the following modules/features enabled:

* `headers_more`
* `ngx_http_substitutions_filter_module`
* `http_sub`
* `http_ssl`

# Summary

Unless you are fortunate to have these already installed, there are
two options for you:

- spend hours on your own, messing with `backports` and repos, or:
- run the obviously-named scripts in opt.d to compile from source.

...which will do all the work for you, no options/arguments required,
although the actual compilation may take a long time.  It's your
choice.  If you choose the latter option, do this:

- `./opt.d/build-nginx-on-debian.sh`
- `./opt.d/build-tor-on-debian.sh`

...as appropriate.
