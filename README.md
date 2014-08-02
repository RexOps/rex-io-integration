# Rex.IO integration for Rex

This repository contains the library to integrate Rex with Rex.IO.

## Status

Currently you can store the inventory of a system inside Rex.IO and use it as a persistant cache.

## Installation

You can install Rex.IO integration with the following commands:

```bash
perl Makefile.PL
make
make install
```

## Usage

To use Rex.IO integration within your Rexfile you have to configure it.

```perl
use Rex::RexIO;

set rexio => {
  server   => 'https://your-rexio-server:5000',
  user     => 'the-user',
  password => 'the-password',
};
```

Now you can use with the CLI switch *-c* to activate the cache.
