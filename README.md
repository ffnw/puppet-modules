# puppet-modules
This repository contains a collection of puppet modules for the Freifunk Nordwest network.

## How to use

### master
```sh
git clone --recursive https://github.com/ffnw/puppet-modules.git puppet-modules-test
git checkout master
git submodule foreach --recursive 'branch="$(git config -f $toplevel/.gitmodules submodule.$name.branch)"; git checkout $branch'
```

### production
```sh
git clone --recursive https://github.com/ffnw/puppet-modules.git puppet-modules-test
git checkout production
git submodule foreach --recursive 'branch="$(git config -f $toplevel/.gitmodules submodule.$name.branch)"; git checkout $branch'
```
