参考:
https://www.mingw-w64.org/getting-started/msys2/

環境:
- Windows
- PowerShell
- Visual Studio Code
- MSYS2 UCRT64
- MinGW-w64 (GCC)

## MSYS2のインストール
https://www.msys2.org/

`msys2-x86_64-yyyyMMdd.exe`をインストール

```bash
$ pacman -Syu
$ pacman -S mingw-w64-ucrt-x86_64-gcc mingw-w64-ucrt-x86_64-gdb
```

システム環境変数`Path`に追加
```
C:\msys64\ucrt64\bin
```
