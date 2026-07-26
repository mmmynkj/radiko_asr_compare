Parakeet ASR 比較: exact(ビタ切り) vs silence2(2秒無音前置)
対象: annotation_target_20260725 の33番組 / 全15,648発話

- <target_id>__<番組名>.csv : 番組ごと。発話(segment_id)を1行に、両条件のASRテキストを横並び。
- _ALL_targets_combined.csv  : 全番組結合
- _index.csv                 : 番組別の発話数・一致/相違数

列: segment_id, speaker, start_sec, end_sec, duration_sec(元音声絶対時刻),
    parakeet_exact_text, parakeet_silence2_text, texts_match, char_diff 等
文字コード: UTF-8 (BOM付き, Excelでそのまま開けます)
モデル: nvidia/parakeet-tdt_ctc-0.6b-ja (tdt), 16kHz, 入力=音楽マスク後音源
