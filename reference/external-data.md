# External data

The following is a list of the external data sources used, including what they are used for, and how often the data is updated. 使用する外部データソースについて、その使用目的、データの更新頻度などを以下に示す。

### Citations

Data source(データソース): [OpenAlex](https://docs.openalex.org/)

Update frequency（更新頻度）: Quarterly (4x per year)　４半期毎、年４回

Used in Unsub: Journal level Cost Per Use calculation (if you include citations in your scenario parameters). Citations data shown in single journal view or in the table view in a scenario. Institutional level APC Report. Unsubでの使用: ジャーナルレベルの Cost Per Use の計算 (引用を scenario parameters に含む場合). single journal viewまたはシナリオのテーブルビューに表示される引用データ。機関レベルのAPC Report。

### Authorships

Data source(データソース): [OpenAlex](https://docs.openalex.org/)

Update frequency(更新頻度): Quarterly (4x per year)　４半期毎、年４回

Used in Unsub: Journal level Cost Per Use calculation (if you include authorships in your scenario parameters). Authorships data shown in single journal view or in the table view in a scenario. Institutional level APC Report. Unsubでの使用。ジャーナルレベルのCost Per Use の計算（senario parameters にオーサーシップを含む場合）。single journal viewまたはシナリオのテーブルビューに表示される著者数データ。機関レベルの APC Report.

### Journal metadata

This includes journal title, ISSNs, publisher, open access status, and whether title is currently publishing (based on date of last DOI published). これには、ジャーナルのタイトル、ISSN、出版社、オープンアクセスの状況、タイトルが現在出版されているかどうか（最後にDOIが発行された日付に基づく）が含まれます。

Data source(データソース): [OpenAlex](https://docs.openalex.org/)

Update frequency(更新頻度): Daily(毎日)

Used in Unsub: Determine whether a journal should be included in Unsub dashboards or not (see Why don't I see a certain title in my dashboard?), and as the source of truth to link together journals, user uploaded data, and any external journal level data. Unsubでの使用：ジャーナルを Unsub ダッシュボードに含めるかどうかを決定し（\[Why don't I see a certain title-in-my-dashboard.md]\(../troubleshooting/why-dont-i-see a certain-title-in-my-dashboard.md) 参照）、ジャーナル、ユーザーアップロードデータ、外部ジャーナルレベルのデータを結びつけるためのソースとして使用します。

### Journal embargo periods

Data source(データソース): Manually collected. We will soon switch over to using data from [oa.works](https://oa.works/)　(手作業で収集。近日中に[oa.works](https://oa.works/)のデータの利用に切り替わる予定です。)

Update frequency(更新頻度): Not currently updated (現在更新していません)

Used in Unsub: Shown in single journal view in Unsub dashboards, and used in calculating Cost Per Use Unsubでの使用：Unsubダッシュボードのsingle journal viewに表示され、Cost Per Use の計算に使用される。

### Publisher societies

Data source(データソース): Manually collected.（手作業での収集）

Update frequency(更新頻度): Not currently updated(現在更新していません)

Used in Unsub: Shown in single journal view in Unsub dashboards Unsubでの使用：Unsubダッシュボードのsingle journal view に表示される。

### Number of papers

Data source(データソース): [OpenAlex](https://docs.openalex.org/)

Update frequency(更新頻度): Daily(毎日)

Used in Unsub: Journal level usage forecast. Unsubでの使用: ジャーナルレベルの利用量予測。

### ROR and Grid identifiers

Data source(データソース): Microsoft Academic Graph

Update frequency(更新頻度): Not currently updated; we'll switch to OpenAlex in the near future.(現在は更新されていません。近い将来、OpenAlexに切り替わる予定です。)

Used in Unsub: Used to link together many kinds of data (journals, authors, etc.) to institutions. Unsubでの使用：多くの種類のデータ（ジャーナル、著者など）をまとめて機関にリンクするために使用します。

### APC prices

Data source(データソース): We get these from publisher websites(出版社サイト).

Update frequency(更新頻度): Not updated(更新されていません)

Used in Unsub: For the institutional APC Report for the big five publishers (Elsevier, Wiley, Springer Nature, Taylor & Francis, SAGE) only. Unsubでの使用: 大手出版社5社（Elsevier, Wiley, Springer Nature, Taylor & Francis, SAGE）のみの機関版APC Report用です。

### Unpaywall

Data source(データソース): [Unpaywall](https://unpaywall.org/)

Update frequency(更新頻度): Every 6 hours (4x/day)(6時間毎、1日４回)

Used in Unsub: Used to determine usage patterns at a journal title level. Also used in creating citation and authorship data (see above for how citation and authorship data are used). Unsubでの使用：ジャーナルタイトルレベルでの利用パターンを把握するために使用します。引用・著者名データの作成にも使用（引用・著者名データの使用方法は上記を参照）。

### Unpaywall Browser Extension

Data source(データソース): [Unpaywall](https://unpaywall.org/) Browser Extension data; aggregated statistics about journal-level year of publication usage derived from usage of people with the Unpaywall browser extension installed(ブラウザ拡張機能オプション・データ：Unpaywallブラウザ拡張機能をインストールした人の利用状況から、ジャーナルレベルの出版年の利用状況を集計した統計データ)

Update frequency(更新頻度): Updated October 2022. Likely update frequency: annual(2022年10月に更新、毎年更新予定)

Used in Unsub: Used to determine usage patterns at a journal title level. Unsubでの使用：ジャーナルタイトルレベルでの利用パターンを把握するために使用します。
