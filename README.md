# plymouth-theme-yukkuri
-----
# パッケージを作ろう
1. ディレクトリにまとめる

Debian向けの場合
```bash
mkdir pkg
cp -r usr pkg/usr
cp -r DEBIAN/debian pkg/DEBIAN
```

Ubuntu向けの場合
```bash
mkdir pkg
cp -r usr pkg/usr
cp -r DEBIAN/ubuntu pkg/DEBIAN
```

2. 圧縮する
```bash
dpkg-deb -Zxz -b pkg plymouth-theme-yukkuri.deb
```

