---
title: Installing Ruby using rvm
---

This topic describes how to install Ruby using rvm.

<p class="note"><strong>Note</strong>: This topic requires that you are starting with a pristine Ubuntu 12.10 installation on a VM or physical machine.</p>

1. Install `curl` using `apt-get`:
  <pre class="terminal">
    $ sudo apt-get install curl
  </pre>

1. Install rvm using `curl`:
  <pre class="terminal">
    $ curl -L https://get.rvm.io | bash -s
  </pre>

1. Restart your shell:
  <pre class="terminal">
    $ source ~/.bash_profile
  </pre>
  <p class="note"><strong>Note</strong>: Follow the steps in <a href="https://rvm.io/integration/gnome-terminal/">Integrating RVM with gnome-terminal</a> to make sure bash runs as a login shell and rvm loads correctly.</p>

1. Check the required dependencies for installing Ruby:
  <pre class="terminal">
    $ rvm requirements
  </pre>

1. Install the required pre-requisites for installing Ruby:
  <pre class="terminal">
    $ sudo /usr/bin/apt-get install build-essential bison openssl libreadline6 libreadline6-dev \
    curl git-core zlib1g zlib1g-dev libssl-dev libyaml-dev libsqlite3-0 libsqlite3-dev \
    sqlite3 libxml2-dev libxslt-dev autoconf libc6-dev ncurses-dev
  </pre>

1. Install Ruby 1.9.3 or Ruby 2.1.2 using `rvm`:
  * For Ruby 1.9.3, run the following command:
  <pre class="terminal">
    $ rvm install 1.9.3
  </pre>
  * For Ruby 2.1.2, run the following command:
  <pre class="terminal">
    $ rvm install 2.1.2
  </pre>

1. Set the Ruby version:
  * For Ruby 1.9.3, run the following command:
  <pre class="terminal">
    $ rvm use 1.9.3
  </pre>
  * For Ruby 2.1.2, run the following command:
  <pre class="terminal">
    $ rvm use 2.1.2
  </pre>

1. Use `ruby -v` to check that the correct version of ruby has been set:
  <pre class="terminal">
    $ ruby -v
  </pre>

1. Install the `bundler` gem:
  <pre class="terminal">
    $ gem install bundler
  </pre>

1. Install the `rake` gem:
<pre class="terminal">
  $ gem install rake
</pre>