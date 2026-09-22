参考:
https://www.mingw-w64.org/getting-started/msys2/

環境:
- Windows
- PowerShell
- Visual Studio Code
- MSYS2 UCRT64
- MinGW-w64 (GCC)

## 1. Visual Studio Codeのインストール
https://code.visualstudio.com/

拡張機能:
- C/C++

## 2. MSYS2のインストール
https://www.msys2.org/

`msys2-x86_64-yyyyMMdd.exe`をインストール

```bash
pacman -Syu
pacman -S mingw-w64-ucrt-x86_64-gcc mingw-w64-ucrt-x86_64-gdb
```

システム環境変数`Path`に追加
```text
C:\msys64\ucrt64\bin
```

## 3. ワークスペースに設定ファイルを置く
```text
project/
├── .vscode/
│   ├── c_cpp_properties.json
│   ├── launch.json
│   └── tasks.json
├── main.c
└── main.cpp
```

必要に応じてPowerShellのプロファイルを編集
```powershell
$OutputEncoding = [console]::InputEncoding = [console]::OutputEncoding = New-Object System.Text.UTF8Encoding
```

