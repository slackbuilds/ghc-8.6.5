## GHC

A ghc-8.6.5 build script.

```
bash-4.3$ diff ghc.SlackBuild.orig ghc.SlackBuild
27,28c27,28
< VERSION=${VERSION:-8.4.3}
< BUILD=${BUILD:-2}
---
> VERSION=${VERSION:-8.6.5}
> BUILD=${BUILD:-1}
72c72
<   tar xvf $CWD/$PRGNAM-$VERSION-$TARARCH-deb8-linux.tar.xz
---
>   tar xvf $CWD/$PRGNAM-$VERSION-$TARARCH-deb9-linux.tar.xz
121c121
< patch -p1 < $CWD/4eebc8016f68719e1ccdf460754a97d1f4d6ef05.patch
---
> # patch -p1 < $CWD/4eebc8016f68719e1ccdf460754a97d1f4d6ef05.patch
bash-4.3$ 
```

This is compatible with [LLVM 6.0.1](https://github.com/varehus/llvm-6.0.1).

See the ghc.info file for the download URLs.