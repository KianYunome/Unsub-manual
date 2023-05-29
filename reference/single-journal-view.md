# Single Journal View

In histogram or table view in an Unsub scenario you can click on any journal to get to the single journal view. Unsubシナリオのヒストグラムまたはテーブルビューで、任意のジャーナルをクリックすると、single journal view(単一ジャーナルビュー)に移動します。

For example, if we click on the box for the journal **Chest** 例えば、ジャーナル **Chest** のボックスをクリックすると

we then get a zoom view of that journal: そして、そのジャーナルを拡大表示します。

This zoomed view of a single journal contains journal metadata and a breakdown of the Cost Per Use calculations. この単一ジャーナルの拡大表示には、ジャーナルのメタデータとCost Per Useの計算の内訳が含まれています

On this single journal zoom you can subscribe or unsubscribe if you're already subscribed to the journal. このSingle journal zoom(シングルジャーナル拡大表示)では、購読の申し込みや、すでに購読している場合は購読の解除ができます。

### Overview

The overview tab contains journal metadata, annual usage, annual cost, and the CPU value. Overview Tab(概要タブ)には、ジャーナルのメタデータ、年間利用量、年間コスト、CPU値が表示されます。

#### Journal metadata

This section of the single journal view contains: single journal view(シングルジャーナルビュー)のこのセクションには、 以下が含まれています。

* Subject: a single subject from OpenAlex concepts - see Data export for more information.(OpenAlexのコンセプトに基づく単一のsubject(主題) - 詳細はData exportを参照。)
* ISSN: the Linking ISSN (or ISSN-L)(リンクISSN(またはISSN-L))
* Society Journal: Whether the journal is a society journal ("Yes") or not ("No"). (Society Journal (学会誌):Society Journal: そのジャーナルが学会誌かどうか（"Yes"）、またはそうでないか（"No"）)
* Delayed OA: Whether the journal a delayed OA journal ("Yes") or not ("No"). If "Yes", then the journal makes content free to read after an embargo period has passed - and there will be an additional row below "OA embargo length" that gives the length in months.(Delayed OA(遅延OA): 遅延型OAジャーナルかどうか（"Yes"）、または（"No"）。"Yes"の場合、そのジャーナルはエンバーゴ期間が過ぎるとコンテンツを自由に読むことができるようになり、「OAエンバーゴ期間」の下に、その期間を月単位で示す行が追加される。)
* PTA (Post-Termination Access) rights: This is empty if you have not uploaded PTA rights for the journal, and gives the start and end years if you have uploaded PTA rights for the journal.(PTA (Post-Termination Access)の権利。PTA権をアップロードしていない場合は空欄、PTA権をアップロードしている場合は開始と終了の年数が表示されます。)

{% hint style="danger" %}
Numbers are rounded! If you try to do the math yourself you may end up with slightly different results - which should always be due to rounding. If you're still not sure, get in touch at [support@unsub.org](mailto:support@unsub.org) 数値は四捨五入されています。ご自身で計算される場合、若干異なる結果になることがありますが、これは常に四捨五入によるものとなります。それでもご不明な点は、[support@unsub.org](mailto:support@unsub.org)までご連絡ください。
{% endhint %}

{% hint style="info" %}
Numbers are forecasted numbers. They will not match current day numbers you may have. 数値は予測値です。現在お持ちの数値とは一致しません。
{% endhint %}

#### Annual usage

**Weighted overall uses** is three components combined:(**Weighted overall uses**は、3つのコンポーネントを組み合わせたものです。)

* Downloads: forecasted downloads (or usage) derived from the COUNTER reports you uploaded.(ダウンロード数：アップロードしたCOUNTERレポートから得られるダウンロード数（または利用数）の予測値。)
* Citations: forecasted citations to the journal from any published paper (in any journal, including this one) by members of your institution.(引用数：所属機関の研究者が発表した論文からの引用数予測（本誌を含む全ジャーナル）)
* Authorships: forecasted authorships in the journal by members of your institution.(著者数：所属機関の研究者による本誌の著者数予測。)

Then we want to get to **Paywalled uses** because we don't want to factor free usage into our CPU calculation. To arrive at **Paywalled uses** we subtract from **Weighted overall uses**: 次に、CPUの計算に無料でアクセス可能な利用を省くため、**Paywalled uses**を求めることにします。Paywalled uses\*\* を求めるには、**Weighted overall uses** から差し引きます。

* Open access usage: forecasted open access usage(オープンアクセス利用：オープンアクセス利用の予測値)
* PTA/Backfile usage: forecasted usage via PTA/backfile(PTA/バックファイル利用：PTA/バックファイル経由の利用予測)

#### Annual cost

Cost is not just the base subscription cost as you might be used to. We want to account for the cost of ILL because the opposite of subscribing is not free. There is a cost to ILL. コストとは、皆さんが慣れ親しんでいるような基本的な購読料だけではありません。購読の反対は無料ではないので、ILLにかかる費用を計上します。ILLにはコストがかかります。

To get to **Net subscription cost** we subtract forecasted ILL cost from base subscription cost. **Net購読コスト**を得るために、基本的な購読コストからILLコスト予測を差し引きます。

#### Cost Per Use

CPU is the **Net subscription cost** divided by **Paywalled uses**. CPUは、**Net subscription cost** を**Paywalled uses** で割ったものです。

### Timelines

The Timelines tab has a number of sections: タイムラインのタブには、いくつかのセクションがあります。

* Fulfillment: breakdown of different fulfillment types by year.(Fulfillment（実現可能性)：年別のフルフィルメントタイプの内訳)
* Open Access: OA fulfillment by type across all years.(オープンアクセス: 全年度における OA の種類別の実現可能性)
* Impact: Downloads, citations, and authorships contribution to usage.(インパクト：ダウンロード数、引用数、著者数の利用への貢献度)
* Subscription cost: subscription details by year.(購読料：年別の購読料の詳細)
* API response: [JSON](https://en.wikipedia.org/wiki/JSON) formatted response for the technical folks.(APIレスポンス:技術者向けの[JSON](https://en.wikipedia.org/wiki/JSON)形式のレスポンス)
