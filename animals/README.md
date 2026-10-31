# どうぶつカード（記憶エンジン版）

- 公開リンク（GitHub Pages・マイク対応）: https://joshi898-gif.github.io/eigo-cards/animals/
- 公開リンク（claude.ai・マイクなし）: https://claude.ai/artifact/B58XMbHe458mo4nRK2XGQA
- GitHub リポジトリ: https://github.com/Joshi898-gif/eigo-cards （ローカル作業用コピー: C:/Users/Owner/github-eigo-cards）
- このフォルダの中身: index.html（アプリ本体）、img/（写真100枚）、audio/（音声300本）、credits.json（写真の出典）

## マイクについて
claude.ai のリンクで開くと、ブラウザの仕組み上マイクが使えません。
その場合アプリは「声に出して言う → お手本を聞く → おなじに いえた／ちがった を自分で選ぶ」方式に自動で切り替わります。

マイク判定と録音の聞き比べを使いたいときは、このフォルダ（index.html・img・audio・credits.json）をそのまま
GitHub Pages や Netlify などの無料の静的サイトに置くと、Chrome・Edge・Safari でマイクが使えます。

## 学習の仕組み
- 新しい語は同じ日に3回思い出す（出会う → 言う → 聞いて選ぶ）
- 復習は 1日 → 3日 → 7日 → 14日 → 30日 → 60日 → 120日 と間隔を広げる
- 間違えたら間隔を1段階戻して翌日に出す。答える速さで間隔を自動調整
- 覚えが進むほど 4択 → 絵を見て言う → 文で言う に切り替える
- 1日の新しい語は設定で 2〜8語（初期値5）。復習が20枚たまると新出は止まる
