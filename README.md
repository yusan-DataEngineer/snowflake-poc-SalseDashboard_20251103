# snowflake-poc-SalseDashboard_20251103

🏢 想定企業：中堅小売業の「販売ダッシュボード構築PoC」
🎯 目的
経営層や店舗責任者が「日別・商品別・顧客属性別売上」を即時に可視化できるダッシュボードをSnowflake＋BIツールで構築。
データ量は1万行規模（サンプル）で十分。構造理解・分析パイプライン設計を重視。

◾️全体構成

[S3 or local CSV]
↓  COPY INTO
[Snowflake RAW層]
↓  SQL Transform（ELT）
[Snowflake MART層: Star Schema]
↓  Direct Query
