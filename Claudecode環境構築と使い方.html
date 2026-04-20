<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Claude Code 完全入門ガイド</title>
<style>
* { box-sizing: border-box; margin: 0; padding: 0; }
body {
  font-family: 'Hiragino Sans','Hiragino Kaku Gothic ProN','Noto Sans JP',sans-serif;
  background: #0f0f1a; color: #fff; height: 100vh; overflow: hidden;
}
.slideshow { width:100%; height:100vh; position:relative; }
.slide {
  display:none; width:100%; height:100vh;
  padding: 36px 60px 76px;
  position:absolute; top:0; left:0;
  animation: fadeIn .3s ease;
  overflow-y:auto;
}
.slide.active { display:flex; flex-direction:column; justify-content:center; }
.slide.active.top { justify-content:flex-start; padding-top:36px; }
@keyframes fadeIn { from{opacity:0;transform:translateY(6px)} to{opacity:1;transform:translateY(0)} }

/* テーマ */
.s-title   { background:linear-gradient(135deg,#1a0533,#0a1a3a); }
.s-what    { background:linear-gradient(135deg,#0d1f0d,#0a1a3a); }
.s-prepare { background:linear-gradient(135deg,#1a1a0a,#0a1a3a); }
.s-term    { background:linear-gradient(135deg,#1a0a0a,#0a0a2a); }
.s-nodejs  { background:linear-gradient(135deg,#0a1a0a,#0a1a2a); }
.s-install { background:linear-gradient(135deg,#1a0d1a,#0a1a3a); }
.s-login   { background:linear-gradient(135deg,#0a1a1a,#1a0a1a); }
.s-start   { background:linear-gradient(135deg,#001a1a,#0a0a2a); }
.s-usage   { background:linear-gradient(135deg,#0d0a1a,#1a0a0a); }
.s-end     { background:linear-gradient(135deg,#0a1a0a,#1a0a1a); }
.s-ref     { background:linear-gradient(135deg,#0a0a1a,#1a0a0a); }
.s-trouble { background:linear-gradient(135deg,#1a0a0a,#0a1a1a); }

/* タイポ */
h1 { font-size:40px; font-weight:800; line-height:1.2; margin-bottom:12px; }
h2 { font-size:26px; font-weight:700; margin-bottom:14px; }
h3 { font-size:16px; font-weight:600; margin-bottom:8px; color:#c4b5fd; }
p  { font-size:15px; line-height:1.75; color:#cbd5e1; margin-bottom:8px; }
.hl { color:#c4b5fd; font-weight:700; }
.green { color:#34d399; } .blue { color:#60a5fa; }
.yellow { color:#fbbf24; } .red { color:#f87171; }
.sub { font-size:17px; color:#94a3b8; margin-bottom:24px; }

/* OSタブ */
.os-tabs { display:flex; gap:8px; margin-bottom:16px; flex-wrap:wrap; }
.os-tab { padding:5px 18px; border-radius:20px; font-size:13px; font-weight:600; cursor:pointer; border:2px solid transparent; transition:all .2s; }
.os-tab.mac  { background:#1c1c2e; border-color:#a78bfa; color:#a78bfa; }
.os-tab.win  { background:#1c1c2e; border-color:#60a5fa; color:#60a5fa; }
.os-tab.both { background:#1c1c2e; border-color:#34d399; color:#34d399; }
.os-tab.active.mac  { background:#a78bfa; color:#0f0f1a; }
.os-tab.active.win  { background:#60a5fa; color:#0f0f1a; }
.os-tab.active.both { background:#34d399; color:#0f0f1a; }
.os-content { display:none; }
.os-content.active { display:block; }

/* コードブロック */
.code {
  background:#1e1e2e; border:1px solid #2d2d3e; border-radius:10px;
  padding:12px 16px; font-family:'Menlo','Consolas',monospace;
  font-size:14px; color:#a5f3fc; margin:8px 0;
  position:relative; white-space:pre; overflow-x:auto; line-height:1.65;
}
.code .cmd { color:#86efac; }
.code .out { color:#94a3b8; }
.code .cm  { color:#4b5563; }
.copy-btn {
  position:absolute; top:8px; right:8px;
  background:#374151; border:none; border-radius:6px;
  color:#9ca3af; font-size:11px; padding:3px 9px;
  cursor:pointer; transition:all .2s; font-family:inherit;
}
.copy-btn:hover { background:#4b5563; color:#fff; }
.copy-btn.ok { background:#065f46; color:#34d399; }

/* ターミナル */
.term {
  background:#111827; border-radius:10px; overflow:hidden;
  margin:8px 0; font-family:'Menlo','Consolas',monospace; font-size:13px;
}
.term-bar { background:#1f2937; padding:6px 12px; display:flex; align-items:center; gap:6px; }
.dot { width:10px; height:10px; border-radius:50%; }
.dr { background:#ff5f57; } .dy { background:#febc2e; } .dg { background:#28c840; }
.term-title { color:#6b7280; font-size:11px; margin-left:6px; }
.term-body { padding:10px 14px; line-height:1.75; }
.tp { color:#6b7280; } .tc { color:#86efac; } .to { color:#94a3b8; } .te { color:#f87171; }

/* カード */
.cards { display:grid; gap:12px; }
.col2 { grid-template-columns:1fr 1fr; }
.col3 { grid-template-columns:1fr 1fr 1fr; }
.card { background:#1e1e2e; border:1px solid #2d2d3e; border-radius:12px; padding:16px; }

/* ステップ */
.steps { display:flex; flex-direction:column; gap:8px; }
.step { display:flex; align-items:flex-start; gap:12px; background:#1e1e2e; border-radius:10px; padding:12px; }
.sn { min-width:28px; height:28px; background:#a78bfa; color:#0f0f1a; border-radius:50%; display:flex; align-items:center; justify-content:center; font-weight:800; font-size:13px; flex-shrink:0; }
.sn.b { background:#60a5fa; }
.sb h4 { color:#e2e8f0; font-size:14px; margin-bottom:3px; }
.sb p  { font-size:13px; margin-bottom:0; color:#94a3b8; }

/* アラート */
.alert { border-radius:10px; padding:11px 15px; margin:8px 0; font-size:14px; line-height:1.65; }
.warn    { background:#2d1b00; border-left:4px solid #fbbf24; color:#fde68a; }
.info    { background:#0c1f3d; border-left:4px solid #60a5fa; color:#bfdbfe; }
.ok      { background:#052e16; border-left:4px solid #34d399; color:#a7f3d0; }
.purple  { background:#1a0d2e; border-left:4px solid #a78bfa; color:#ddd6fe; }
.company { background:#0f2a0f; border-left:4px solid #22c55e; color:#bbf7d0; }

/* 確認ボックス（大） */
.check-box {
  background:#052e16; border:2px solid #34d399; border-radius:12px;
  padding:14px 18px; margin:10px 0;
}
.check-box .check-title { color:#34d399; font-size:15px; font-weight:700; margin-bottom:6px; }
.check-box .term { margin:6px 0 0; }

/* 2カラム */
.two { display:grid; grid-template-columns:1fr 1fr; gap:16px; align-items:start; }

/* バッジ */
.badge { display:inline-block; padding:2px 9px; border-radius:12px; font-size:11px; font-weight:700; margin-right:4px; vertical-align:middle; }
.bm  { background:#3b1f6e; color:#c4b5fd; }
.bw  { background:#1e3a5f; color:#93c5fd; }
.bb  { background:#064e3b; color:#6ee7b7; }
.bnew{ background:#134e4a; color:#5eead4; }
.bco { background:#14532d; color:#86efac; }

/* 画像フレーム */
.img-box { border-radius:10px; overflow:hidden; border:1px solid #2d2d3e; margin:8px 0; background:#1e1e2e; }
.img-box img { width:100%; display:block; max-height:180px; object-fit:contain; background:#fff; }
.img-box.dark-bg img { background:#1e1e2e; }
.img-cap { padding:5px 12px; font-size:11px; color:#6b7280; text-align:center; background:#1e1e2e; }

/* テーブル */
table { width:100%; border-collapse:collapse; font-size:14px; margin:8px 0; }
th { background:#1e293b; color:#94a3b8; font-size:12px; text-transform:uppercase; letter-spacing:.04em; padding:8px 12px; text-align:left; }
td { padding:10px 12px; border-bottom:1px solid #1e293b; color:#cbd5e1; }
tr:last-child td { border-bottom:none; }

/* ナビ */
.nav {
  position:fixed; bottom:0; left:0; right:0;
  display:flex; justify-content:space-between; align-items:center;
  padding:11px 28px;
  background:rgba(15,15,26,.97); backdrop-filter:blur(8px);
  border-top:1px solid #1e1e2e; z-index:100;
}
.nb { background:#1e1e2e; border:1px solid #333; color:#e2e8f0; padding:7px 20px; border-radius:8px; font-size:13px; cursor:pointer; transition:all .2s; font-family:inherit; }
.nb:hover { background:#2d2d3e; border-color:#a78bfa; }
.nb:disabled { opacity:.3; cursor:default; }
.sc { color:#6b7280; font-size:12px; }
.progress-bar { height:3px; background:#1e1e2e; position:fixed; top:0; left:0; right:0; z-index:100; }
.pf { height:100%; background:linear-gradient(90deg,#a78bfa,#60a5fa); transition:width .3s ease; }

/* kbdキー */
kbd { background:#2d2d3e; border:1px solid #555; border-radius:4px; padding:2px 7px; font-size:12px; font-family:inherit; }
</style>
</head>
<body>
<div class="progress-bar"><div class="pf" id="pf"></div></div>
<div class="slideshow" id="ss">

<!-- 1: タイトル -->
<div class="slide s-title active">
  <div style="text-align:center;">
    <div style="font-size:60px;margin-bottom:14px;">🤖</div>
    <h1>Claude Code<br>完全入門ガイド</h1>
    <p class="sub">はじめてでも一人でできる・環境構築から動かすまで</p>
    <div style="display:flex;justify-content:center;gap:12px;margin:18px 0;">
      <div style="padding:8px 24px;border-radius:30px;border:2px solid #a78bfa;color:#c4b5fd;font-size:16px;font-weight:700;background:#a78bfa20;">🍎 Mac</div>
      <div style="padding:8px 24px;border-radius:30px;border:2px solid #60a5fa;color:#93c5fd;font-size:16px;font-weight:700;background:#60a5fa20;">🪟 Windows</div>
    </div>
    <div class="alert company" style="display:inline-block;margin-top:8px;font-size:14px;">
      🏢 会社のClaudeアカウントをお持ちの方向けに最適化済み
    </div>
    <p style="color:#4b5563;font-size:12px;margin-top:16px;">← → キーまたは下のボタンで次のスライドへ</p>
  </div>
</div>

<!-- 2: 全体の流れ -->
<div class="slide s-what">
  <h2>📍 全体の流れ（これだけ覚えれば大丈夫！）</h2>
  <div class="cards col3" style="margin-top:16px;">
    <div class="card" style="border-color:#a78bfa;text-align:center;">
      <div style="font-size:32px;margin-bottom:8px;">①</div>
      <h3 style="text-align:center;">準備する</h3>
      <p style="font-size:13px;text-align:center;">ターミナルを開く<br>Node.jsを入れる<br>Claude Codeを入れる<br><span style="color:#4b5563;">（最初の1回だけ）</span></p>
    </div>
    <div class="card" style="border-color:#60a5fa;text-align:center;">
      <div style="font-size:32px;margin-bottom:8px;">②</div>
      <h3 style="text-align:center;color:#93c5fd;">ログインする</h3>
      <p style="font-size:13px;text-align:center;">会社のClaudeアカウントで<br>ログイン<br><span style="color:#4b5563;">（最初の1回だけ）</span></p>
    </div>
    <div class="card" style="border-color:#34d399;text-align:center;">
      <div style="font-size:32px;margin-bottom:8px;">③</div>
      <h3 style="text-align:center;color:#34d399;">毎日使う</h3>
      <p style="font-size:13px;text-align:center;">ターミナルを開く<br>claudeと入力<br>日本語で話しかける</p>
    </div>
  </div>
  <div class="alert info" style="margin-top:16px;">
    💡 <strong>①②は最初の1回だけ</strong>です。次の日からは③だけで使えます！
  </div>
  <div class="alert company" style="margin-top:8px;">
    🏢 会社のClaudeアカウントがあるので、<strong>APIキーの取得や課金設定は不要</strong>です。
  </div>
</div>

<!-- 3: ターミナルとは -->
<div class="slide s-term">
  <h2>🖥️ ターミナルとは？</h2>
  <p>ターミナルとは<span class="hl">文字を打ち込んでパソコンに命令する画面</span>です。</p>
  <div class="cards col2" style="margin-top:12px;">
    <div class="card">
      <h3>📌 普通のパソコン操作との違い</h3>
      <table style="margin-top:8px;">
        <tr><th>普段の操作</th><th>ターミナル</th></tr>
        <tr><td>アイコンをクリック</td><td>文字を打ち込む</td></tr>
        <tr><td>マウスで操作</td><td>キーボードで操作</td></tr>
        <tr><td>見た目でわかる</td><td>コマンドを覚える</td></tr>
      </table>
    </div>
    <div class="card">
      <h3>📌 ターミナルの見た目</h3>
      <div class="term" style="margin-top:8px;">
        <div class="term-bar"><div class="dot dr"></div><div class="dot dy"></div><div class="dot dg"></div><span class="term-title">ターミナル</span></div>
        <div class="term-body">
          <div><span class="tp">yourname@Mac ~ </span><span class="tc">%</span> <span style="color:#fff;">█</span></div>
          <div style="color:#4b5563;font-size:12px;margin-top:4px;">↑ここに命令を入力する</div>
        </div>
      </div>
      <div class="term" style="margin-top:6px;">
        <div class="term-bar"><span class="term-title" style="margin-left:0;">Windows PowerShell</span></div>
        <div class="term-body">
          <div><span class="tp">PS C:\Users\yourname&gt; </span><span style="color:#fff;">█</span></div>
          <div style="color:#4b5563;font-size:12px;margin-top:4px;">↑ここに命令を入力する</div>
        </div>
      </div>
    </div>
  </div>
  <div class="alert warn" style="margin-top:12px;">
    ⚠️ <strong>大事なルール：</strong>コマンドを入力したら必ず <kbd>Enter</kbd> を押して実行してください。
  </div>
</div>

<!-- 4: ターミナルの開き方 -->
<div class="slide s-term top">
  <h2>🖥️ ターミナルの開き方</h2>
  <div class="os-tabs" id="tab-t">
    <div class="os-tab mac active" onclick="sw('t','mac')">🍎 Mac</div>
    <div class="os-tab win" onclick="sw('t','win')">🪟 Windows</div>
  </div>

  <div id="t-mac" class="os-content active">
    <div class="two">
      <div>
        <div class="steps">
          <div class="step">
            <div class="sn">1</div>
            <div class="sb">
              <h4>キーボードを押す</h4>
              <p><kbd>⌘ Command</kbd> を押しながら <kbd>スペース</kbd> を押す</p>
            </div>
          </div>
          <div class="step">
            <div class="sn">2</div>
            <div class="sb">
              <h4>「ターミナル」と入力</h4>
              <p>画面中央に検索バーが出てくる<br>「ターミナル」と日本語で入力する</p>
            </div>
          </div>
          <div class="step">
            <div class="sn">3</div>
            <div class="sb">
              <h4>「ターミナル.app」をクリック</h4>
              <p>一覧の一番上に出てくるものをクリックする</p>
            </div>
          </div>
        </div>
        <div class="alert warn" style="margin-top:10px;font-size:13px;">
          ⚠️ <strong>貼り付けは <kbd>⌘ Command</kbd> + <kbd>V</kbd></strong>（Ctrl+Vではない）
        </div>
      </div>
      <div>
        <div class="img-box dark-bg">
          <img src="https://help.apple.com/assets/694058E34AF4DEFE100B21F0/694058E5E47399E70903F18D/en_US/fe66109d1c446abfb01861b47ef61791.png" alt="Mac Spotlight" loading="lazy" onerror="this.parentElement.style.display='none'">
        </div>
        <p class="img-cap">Spotlight検索の画面（出典：Apple）</p>
        <div class="check-box" style="margin-top:8px;">
          <div class="check-title">✅ こうなればOK！</div>
          <div class="term">
            <div class="term-bar"><div class="dot dr"></div><div class="dot dy"></div><div class="dot dg"></div><span class="term-title">ターミナル</span></div>
            <div class="term-body">
              <div><span class="to">Last login: Thu Apr 17...</span></div>
              <div><span class="tp">yourname@MacBook ~ </span><span class="tc">%</span> <span style="color:#fff;">█</span></div>
            </div>
          </div>
          <p style="font-size:13px;margin-top:6px;color:#6ee7b7;">「%」の後ろにカーソルが点滅したら成功！</p>
        </div>
      </div>
    </div>
  </div>

  <div id="t-win" class="os-content">
    <div class="two">
      <div>
        <div class="steps">
          <div class="step">
            <div class="sn b">1</div>
            <div class="sb">
              <h4>Windowsキーを押す</h4>
              <p>キーボード左下の <kbd>⊞</kbd> キーを押す</p>
            </div>
          </div>
          <div class="step">
            <div class="sn b">2</div>
            <div class="sb">
              <h4>「powershell」と入力</h4>
              <p>スタートメニューが開いたらそのまま「powershell」と入力する</p>
            </div>
          </div>
          <div class="step">
            <div class="sn b">3</div>
            <div class="sb">
              <h4>「Windows PowerShell」をクリック</h4>
              <p>検索結果に出てきた「Windows PowerShell」をクリック</p>
            </div>
          </div>
        </div>
        <div class="alert warn" style="margin-top:10px;font-size:13px;">
          ⚠️ <strong>貼り付けは右クリック → 貼り付け</strong>（または <kbd>Ctrl</kbd>+<kbd>V</kbd>）
        </div>
      </div>
      <div>
        <div class="img-box">
          <img src="https://learn.microsoft.com/en-us/windows/terminal/images/settings-default-shell.png" alt="Windows Terminal" loading="lazy" onerror="this.parentElement.style.display='none'">
        </div>
        <p class="img-cap">Windows Terminal の画面（出典：Microsoft）</p>
        <div class="check-box" style="margin-top:8px;">
          <div class="check-title">✅ こうなればOK！</div>
          <div class="term">
            <div class="term-bar"><span class="term-title" style="margin-left:0;">Windows PowerShell</span></div>
            <div class="term-body">
              <div><span class="to">Windows PowerShell</span></div>
              <div><span class="to">Copyright (C) Microsoft...</span></div>
              <div style="margin-top:4px;"><span class="tp">PS C:\Users\yourname&gt; </span><span style="color:#fff;">█</span></div>
            </div>
          </div>
          <p style="font-size:13px;margin-top:6px;color:#6ee7b7;">「PS C:\Users\...>」が出たら成功！</p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- 5: Node.jsのインストール -->
<div class="slide s-nodejs top">
  <h2>📦 Node.jsのインストール</h2>
  <p style="margin-bottom:10px;">開発環境として入れておくと便利です。まずインストール済みか確認しましょう。</p>
  <div class="os-tabs" id="tab-n">
    <div class="os-tab both active" onclick="sw('n','both')">🍎🪟 共通手順</div>
  </div>
  <div id="n-both" class="os-content active">
    <div class="two">
      <div>
        <p style="font-size:14px;margin-bottom:6px;"><strong>Step 1：バージョン確認コマンドを入力</strong></p>
        <div class="code"><span class="cmd">node --version</span><button class="copy-btn" onclick="cp('node --version',this)">コピー</button></div>
        <div class="check-box">
          <div class="check-title">✅ v18以上が出たら次のスライドへ</div>
          <div class="term"><div class="term-body"><div><span class="tc">node --version</span></div><div><span class="to">v20.11.0  ← これが出たらOK！</span></div></div></div>
        </div>
        <div class="alert warn" style="margin-top:8px;">
          ❌ <strong>エラーが出た場合 → 右の手順でインストール</strong>
        </div>
      </div>
      <div>
        <p style="font-size:14px;margin-bottom:6px;"><strong>エラーが出た場合のインストール手順</strong></p>
        <div class="steps">
          <div class="step">
            <div class="sn">1</div>
            <div class="sb">
              <h4>ブラウザで nodejs.org を開く</h4>
              <p>URLバーに「nodejs.org」と入力してEnter</p>
            </div>
          </div>
          <div class="step">
            <div class="sn">2</div>
            <div class="sb">
              <h4>「LTS」の緑ボタンをクリック</h4>
              <p>「推奨版」と書いてある方をクリック<br>（Current ではなく LTS を選ぶ）</p>
            </div>
          </div>
          <div class="step">
            <div class="sn">3</div>
            <div class="sb">
              <h4>ダウンロードしたファイルを開く</h4>
              <p>Mac：.pkgファイル　Windows：.msiファイル<br>「次へ」「Continue」を押し続ける</p>
            </div>
          </div>
          <div class="step">
            <div class="sn">4</div>
            <div class="sb">
              <h4>ターミナルを閉じて開き直す</h4>
              <p>インストール完了後、ターミナルを一度閉じて再度開く</p>
            </div>
          </div>
          <div class="step">
            <div class="sn">5</div>
            <div class="sb">
              <h4>再度確認コマンドを入力</h4>
              <div class="code" style="margin-top:4px;font-size:12px;"><span class="cmd">node --version</span>
<span class="cmd">npm --version</span></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- 6: Claude Codeのインストール -->
<div class="slide s-install top">
  <h2>🚀 Claude Codeのインストール</h2>
  <div class="alert purple" style="margin-bottom:12px;">✨ Node.jsとは別の専用インストーラーを使います。1コマンドで完了！</div>
  <div class="os-tabs" id="tab-i">
    <div class="os-tab mac active" onclick="sw('i','mac')">🍎 Mac</div>
    <div class="os-tab win" onclick="sw('i','win')">🪟 Windows</div>
  </div>

  <div id="i-mac" class="os-content active">
    <div class="two">
      <div>
        <div class="steps">
          <div class="step">
            <div class="sn">1</div>
            <div class="sb">
              <h4>コマンドをコピーする</h4>
              <p>右のボタンを押すか、コマンドをすべて選択してコピー</p>
            </div>
          </div>
          <div class="step">
            <div class="sn">2</div>
            <div class="sb">
              <h4>ターミナルに貼り付ける</h4>
              <p><kbd>⌘ Command</kbd> + <kbd>V</kbd> で貼り付け</p>
            </div>
          </div>
          <div class="step">
            <div class="sn">3</div>
            <div class="sb">
              <h4>Enterを押して実行</h4>
              <p>しばらく待つ（30秒〜1分程度）</p>
            </div>
          </div>
        </div>
        <div class="code" style="margin-top:12px;"><span class="cmd">curl -fsSL https://claude.ai/install.sh | bash</span><button class="copy-btn" onclick="cp('curl -fsSL https://claude.ai/install.sh | bash',this)">コピー</button></div>
      </div>
      <div>
        <div class="check-box">
          <div class="check-title">✅ インストール成功の画面</div>
          <div class="term">
            <div class="term-bar"><div class="dot dr"></div><div class="dot dy"></div><div class="dot dg"></div></div>
            <div class="term-body" style="font-size:12px;">
              <div><span class="tc">% curl -fsSL https://claude.ai/install.sh | bash</span></div>
              <div><span class="to">Installing Claude Code...</span></div>
              <div><span class="to">✓ Downloaded</span></div>
              <div><span class="to">✓ Installed successfully</span></div>
              <div style="margin-top:4px;"><span class="tp">% </span><span style="color:#fff;">█ ← ここに戻ってきたら完了</span></div>
            </div>
          </div>
          <p style="font-size:13px;margin-top:6px;color:#6ee7b7;">「%」が戻ってきたらインストール完了！</p>
        </div>
        <p style="font-size:14px;margin-top:10px;margin-bottom:4px;"><strong>確認コマンド：</strong></p>
        <div class="code"><span class="cmd">claude --version</span>
<span class="out">1.x.x  ← バージョンが出ればOK</span></div>
      </div>
    </div>
  </div>

  <div id="i-win" class="os-content">
    <div class="two">
      <div>
        <div class="steps">
          <div class="step">
            <div class="sn b">1</div>
            <div class="sb">
              <h4>コマンドをコピーする</h4>
              <p>右のコピーボタンを押す</p>
            </div>
          </div>
          <div class="step">
            <div class="sn b">2</div>
            <div class="sb">
              <h4>PowerShellに貼り付ける</h4>
              <p>PowerShellの画面で右クリック → 「貼り付け」</p>
            </div>
          </div>
          <div class="step">
            <div class="sn b">3</div>
            <div class="sb">
              <h4>Enterを押して実行</h4>
              <p>しばらく待つ（30秒〜1分程度）</p>
            </div>
          </div>
        </div>
        <div class="code" style="margin-top:12px;"><span class="cmd">irm https://claude.ai/install.ps1 | iex</span><button class="copy-btn" onclick="cp('irm https://claude.ai/install.ps1 | iex',this)">コピー</button></div>
        <div class="alert warn" style="margin-top:8px;font-size:13px;">
          ⚠️ <strong>事前にGit for Windowsが必要です</strong><br>
          エラーが出た場合は <strong>git-scm.com/downloads/win</strong> でインストール後に再試行
        </div>
      </div>
      <div>
        <div class="check-box">
          <div class="check-title">✅ インストール成功の画面</div>
          <div class="term">
            <div class="term-bar"><span class="term-title" style="margin-left:0;">PowerShell</span></div>
            <div class="term-body" style="font-size:12px;">
              <div><span class="tc">&gt; irm https://claude.ai/install.ps1 | iex</span></div>
              <div><span class="to">Installing Claude Code...</span></div>
              <div><span class="to">✓ Installed successfully</span></div>
              <div style="margin-top:4px;"><span class="tp">PS C:\...&gt; </span><span style="color:#fff;">█ ← 戻ってきたら完了</span></div>
            </div>
          </div>
          <p style="font-size:13px;margin-top:6px;color:#6ee7b7;">「PS C:\...&gt;」が戻ってきたら完了！</p>
        </div>
        <p style="font-size:14px;margin-top:10px;margin-bottom:4px;"><strong>確認コマンド：</strong></p>
        <div class="code"><span class="cmd">claude --version</span>
<span class="out">1.x.x  ← バージョンが出ればOK</span></div>
      </div>
    </div>
  </div>
</div>

<!-- 7: ログイン -->
<div class="slide s-login top">
  <h2>🔑 ログイン（会社アカウントで）</h2>
  <div class="alert company" style="margin-bottom:12px;">
    🏢 <strong>会社のClaudeアカウントでログインします。APIキーは不要です。</strong>
  </div>

  <!-- 招待リンクボックス -->
  <div style="background:#0f2a0f;border:2px solid #22c55e;border-radius:12px;padding:14px 18px;margin-bottom:14px;display:flex;align-items:center;gap:16px;flex-wrap:wrap;">
    <div style="font-size:22px;">🔗</div>
    <div style="flex:1;">
      <div style="font-size:14px;font-weight:700;color:#86efac;margin-bottom:4px;">【事前準備】まず招待リンクからorganizationに参加してください</div>
      <a href="https://claude.ai/join/org/PyHXom_4AZrW-KAU32gXQQ"
         target="_blank"
         style="display:inline-block;background:#16a34a;color:#fff;font-size:13px;font-weight:700;padding:7px 18px;border-radius:8px;text-decoration:none;margin-top:4px;">
        ▶ 会社の組織に参加する（クリック）
      </a>
      <div style="font-size:12px;color:#4ade80;margin-top:6px;">ブラウザでこのページが開きます → 会社メールでサインアップ or ログイン</div>
    </div>
  </div>

  <div class="two">
    <div>
      <div class="steps">
        <div class="step">
          <div class="sn">1</div>
          <div class="sb">
            <h4>Claude Codeを起動する</h4>
            <div class="code" style="margin-top:4px;"><span class="cmd">claude</span></div>
            <p>ターミナルに入力してEnter</p>
          </div>
        </div>
        <div class="step">
          <div class="sn">2</div>
          <div class="sb">
            <h4>ログインコマンドを入力</h4>
            <div class="code" style="margin-top:4px;"><span class="cmd">/login</span></div>
            <p>「&gt;」の後ろに入力してEnter</p>
          </div>
        </div>
        <div class="step">
          <div class="sn">3</div>
          <div class="sb">
            <h4>ブラウザが自動で開く</h4>
            <p>claude.ai のログイン画面が開く</p>
          </div>
        </div>
        <div class="step">
          <div class="sn">4</div>
          <div class="sb">
            <h4>会社のメールでログイン</h4>
            <p>会社のメールアドレスとパスワードを入力</p>
          </div>
        </div>
        <div class="step">
          <div class="sn">5</div>
          <div class="sb">
            <h4>ターミナルに戻る</h4>
            <p>認証完了 → ターミナルが自動で続きを始める</p>
          </div>
        </div>
      </div>
    </div>
    <div>
      <div class="check-box">
        <div class="check-title">✅ ログイン成功の画面</div>
        <div class="term">
          <div class="term-bar"><div class="dot dr"></div><div class="dot dy"></div><div class="dot dg"></div></div>
          <div class="term-body" style="font-size:12px;">
            <div><span class="tc">% claude</span></div>
            <div class="to" style="margin-top:4px;">╔══════════════════════════╗</div>
            <div class="to">║   Claude Code  v1.x      ║</div>
            <div class="to">╚══════════════════════════╝</div>
            <div style="margin-top:6px;"><span style="color:#a78bfa;">&gt; </span><span class="tc">/login</span></div>
            <div class="to">Opening browser for authentication...</div>
            <div class="to">✓ Logged in as you@company.com</div>
            <div style="margin-top:4px;"><span style="color:#a78bfa;">&gt; </span><span style="color:#fff;">█</span></div>
          </div>
        </div>
        <p style="font-size:13px;margin-top:6px;color:#6ee7b7;">メールアドレスが表示されたらログイン成功！</p>
      </div>
      <div class="alert ok" style="margin-top:10px;">
        ✅ 一度ログインすれば<strong>次回から自動でログイン</strong>されます。毎回入力する必要はありません。
      </div>
      <div class="alert info" style="margin-top:8px;font-size:13px;">
        💡 ブラウザが開かない場合は、ターミナルに表示されるURLをコピーしてブラウザに貼り付けてください。
      </div>
    </div>
  </div>
</div>

<!-- 8: 毎回の始め方 -->
<div class="slide s-start top">
  <h2>▶️ 毎回の始め方（2ステップだけ！）</h2>
  <div class="os-tabs" id="tab-s">
    <div class="os-tab mac active" onclick="sw('s','mac')">🍎 Mac</div>
    <div class="os-tab win" onclick="sw('s','win')">🪟 Windows</div>
  </div>

  <div id="s-mac" class="os-content active">
    <div class="two">
      <div>
        <div class="steps">
          <div class="step">
            <div class="sn">1</div>
            <div class="sb">
              <h4>ターミナルを開く</h4>
              <p><kbd>⌘</kbd> + <kbd>スペース</kbd> → 「ターミナル」→ Enter</p>
            </div>
          </div>
          <div class="step">
            <div class="sn">2</div>
            <div class="sb">
              <h4>作業したいフォルダに移動</h4>
              <div class="code" style="margin-top:4px;"><span class="cmd">cd ~/Desktop</span><span class="cm">      # デスクトップへ</span>
<span class="cmd">cd ~/Documents</span><span class="cm">   # 書類フォルダへ</span>
<span class="cmd">cd フォルダ名</span><span class="cm">     # 指定フォルダへ</span></div>
              <p style="font-size:12px;margin-top:4px;"><code style="background:#1e1e2e;padding:1px 5px;border-radius:3px;">cd</code> = 「Change Directory」フォルダを移動するコマンド</p>
            </div>
          </div>
          <div class="step">
            <div class="sn">3</div>
            <div class="sb">
              <h4>Claude Codeを起動！</h4>
              <div class="code" style="margin-top:4px;"><span class="cmd">claude</span></div>
            </div>
          </div>
        </div>
        <div class="alert info" style="margin-top:10px;font-size:13px;">
          💡 特定のフォルダに移動しなくても <code style="background:#0c1f3d;padding:1px 6px;border-radius:3px;">claude</code> だけで起動できます。
        </div>
      </div>
      <div>
        <div class="check-box">
          <div class="check-title">✅ 起動成功の画面</div>
          <div class="term">
            <div class="term-bar"><div class="dot dr"></div><div class="dot dy"></div><div class="dot dg"></div></div>
            <div class="term-body" style="font-size:12px;">
              <div><span class="tp">~ % </span><span class="tc">cd ~/Desktop</span></div>
              <div><span class="tp">Desktop % </span><span class="tc">claude</span></div>
              <div class="to" style="margin-top:6px;">╔══════════════════════════╗</div>
              <div class="to">║   Claude Code  v1.x      ║</div>
              <div class="to">╚══════════════════════════╝</div>
              <div style="margin-top:6px;"><span style="color:#a78bfa;">&gt; </span><span style="color:#fff;">█</span></div>
            </div>
          </div>
          <p style="font-size:13px;margin-top:6px;color:#6ee7b7;">「&gt;」が出たら話しかけられる状態！</p>
        </div>
      </div>
    </div>
  </div>

  <div id="s-win" class="os-content">
    <div class="two">
      <div>
        <div class="steps">
          <div class="step">
            <div class="sn b">1</div>
            <div class="sb">
              <h4>PowerShellを開く</h4>
              <p><kbd>⊞</kbd> キー → 「powershell」→ Enter</p>
            </div>
          </div>
          <div class="step">
            <div class="sn b">2</div>
            <div class="sb">
              <h4>作業したいフォルダに移動</h4>
              <div class="code" style="margin-top:4px;"><span class="cmd">cd $HOME\Desktop</span><span class="cm">    # デスクトップへ</span>
<span class="cmd">cd $HOME\Documents</span><span class="cm"> # ドキュメントへ</span>
<span class="cmd">cd フォルダ名</span><span class="cm">       # 指定フォルダへ</span></div>
            </div>
          </div>
          <div class="step">
            <div class="sn b">3</div>
            <div class="sb">
              <h4>Claude Codeを起動！</h4>
              <div class="code" style="margin-top:4px;"><span class="cmd">claude</span></div>
            </div>
          </div>
        </div>
      </div>
      <div>
        <div class="check-box">
          <div class="check-title">✅ 起動成功の画面</div>
          <div class="term">
            <div class="term-bar"><span class="term-title" style="margin-left:0;">PowerShell</span></div>
            <div class="term-body" style="font-size:12px;">
              <div><span class="tp">PS C:\...&gt; </span><span class="tc">cd $HOME\Desktop</span></div>
              <div><span class="tp">Desktop&gt; </span><span class="tc">claude</span></div>
              <div class="to" style="margin-top:6px;">╔══════════════════════════╗</div>
              <div class="to">║   Claude Code  v1.x      ║</div>
              <div class="to">╚══════════════════════════╝</div>
              <div style="margin-top:6px;"><span style="color:#a78bfa;">&gt; </span><span style="color:#fff;">█</span></div>
            </div>
          </div>
          <p style="font-size:13px;margin-top:6px;color:#6ee7b7;">「&gt;」が出たら話しかけられる状態！</p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- 9: 使い方 -->
<div class="slide s-usage top">
  <h2>💬 基本的な使い方</h2>
  <div class="two">
    <div>
      <p style="margin-bottom:10px;"><span class="badge bb">共通</span> 「&gt;」の後ろに<span class="hl">日本語でそのまま</span>話しかけます。</p>
      <div class="card" style="margin-bottom:10px;">
        <h3>📝 こんなことを頼めます</h3>
        <div class="term" style="margin-top:8px;">
          <div class="term-body" style="font-size:13px;line-height:2;">
            <div><span style="color:#a78bfa;">&gt; </span>このフォルダにあるファイルを教えて</div>
            <div><span style="color:#a78bfa;">&gt; </span>index.htmlを作ってHello Worldを表示して</div>
            <div><span style="color:#a78bfa;">&gt; </span>このコードを日本語で説明して</div>
            <div><span style="color:#a78bfa;">&gt; </span>エラーを直して</div>
            <div><span style="color:#a78bfa;">&gt; </span>このファイルをCSVに変換するコードを書いて</div>
          </div>
        </div>
      </div>
      <div class="card">
        <h3>⌨️ キーボード操作まとめ</h3>
        <table style="margin-top:6px;">
          <tr><td style="font-size:13px;"><kbd>Enter</kbd></td><td style="font-size:13px;">送信する</td></tr>
          <tr><td style="font-size:13px;"><kbd>Shift</kbd>+<kbd>Enter</kbd></td><td style="font-size:13px;">改行する（送信しない）</td></tr>
          <tr><td style="font-size:13px;"><kbd>↑</kbd> キー</td><td style="font-size:13px;">前のコマンドを呼び出す</td></tr>
          <tr><td style="font-size:13px;"><kbd>Ctrl</kbd>+<kbd>C</kbd></td><td style="font-size:13px;">キャンセルする</td></tr>
        </table>
      </div>
    </div>
    <div>
      <div class="img-box dark-bg" style="margin-bottom:8px;">
        <img src="https://github.com/anthropics/claude-code/raw/main/demo.gif" alt="Claude Code デモ" style="max-height:200px;" loading="lazy" onerror="this.parentElement.innerHTML='<div style=\'padding:30px;text-align:center;color:#6b7280;font-size:13px;\'>デモ GIF を読み込み中...</div>'">
      </div>
      <p class="img-cap">Claude Code の実際の動作（出典：Anthropic GitHub）</p>
      <div class="card" style="margin-top:8px;">
        <h3>/ コマンド（特別な命令）</h3>
        <div class="code" style="margin-top:6px;font-size:13px;"><span class="cmd">/help</span>   <span class="cm"># 使い方を確認する</span>
<span class="cmd">/clear</span>  <span class="cm"># 会話をリセットする</span>
<span class="cmd">/login</span>  <span class="cm"># ログインし直す</span>
<span class="cmd">/quit</span>   <span class="cm"># 終了する</span></div>
      </div>
    </div>
  </div>
</div>

<!-- 10: 毎回の終わり方 -->
<div class="slide s-end">
  <h2>⏹️ 毎回の終わり方</h2>
  <p style="margin-bottom:16px;"><span class="badge bb">Mac / Windows 共通</span></p>
  <div class="cards col2">
    <div class="card">
      <h3>方法①　コマンドで終了（推奨）</h3>
      <div class="code" style="margin-top:8px;"><span class="cmd">/quit</span></div>
      <div class="term" style="margin-top:8px;">
        <div class="term-body" style="font-size:13px;">
          <div><span style="color:#a78bfa;">&gt; </span><span class="tc">/quit</span></div>
          <div class="to" style="margin-top:4px;">Goodbye! 👋</div>
          <div style="margin-top:4px;"><span class="tp">% </span><span style="color:#4b5563;">← 元の画面に戻ったら終了完了</span></div>
        </div>
      </div>
    </div>
    <div class="card">
      <h3>方法②　キーボードで終了</h3>
      <p style="margin-top:10px;font-size:15px;">
        <kbd>Ctrl</kbd> + <kbd>C</kbd> を <strong>2回</strong> 押す
      </p>
      <p style="margin-top:10px;font-size:14px;color:#94a3b8;">その後、ターミナルのウィンドウを × で閉じてOKです。</p>
    </div>
  </div>
  <div class="check-box" style="margin-top:16px;">
    <div class="check-title">✅ 完全終了の流れ</div>
    <p style="font-size:14px;color:#6ee7b7;margin-top:6px;">
      <code style="background:#052e16;padding:2px 8px;border-radius:4px;">/quit</code>
      でClaude Code終了 →
      ターミナルのウィンドウを × で閉じる
      → 完了！
    </p>
  </div>
</div>

<!-- 11: コマンド一覧 -->
<div class="slide s-ref top">
  <h2>📌 コマンド一覧</h2>
  <div class="os-tabs" id="tab-r">
    <div class="os-tab mac active" onclick="sw('r','mac')">🍎 Mac</div>
    <div class="os-tab win" onclick="sw('r','win')">🪟 Windows</div>
  </div>
  <div id="r-mac" class="os-content active">
    <div class="two">
      <div>
        <p style="font-size:13px;color:#6b7280;margin-bottom:4px;">【最初の1回だけ】</p>
        <div class="code" style="font-size:13px;"><span class="cmd">curl -fsSL https://claude.ai/install.sh | bash</span><span class="cm"> # インストール</span>
<span class="cmd">claude</span>  <span class="cm">→ 起動 →</span> <span class="cmd">/login</span>  <span class="cm"># ログイン</span></div>
        <p style="font-size:13px;color:#6b7280;margin-bottom:4px;margin-top:10px;">【毎回の作業開始】</p>
        <div class="code" style="font-size:13px;"><span class="cmd">cd ~/Desktop</span>  <span class="cm"># フォルダに移動</span>
<span class="cmd">claude</span>        <span class="cm"># 起動</span></div>
        <p style="font-size:13px;color:#6b7280;margin-bottom:4px;margin-top:10px;">【Claude Code内で使うコマンド】</p>
        <div class="code" style="font-size:13px;"><span class="cmd">/help</span>   <span class="cm"># ヘルプ</span>
<span class="cmd">/clear</span>  <span class="cm"># 会話リセット</span>
<span class="cmd">/quit</span>   <span class="cm"># 終了</span></div>
      </div>
      <div>
        <p style="font-size:13px;color:#6b7280;margin-bottom:4px;">【よく使うフォルダ操作】</p>
        <div class="code" style="font-size:13px;"><span class="cmd">pwd</span>           <span class="cm"># 今いる場所を表示</span>
<span class="cmd">ls</span>            <span class="cm"># ファイル一覧を表示</span>
<span class="cmd">mkdir 名前</span>    <span class="cm"># フォルダを作る</span>
<span class="cmd">cd ..</span>         <span class="cm"># 1つ上に戻る</span>
<span class="cmd">cd ~</span>          <span class="cm"># ホームに戻る</span></div>
        <div class="alert info" style="margin-top:10px;font-size:13px;">
          💡 <strong>フォルダ名にスペースが入っている場合</strong>は<br>
          <code style="background:#0c1f3d;padding:1px 6px;border-radius:3px;">cd "My Folder"</code> のように <strong>""</strong> で囲む
        </div>
      </div>
    </div>
  </div>
  <div id="r-win" class="os-content">
    <div class="two">
      <div>
        <p style="font-size:13px;color:#6b7280;margin-bottom:4px;">【最初の1回だけ】</p>
        <div class="code" style="font-size:13px;"><span class="cmd">irm https://claude.ai/install.ps1 | iex</span><span class="cm"> # インストール</span>
<span class="cmd">claude</span>  <span class="cm">→ 起動 →</span> <span class="cmd">/login</span>  <span class="cm"># ログイン</span></div>
        <p style="font-size:13px;color:#6b7280;margin-bottom:4px;margin-top:10px;">【毎回の作業開始】</p>
        <div class="code" style="font-size:13px;"><span class="cmd">cd $HOME\Desktop</span>  <span class="cm"># フォルダに移動</span>
<span class="cmd">claude</span>            <span class="cm"># 起動</span></div>
        <p style="font-size:13px;color:#6b7280;margin-bottom:4px;margin-top:10px;">【Claude Code内で使うコマンド】</p>
        <div class="code" style="font-size:13px;"><span class="cmd">/help</span>   <span class="cm"># ヘルプ</span>
<span class="cmd">/clear</span>  <span class="cm"># 会話リセット</span>
<span class="cmd">/quit</span>   <span class="cm"># 終了</span></div>
      </div>
      <div>
        <p style="font-size:13px;color:#6b7280;margin-bottom:4px;">【よく使うフォルダ操作】</p>
        <div class="code" style="font-size:13px;"><span class="cmd">pwd</span>           <span class="cm"># 今いる場所を表示</span>
<span class="cmd">ls</span>            <span class="cm"># ファイル一覧（dir でも可）</span>
<span class="cmd">mkdir 名前</span>    <span class="cm"># フォルダを作る</span>
<span class="cmd">cd ..</span>         <span class="cm"># 1つ上に戻る</span>
<span class="cmd">cd $HOME</span>      <span class="cm"># ホームに戻る</span></div>
        <div class="alert warn" style="margin-top:10px;font-size:13px;">
          ⚠️ <strong>パスにスペースが入っている場合</strong>は<br>
          <code style="background:#2d1b00;padding:1px 6px;border-radius:3px;">cd "C:\My Folder"</code> のように <strong>""</strong> で囲む
        </div>
      </div>
    </div>
  </div>
</div>

<!-- 12: トラブル対処 -->
<div class="slide s-trouble top">
  <h2>🛠️ こんなときどうする？</h2>
  <div style="display:flex;flex-direction:column;gap:10px;">
    <div class="card">
      <h3><span class="red">❌</span> 「command not found: claude」と出る</h3>
      <p style="font-size:14px;margin-bottom:6px;">Claude Code がインストールされていません。スライド6のインストールコマンドを実行してください。</p>
    </div>
    <div class="card">
      <h3><span class="red">❌</span> 「claude」と入力しても反応しない / 固まった</h3>
      <p style="font-size:14px;"><kbd>Ctrl</kbd>+<kbd>C</kbd> を押してキャンセル → ターミナルを閉じて開き直す → 再度 <code style="background:#1e1e2e;padding:1px 5px;border-radius:3px;">claude</code> と入力</p>
    </div>
    <div class="card">
      <h3><span class="red">❌</span> ログインできない（ブラウザが開かない）</h3>
      <p style="font-size:14px;">ターミナルに表示される <strong>URLをコピー</strong> してブラウザのアドレスバーに貼り付ける</p>
    </div>
    <div class="card">
      <h3><span class="red">❌</span> Windows「UnauthorizedAccess」と出る</h3>
      <div class="code" style="font-size:13px;margin-top:6px;"><span class="cmd">Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser</span></div>
      <p style="font-size:13px;margin-top:4px;"><code style="background:#1e1e2e;padding:1px 6px;border-radius:3px;">Y</code> を入力 → Enter → もう一度インストールを試す</p>
    </div>
    <div class="card">
      <h3><span class="red">❌</span> Mac「Permission denied」と出る</h3>
      <div class="code" style="font-size:13px;margin-top:6px;"><span class="cmd">sudo curl -fsSL https://claude.ai/install.sh | bash</span></div>
      <p style="font-size:13px;margin-top:4px;">パスワードを求められたら Mac のログインパスワードを入力（画面には表示されないが入力されている）</p>
    </div>
  </div>
</div>

<!-- 13: クイックリファレンス -->
<div class="slide s-ref top">
  <h2>📋 まとめ・クイックリファレンス</h2>
  <div class="cards col2" style="margin-bottom:12px;">
    <div class="card" style="border-color:#a78bfa;">
      <h3 style="color:#c4b5fd;">🍎 Macユーザー</h3>
      <table style="margin-top:8px;">
        <tr><td style="font-size:12px;color:#6b7280;">ターミナルを開く</td><td style="font-size:12px;"><kbd>⌘</kbd>+<kbd>スペース</kbd>→「ターミナル」</td></tr>
        <tr><td style="font-size:12px;color:#6b7280;">インストール（初回）</td><td style="font-size:12px;"><code>curl -fsSL https://claude.ai/install.sh | bash</code></td></tr>
        <tr><td style="font-size:12px;color:#6b7280;">ログイン（初回）</td><td style="font-size:12px;"><code>claude</code> → <code>/login</code></td></tr>
        <tr><td style="font-size:12px;color:#6b7280;">毎回の起動</td><td style="font-size:12px;"><code>cd ~/Desktop</code> → <code>claude</code></td></tr>
        <tr><td style="font-size:12px;color:#6b7280;">終了</td><td style="font-size:12px;"><code>/quit</code></td></tr>
        <tr><td style="font-size:12px;color:#6b7280;">貼り付け</td><td style="font-size:12px;"><kbd>⌘</kbd>+<kbd>V</kbd></td></tr>
      </table>
    </div>
    <div class="card" style="border-color:#60a5fa;">
      <h3 style="color:#93c5fd;">🪟 Windowsユーザー</h3>
      <table style="margin-top:8px;">
        <tr><td style="font-size:12px;color:#6b7280;">PowerShellを開く</td><td style="font-size:12px;"><kbd>⊞</kbd>→「powershell」→Enter</td></tr>
        <tr><td style="font-size:12px;color:#6b7280;">インストール（初回）</td><td style="font-size:12px;"><code>irm https://claude.ai/install.ps1 | iex</code></td></tr>
        <tr><td style="font-size:12px;color:#6b7280;">ログイン（初回）</td><td style="font-size:12px;"><code>claude</code> → <code>/login</code></td></tr>
        <tr><td style="font-size:12px;color:#6b7280;">毎回の起動</td><td style="font-size:12px;"><code>cd $HOME\Desktop</code> → <code>claude</code></td></tr>
        <tr><td style="font-size:12px;color:#6b7280;">終了</td><td style="font-size:12px;"><code>/quit</code></td></tr>
        <tr><td style="font-size:12px;color:#6b7280;">貼り付け</td><td style="font-size:12px;">右クリック→貼り付け</td></tr>
      </table>
    </div>
  </div>
  <div class="check-box">
    <div class="check-title">🎉 これで環境構築から使い方まで完了！</div>
    <p style="font-size:14px;color:#6ee7b7;margin-top:6px;">わからないことが出たら Claude Code に<strong>日本語でそのまま聞いてみましょう。</strong></p>
    <div style="display:flex;gap:10px;margin-top:10px;flex-wrap:wrap;">
      <div style="font-size:13px;color:#94a3b8;">📖 公式ドキュメント：<span style="color:#60a5fa;">code.claude.com/docs</span></div>
      <div style="font-size:13px;color:#94a3b8;">🔑 コンソール：<span style="color:#60a5fa;">console.anthropic.com</span></div>
    </div>
  </div>
</div>

</div><!-- /slideshow -->

<div class="nav">
  <button class="nb" id="pb" onclick="go(-1)">← 前へ</button>
  <span class="sc"><span id="cs">1</span> / <span id="ts">13</span></span>
  <button class="nb" id="nb" onclick="go(1)">次へ →</button>
</div>

<script>
let cur = 0;
const slides = document.querySelectorAll('.slide');
const tot = slides.length;
document.getElementById('ts').textContent = tot;

function show(n) {
  slides[cur].classList.remove('active');
  cur = ((n % tot) + tot) % tot;
  const s = slides[cur];
  s.classList.add('active');
  s.scrollTop = 0;
  document.getElementById('cs').textContent = cur + 1;
  document.getElementById('pb').disabled = cur === 0;
  document.getElementById('nb').disabled = cur === tot - 1;
  document.getElementById('pf').style.width = ((cur + 1) / tot * 100) + '%';
}
function go(d) { show(cur + d); }
document.addEventListener('keydown', e => {
  if (e.key==='ArrowRight'||e.key==='ArrowDown') go(1);
  if (e.key==='ArrowLeft' ||e.key==='ArrowUp')   go(-1);
});
function sw(g, os) {
  document.querySelectorAll('#tab-'+g+' .os-tab').forEach(t=>t.classList.remove('active'));
  const at = document.querySelector('#tab-'+g+' .os-tab.'+os);
  if(at) at.classList.add('active');
  document.querySelectorAll('[id^="'+g+'-"]').forEach(c=>c.classList.remove('active'));
  const tg = document.getElementById(g+'-'+os);
  if(tg) tg.classList.add('active');
}
function cp(text, btn) {
  navigator.clipboard.writeText(text).then(()=>{
    const o = btn.textContent;
    btn.textContent='コピーしました！'; btn.classList.add('ok');
    setTimeout(()=>{ btn.textContent=o; btn.classList.remove('ok'); }, 2000);
  }).catch(()=>{ btn.textContent='コピー失敗'; setTimeout(()=>btn.textContent='コピー',2000); });
}
show(0);
</script>
</body>
</html>
