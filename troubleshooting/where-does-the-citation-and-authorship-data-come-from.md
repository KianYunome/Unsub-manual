# where does the citation and authorship data come from

## Where does the citation and authorship data come from?

## 引用と著者のデータはどこから来ているのですか？

Citation and authorship data come from [OpenAlex](https://openalex.org/). 引用と著者のデータは、[OpenAlex](https://openalex.org/).\&#x20. から来ています。

There are a few different sources of this kind of data. OpenAlex is superior to the alternatives, and here's why. We think coverage is the most important factor when considering the Unsub use case. According to Harzing (2016) Coverage of MAG (and therefore OpenAlex as it's built on MAG) is better than WoS and at least as good as Scopus. Visser et al. (2020) found that MAG had the highest overall coverage of the set: MAG, WoS, Scopus, Dimensions and Crossref. この種のデータのソースはいくつかあります。この種のデータソースはいくつかありますが、OpenAlexは他のものより優れており、その理由は次のとおりです。Unsubの利用ケースを考える上で、収録範囲は最も重要なファクターだと考えています。Harzing (2016)によれば、MAG(Microsoft Academic Graph)の収録範囲（したがって、OpenAlexはMAGに基づいて構築されているため）はWoS(Web of Science)よりも優れており、少なくともScopusと同程度のものです。Visserら(2020)は、MAGがMAG、WoS、Scopus、Dimensions、Crossref. の中でセット全体の収録範囲が最も高いことを発見しました。

References:

Harzing, A.-W. (2016). Microsoft Academic (Search): a Phoenix arisen from the ashes? Scientometrics, 108(3), 1637–1647. [https://doi.org/10.1007/s11192-016-2026-y](https://doi.org/10.1007/s11192-016-2026-y)

Visser, M., van Eck, N. J., & Waltman, L. (2020). _Large_-_scale comparison of bibliographic data sources: Scopus, Web of Science, Dimensions, Crossref, and Microsoft Academic_. [https://doi.org/10.48550/arXiv.2005.10732](https://doi.org/10.48550/arXiv.2005.10732)

#### What years are included in calculating the citations and authorships data in the single journal view popup?

#### シングルジャーナル表示ポップアップの被引用数と著者数の計算には，何年分のデータが含まれますか？

As of right now (August 2022) the years we are pulling from to get citations and authorships data are: 2014-2022 現在（2022年8月）、被引用数と著者数のデータを取得するためにOpenAlexから収集している年は 2014-2022となります。

#### How does Unsub model authorships and citations?

#### Unsubはどのように著者名と引用をモデル化しているのですか？

It’s a linear extrapolation of current data. That is, if there’s 10 authorships in the Journal of Current Chemistry in the last year of data we have, then each future year we’d forecast 10 authorships. Citations works the same way. 現在のデータから直線的に推測します。つまり、Journal of Current Chemistryに10件のオーサーシップがあれば、将来も毎年10件のオーサーシップがあると予測するのです。Citationsも同じように予測します。

#### How often is authorship and citation data updated?

#### 著者名と引用回数のデータはどれくらいの頻度で更新されますか？

We'll have more details here soon regarding update frequency. 更新頻度については、近日中にこちらで詳細をお知らせします。
