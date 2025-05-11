# PongWars_for_Tab5 

M5Stack Tab5（ESP32-P4搭載）上で動作するPong「PongWars」です。
M5Unifiedライブラリを活用しています。

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
オリジナルは M5Stack Core2 用ですが、本リポジトリは M5Stack Tab5（ESP32-P4）向けに移植・拡張しています。

また、pong-warsのオリジナル実装や関連プロジェクトについては下記もご参照ください：
- JavaScript版: https://github.com/vnglst/pong-wars/
- Python版: https://github.com/vocdex/pong-wars-python
- Matlab版: https://github.com/minoue-xx/digital-art-with-matlab


