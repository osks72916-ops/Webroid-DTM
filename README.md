# Webroid//WebUTAU Project 🎤

ブラウザ上で **UTAU (歌声合成ツール)** の基本機能を再現することを目指すプロジェクトです。  
インストール不要で、Webブラウザさえあれば誰でも歌声合成を体験できます。

---

## ✨ Features
- ブラウザ上での歌声合成（リアルタイム再生対応）
- UST (UTAUシーケンスファイル) のインポート / エクスポート
- ピアノロールでのノート編集
- 歌詞入力、音高・長さ・強弱の調整
- 基本的なレンダリングエンジン（WebAssembly + Web Audio API）
- プラグイン的なフィルター機能（リバーブ、EQなど）

---

## 🛠 Technology Stack
- **Frontend:** React, TypeScript, TailwindCSS
- **Audio Engine:** Web Audio API, Tone.js, WebAssembly (Rust / C++ bindings)
- **File Parsing:** WASM で UST ファイルを読み込み
- **Rendering:** Node.js + Express (optional backend for file storage)

---

## 📂 Project Structure
```

/src
/components   → UIコンポーネント
/engine       → 歌声合成エンジン (WASM呼び出し)
/parser       → UST/VSQ ファイルの読み込み
/editor       → ピアノロール、歌詞入力UI
/public
index.html    → エントリーポイント

````

---

## 🚀 Usage
1. プロジェクトを clone  
   ```bash
   git clone https://github.com/yourname/web-utau.git
   cd web-utau
````

2. 依存関係をインストール

   ```bash
   npm install
   ```

3. 開発サーバーを起動

   ```bash
   npm run dev
   ```

4. ブラウザで `http://localhost:3000` を開くとWebUTAUが利用可能 🎶

---

## 🎼 How It Works

1. ユーザーが歌詞とメロディを入力
2. USTライクな内部データ構造に変換
3. WebAssembly製の歌声合成エンジンが波形を生成
4. Web Audio API で再生、または WAV ファイルとして書き出し

---

## 📌 Roadmap

* [ ] フル機能の音源ライブラリ対応（UTAU音源のインポート）
* [ ] タイムストレッチ・ピッチシフトの強化
* [ ] リアルタイム歌詞切り替え
* [ ] VSQ / UST 以外の形式対応
* [ ] モバイル最適化
* [ ] AIベースの補間エンジン統合（将来的に）

---

## 🤝 Contributing

Pull Request & Issue 大歓迎です！
バグ報告や新機能のアイデアは [Issues](https://github.com/yourname/web-utau/issues) へ。

---
## ™️ member

まさかつ / html,CSS,JS,Rust,TS

yakze (@yakze) / JS,CSS,Tailwind

がうちゃん (@gauchan) / CSS,Vim,TS

青林檎 (aoringo01) / React,Tailwind,vanillaJS

## 📜 License

MIT License

```

---
