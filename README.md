# PongWars_for_Tab5 

![image](https://github.com/user-attachments/assets/d7e0d343-1ee9-488e-896e-8c14a24b6619)

https://x.com/anoken2017/status/1921390813499601141

M5Stack Tab5（ESP32-P4搭載）上で動作するPong「PongWars」です。
PlatformIOとM5Unifiedライブラリを使用しています。

## 特徴
- M5Stack Tab5（ESP32-P4）専用
- M5Unified, M5GFXライブラリを使用
- タッチディスプレイでの操作
- 複数のボールや障害物を使ったPong風ゲーム

## ファイル構成
- `src/main.cpp` : ゲームのメインロジック
- `platformio.ini` : PlatformIO用設定ファイル
- `lib/`, `include/` : 必要に応じてライブラリやヘッダを配置

## セットアップ方法
1. [PlatformIO](https://platformio.org/) をインストール
2. 本リポジトリをクローン
3. M5Stack Tab5をPCに接続
4. `platformio.ini` の `env:m5stack-tab5` 設定を確認
5. 以下のコマンドでビルド＆書き込み
   ```
   pio run --target upload
   ```
6. シリアルモニタで動作確認（115200bps）

## 依存ライブラリ
- [M5Unified](https://github.com/m5stack/m5unified)（developブランチ）
- [M5GFX](https://github.com/m5stack/m5gfx)（developブランチ）

`platformio.ini` で自動的にインストールされます。

## 参考・引用元
本プロジェクトは [anoken/pong-wars-forM5Stack](https://github.com/anoken/pong-wars-forM5Stack) を元にTab5に移植・拡張しています。

また、pong-warsのオリジナル実装や関連プロジェクトについては下記もご参照ください：
- JavaScript版: https://github.com/vnglst/pong-wars/

Tab5のPlatformIO IDE 向け設定ファイルは @saitotetsuya -sanの PlatformIO IDE 向け M5Stack 定型コード環境を参考にしました。
https://github.com/3110/m5stack-platformio-boilerplate-code/
