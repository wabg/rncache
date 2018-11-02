# rncache

```bash
Error:
Build failed: Unpacking /Users/jaywcjlove/.rncache/boost_1_63_0.tar.gz...
Print: Entry, ":CFBundleIdentifier", Does Not Exist
```

```bash
git clone https://github.com/wabg/rncache.git ~/.rncache
cd .rncache
```

# 错误

```
❌  error: Build input file cannot be found: '../node_modules/react-native/third-party/double-conversion-1.1.6/src/strtod.cc'
▸ Compiling fast-dtoa.cc
❌  error: Build input file cannot be found: '../node_modules/react-native/third-party/double-conversion-1.1.6/src/fast-dtoa.cc'
▸ Compiling fixed-dtoa.cc
❌  error: Build input file cannot be found: '../node_modules/react-native/third-party/double-conversion-1.1.6/src/fixed-dtoa.cc'
▸ Compiling double-conversion.cc
❌  error: Build input file cannot be found: '../node_modules/react-native/third-party/double-conversion-1.1.6/src/double-conversion.cc'
▸ Compiling diy-fp.cc
❌  error: Build input file cannot be found: '../node_modules/react-native/third-party/double-conversion-1.1.6/src/diy-fp.cc'
▸ Compiling cached-powers.cc
❌  error: Build input file cannot be found: '../node_modules/react-native/third-party/double-conversion-1.1.6/src/cached-powers.cc'
▸ Compiling bignum.cc
❌  error: Build input file cannot be found: '../node_modules/react-native/third-party/double-conversion-1.1.6/src/bignum.cc'

```

解决方法

```bash
cd node_modules/react-native/scripts && ./ios-install-third-party.sh && cd ../../../
cd node_modules/react-native/third-party/glog-0.3.5/ && ../../scripts/ios-configure-glog.sh
```
