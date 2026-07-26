Parakeet ASR 比較: exact(ビタ切り) vs context2(2秒前方延長)
対象: annotation_target_20260725 の33番組 / 全15,648発話

context2 = 発話開始位置を元音声上で2.0秒だけ前方(過去方向)へ延長した入力に対するASR。
発話境界(start_sec/end_sec)は元音声基準の絶対時刻で、条件間で不変。

- <target_id>__<番組名>.csv : 番組ごと。発話(segment_id)を1行に、両条件のASRテキストを横並び。
- _ALL_targets_combined.csv  : 全番組結合
- _index.csv                 : 番組別の発話数・一致/相違数

列: segment_id, speaker, start_sec, end_sec, duration_sec,
    parakeet_exact_text, parakeet_context2_text, texts_match, char_diff 等
文字コード: UTF-8 (BOM付き, Excelでそのまま開けます)
モデル: nvidia/parakeet-tdt_ctc-0.6b-ja (tdt), 16kHz, 入力=音楽マスク後音源
