# Possible painpoints for FI, or at least things worth noting.

* Requires Ruby 1.9.x and fairly new Rails, but RHEL has Ruby 1.8.x
* Requires a ton of unpackaged RubyGems - for now, I just let it bundle these itself with Bundler.
* Requires a patched gitolite (https://github.com/gitlabhq/gitolite)
* Only provides an init.d file, and I don't know how systemd works.
  * I hacked together two service files based on relevant google searches, but they are probably horrible.
* Runs via a proxied Unicorn - another httpd to maintain. Might be configurable/changeable though.