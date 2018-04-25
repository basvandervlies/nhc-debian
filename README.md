# nhc-debian
LBNL Node Health Check build a debian package
To update the submodule: 
 * `git submodule foreach --recursive git pull`
 
 ## Build the package

The following steps to build for example master
 * cd nhc
 * git checkout master
 * ln -s ../debian .
 * dch -n (maybe w must upgrade the version number)
 * debian/rules build
 * fakeroot debian/rules binary
