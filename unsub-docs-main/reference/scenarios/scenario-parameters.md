# Scenario Parameters

Unsub provides a number of Parameters to let you customize a Scenario to your institution's environment and to experiment with different assumptions about the future.
Unsubは、所属機関の環境に合わせてシナリオをカスタマイズし、将来について様々な仮定を試すことができるよう、多くのパラメータを提供しています。

Parameter values are stored as part of the scenario. Parameter values can be changed using the "Parameters" menu. You can make a new scenario that has the same parameter settings as a current scenario using Copy button to the right of the scenario title on a scenario page:
パラメータの値は、シナリオの一部として保存されます。パラメータ値は、"Parameters"（パラメータ）メニューから変更することが出来ます。シナリオページにて、シナリオタイトルの右側にあるコピーボタンを使って、現在のシナリオと同じパラメータ設定を持つ新しいシナリオを作成することが出来ます。

![](../../.gitbook/assets/first-scenario.png)

### &#x20;<a href="#h_68ea9b794f" id="h_68ea9b794f"></a>

### Costs <a href="#h_68ea9b794f" id="h_68ea9b794f"></a>

**Title-by-title 'content fee'**

A content fee charged by publishers if you buy subscriptions title-by-title (literature suggests 5.7% for subscriptions).
(need to check)ジャーナルをタイトル単位で購読する場合に出版社から請求されるコンテンツ料（文献では定期購読の場合は5.7％）。

Default: 5.7%

**Title-by-title subscription cost growth**

The annual percent increase you expect in title-by-title subscription prices (literature suggests 8%).
タイトルごとの購読料金の予想年間上昇率（文献では8％）
Default: 8%

### &#x20;<a href="#h_bb1971fa6a" id="h_bb1971fa6a"></a>

### ILL <a href="#h_bb1971fa6a" id="h_bb1971fa6a"></a>

**ILL transaction cost**

The cost of an ILL request for your institution (literature suggests $17 is average).
所属機関のILLリクエストにかかる費用（文献によると17ドルが平均的とされています）。

Default: $17

**ILL Request Rate**

The percent of turnaways that will result in an ILL request. Our extensive literature review suggests 5% is a conservative estimate. (NB: 'Turnaways' are all usages that aren't fulfilled by Open Access, PTA rights, or title-by-title subscriptions in this scenario.)
ILLリクエストにつながるTurnawayのパーセンテージ。我々の広範な文献調査によると、5%は保守的な見積もりであるとされています。(注：'Turnaway'とは、このシナリオでは、オープンアクセス、PTA権、タイトルごとの購読では満たされないすべての利用を指します)。

Default: 5%

### &#x20;<a href="#h_d192405b0b" id="h_d192405b0b"></a>

### Fulfillment Sources <a href="#h_d192405b0b" id="h_d192405b0b"></a>

**Include Bronze OA**

Include Bronze OA as a type of fulfillment. Bronze OA is when a paper is made freely available on a publisher site without an open license (includes Elsevier's "open archive" journals).
フルフィルメント(実現可能性)の一種として、ブロンズOAを含める。Bronze OAとは、オープンライセンスなしで出版社のサイトで自由に論文を利用できるようにしたものです（Elsevier社の"open archive" ジャーナルも含まれます）。

Default: True

**Permit non-peer-reviewed versions**

For Green OA, allow submitted versions as a type of fulfillment. Submitted versions are papers made available in repositories as preprints or other versions that have not yet been peer reviewed.
グリーンOAの場合、著者最終稿をfulfillment(実現可能性)の一種として許可する。投稿版(著者最終稿）とは、プレプリントなどとしてリポジトリに公開されている論文のうち、まだ査読を受けていないものを指します。

Default: True

**Include ResearchGate-hosted content**

Include ResearchGate and other Academic Social Networks as a fulfillment source.
フルフィルメント（実現可能性)ソースとしてResearchGateやその他のアカデミック・ソーシャルネットワークを含める。

Default: True

### &#x20;Citation and Authorship

**Institutional citation weight(機関の引用での利用の重み付け）**

A citation from someone in your institution contributes this many download-equivalent points to the Usage of the journal. A common value is 10 -- in this case a citation from your institution to this journal is modeled as the equivalent of 10 downloads of this journal.
所属機関の研究者からのジャーナルの引用は、そのジャーナルの使用率に特定のダウンロード相当のポイントを付与します。一般的な値は10です。この場合、所属機関からこのジャーナルへの引用は、このジャーナルの10回分のダウンロードに相当するものとしてモデル化されます。

Default: 10

**Institutional authorship weight(機関での著者の重み付け)**

A paper authored by someone in your institution contributes this many download-equivalent points to the Usage of the journal. A common value is 100 -- in this case an authored paper in this journal is modeled as the equivalent of 100 downloads of this journal.
所属機関の研究者が執筆した論文は、そのジャーナルの使用率に特定のダウンロード相当ポイントを付与する。一般的な値は100です。この場合、このジャーナルの著者による論文は、このジャーナルの100回のダウンロードに相当するものとしてモデル化されます。

Default: 100

\
