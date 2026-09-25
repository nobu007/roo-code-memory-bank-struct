# GoalDev Log

永続的決定と完了記録を追記する。各エントリに日付と検証を必ず付ける
（原則: contracts `llm-wiki-discipline` の log-is-append-with-correction）。

## 2026-09-26 — llm-wiki スキャフォールド

contracts の llm-wiki-discipline 原則に基づき `docs/llm-wiki/` を新設した。

- **Verification**: 原則 `registry/principles/llm-wiki-discipline.yaml`（contracts リポ commit 3ab5768）。

## 2026-09-26 — fork カスタマイズ調査（upstream GreatScottyMac/roo-code-memory-bank）

upstream リモートは登録済みだが refs/remotes/upstream/* が 1 件も存在せず、fetch 禁止の制約内では上流とのコミット差分を確定できない（比較不能）。ローカル main の履歴からは .clinerules→.roorules 改名、config/install.sh・install.cmd の追加、install.sh の URL 修正、AUTOMATION.md・llm-wiki の整備が確認できる。上流との差分確定は今後の fetch 後に回す。

- **Verification**: git for-each-ref refs/remotes/upstream = 0 件、git log -10 でローカル改変コミットを確認（fetch 不実施）。
