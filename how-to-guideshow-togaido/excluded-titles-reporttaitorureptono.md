# Excluded Titles report(タイトルレポートの除外)

Your Unsub dashboard may not include all the titles you uploaded in your COUNTER reports files. See our Why don't I see a certain title in my dashboard? page, which details the four major reasons why a title could be excluded.(Unsubダッシュボードには、COUNTERレポートファイルにアップロードしたすべてのタイトルが含まれていない可能性があります。タイトルが除外される4つの主な理由については、Why don't I see a certain title in my dashboard?(ダッシュボードに特定のタイトルが表示されないのはなぜですか?) ページで詳しく説明しています。)

In your package Setup tab, under the **Diagnostic data** section, you will find an Excluded Titles page which allows you to download a spreadsheet.(パッケージのSetupタブの**Diagnostic data**セクションに、Excluded Titlesのページがあり、スプレッドシートをダウンロードすることができます。)

In the spreadsheet there are two informational columns (issn\_l, publisher), and four columns for the four reasons a title could be excluded from a scenario. The columns are:(スプレッドシートには、2つの情報カラム（issn\_l, publisher）と、タイトルがシナリオから除外される4つの理由のカラムがあります。列は以下のとおりです。)

* **issn\_l**: The linking ISSN, or ISSN-L
* **publisher**: The publisher, according to [OpenAlex](https://openalex.org/)(**publisher**:[OpenAlex](https://openalex.org/)で登録されているThe publisher(出版社名))
* **gold\_oa**: `True` if OpenAlex thinks the journal is Gold Open Access (OA), otherwise `False`. We can not include titles that are Gold OA because there is no subscription access route, and we currently require that(**gold\_oa**:OpenAlexがそのジャーナルをゴールド・オープンアクセス（OA）であると判断した場合は `True` 、そうでない場合は `False` となります。購読アクセスルートがないため、ゴールドOAであるタイトルを含めることはできませんが、現在、以下の条件を満たしている必要があります。)
* **not\_currently\_publishing**: `True` if we think the journal is no longer publishing, otherwise `False`. This determination is based on data from OpenAlex(**not\_Currently\_publishing**: そのジャーナルがもう出版されていないと思われる場合は `True` 、そうでない場合は `False` です。この判断はOpenAlexのデータに基づいています。)
* **price\_not\_available**: `True` if there is not title price, otherwise `False`. You can fix this by uploading title prices. We require title prices for a title to be included in the dashboard(**price\_not\_available**: タイトル価格がない場合は `True` 、そうでない場合は `False` です。タイトル価格のアップロード]\(upload-title-prices.md)で修正可能です。ダッシュボードに含まれるタイトルには、タイトル価格が必要となります。)
* **filtered\_out**: `True` if you filtered the title out using the optional Journal Filter setup step, otherwise `False`. Read the docs for journal filter(**filtered\_out**: Journal Filter setup stepでタイトルをフィルタリングした場合は `True` 、そうでない場合は `False` です。journal filter(ジャーナルフィルター)のドキュメントをご確認ください。)

Here's an example of four rows of the report you'll download:(以下は、ダウンロードするレポートの4行の例です。)

| issn\_l   | publisher | gold\_oa | not\_currently\_publishing | price\_not\_available | filtered\_out |
| --------- | --------- | -------- | -------------------------- | --------------------- | ------------- |
| 2053-9711 | OUP       | True     | False                      | False                 | False         |
| 0007-0912 | Elsevier  | False    | False                      | True                  | False         |
| 1473-6691 | SAGE      | False    | False                      | True                  | False         |
| 0024-6093 | Wiley     | False    | True                       | False                 | False         |

A few notes about the data:(データに関するいくつかの注意事項)

* With the four columns in the report, you can use a spreadsheet filter tool to filter to all the titles that are excluded for the same reason (e.g. missing title prices), and then look into those titles.(レポート内の4つの列で、スプレッドシートのフィルターツールを使用して、同じ理由で除外されたすべてのタイトル（例：タイトル価格がない等）にフィルタリングし、それらのタイトルを調べることができます)
* A title can be excluded for more than one reason. For example, it can be Gold OA and missing a title price.(1つのタイトルが複数の理由で除外されることがあります。例えば、ゴールドOAでありながら、タイトル価格がないこともあります。)
* For some titles you can change something so it appears in your dashboard. For example, if a title price is missing you can get a title price; if you've filtered the title out you can remove the title from your filtered titles upload. However, if the title is Gold OA or is no longer publishing, nothing can be done to make it appear in your dashboard.(いくつかのタイトルでは、ダッシュボードに表示されるように何かを変更することができます。例えば、タイトル価格がない場合、タイトル価格を取得することができます。タイトルを除外した場合、フィルタリングタイトルのアップロードからそのタイトルを削除することができます。しかし、タイトルがゴールド OAであったり、もう出版されていない場合は、ダッシュボードに表示させるためにできることは何もありません。)
* Check out the [OpenAlex documentation](https://docs.openalex.org/) for more about OpenAlex.([OpenAlex documentation(OpenAlexの詳細については)](https://docs.openalex.org/)を参照してください。)

After looking at the report [email us (support@unsub.org)](mailto:support@unsub.org) if you think any of the titles should be included in your scenarios for this package, and we'll have a look.(レポートをご覧になった上で、このタイトルはこのパッケージのシナリオに含めるべきと思われるものがあれば、[email us(support@unsub.org)](mailto:support@unsub.org)にメールしてください。)
