# Data export

The data fields in the Download as Spreadsheet are described here: ここでは、表計算ソフトのダウンロードのデータフィールドについて説明します。

### Metadata <a href="#metadata" id="metadata"></a>

**issn\_l\_prefixed**

The primary ISSN we use for this journal (see issn.org [Linking ISSNs](https://www.issn.org/understanding-the-issn/assignment-rules/the-issn-l-for-publications-on-multiple-media/)) prefixed with "issn:" 我々がジャーナルで使用しているプライマリISSN（issn.org [Linking ISSNs](https://www.issn.org/understanding-the-issn/assignment-rules/the-issn-l-for-publications-on-multiple-media/) 参照）には "issn:" というプレフィックスを付けています。

**issn\_l**

The primary ISSN we use for this journal (see issn.org [Linking ISSNs](https://www.issn.org/understanding-the-issn/assignment-rules/the-issn-l-for-publications-on-multiple-media/)) 我々がジャーナルで使用しているプライマリISSN（issn.org [Linking ISSNs](https://www.issn.org/understanding-the-issn/assignment-rules/the-issn-l-for-publications-on-multiple-media/) をご参照ください。）

**title**

The title of this journal. このジャーナルのタイトルです。

**issns**

A JSON array of ISSNs for this journal このジャーナルのISSNを表すJSON配列

**publisher**

The name of the publisher of the journal. "null" if we do not know the name of the publisher. 雑誌の出版社名。出版社名がわからない場合は "null" となります。

{% hint style="info" %}
OpenAlex uses the term "concept" - which is equivalent to "subject" here OpenAlex では "concept" という用語が使われており、ここでは "subject" と同じ意味です。
{% endhint %}

**subject**

A single OpenAlex concept (equivalent to subject in Unsub). The concept is selected by filtering to level zero OpenAlex concepts, then selecting those with the maximum score. If there's more than one concept we then select one alphabetically, starting from "A". You may also want to look at **subject\_top\_three** due to this alphabetical selection. See [OpenAlex docs](https://docs.openalex.org/about-the-data/venue#x\_concepts) for more information. 単一のOpenAlexコンセプト(Unsubのsubjectに相当)。コンセプトは、レベルゼロのOpenAlexコンセプトにフィルタリングし、最大スコアを持つものを選択します。複数のコンセプトがある場合は、"A" から始まるアルファベット順に選択されます。このアルファベット順の選択のために、**subject\_top\_three**も見ておくとよいでしょう。詳しくは、[OpenAlex docs](https://docs.openalex.org/about-the-data/venue#x\_concepts) をご参照ください。

**subject\_top\_three**

The top three OpenAlex concepts. Selected using the top three level zero OpenAlex concepts based on their score for strength of association between the journal and the concept. See [OpenAlex docs](https://docs.openalex.org/about-the-data/venue#x\_concepts) for more information. OpenAlexの上位3つのコンセプト。ジャーナルとコンセプトの関連性の強さのスコアに基づいて、レベルゼロのOpenAlexコンセプトの上位3つを使用して選択されています。詳しくは、[OpenAlex docs](https://docs.openalex.org/about-the-data/venue#x\_concepts) をご覧ください。

**subjects\_all**

All level zero OpenAlex concepts and their IDs in a JSON array. With the IDs one can look up more information on each concept by appending the ID to `https://openalex.org` (e.g., [https://openalex.org/C185592680](https://openalex.org/C185592680)). See [OpenAlex docs](https://docs.openalex.org/about-the-data/venue#x\_concepts) for more information. OpenAlexのレベル0の全概念とそのIDをJSON配列にしたもの。IDがあれば、`https://openalex.org`にIDを追加することで、各概念の詳細情報を調べることができます（例：[https://openalex.org/C185592680](https://openalex.org/C185592680))。詳しくは[OpenAlex docs](https://docs.openalex.org/about-the-data/venue#x\_concepts) を参照してください。

### Summary <a href="#summary" id="summary"></a>

**subscribed**

`True` if you currently have the journal modeled as "subscribed" in your scenario, `False` if the journal is currently "unsubscribed" シナリオでジャーナルを "subscribed(購読中) "としてモデル化している場合は `True` 、ジャーナルが "unsubscribed(購読停止) "の場合は `False` となります。

**is\_society\_journal**

`True` if the journal is a society journal; `False` if not. 学会誌の場合は `True` 、学会誌でない場合は `False` となります。

**usage**

The projected Usage of the journal by your institution. Usage is a measure of the journal's value to your institution. It is calculated as: 自機関が予測したジャーナルの利用状況。利用率は、自機関にとってそのジャーナルがどのような価値を持つかを示す指標です。次のように計算されます。

`Usage of a journal =`

`Downloads from the journal`

`+ (Citations to the journal by your authors) * (citation weight)`

`+ (Authored papers in the journal) * (authorship weight)`

`Usage of a journal(ジャーナルの利用)=`

`Downloads from the journal(該当ジャーナルからのダウンロード数)`

\`+ (Citations to the journal by your authors(所属の著者による該当ジャーナルへの引用数)) \* (citation weight(引用数重み付け))

\`+ (Authored papers in the journal(該当ジャーナルでの所属著者による論文)) \* (authorship weight(著者数重み付け))

**cpu**

This is the Cost per Use (CPU) of the journal. We use a more advanced variant of CPU (internally we call this Net Per Paid Use, or NCPPU). This CPU calculation is the net cost (subscription minus ILL), divided by Paid Use (Usage that can't be met with free sources). This is our most important measure of journal value--it summarizes the real value you're getting for your subscription dollar. This article has more details: [How do we calculate cost-effectiveness (Cost Per Use, CPU)](https://intercom.help/get-unsub/en/articles/4061107-how-do-we-calculate-cost-effectiveness-cost-per-use-cpu) これは、ジャーナルのCost per Use(利用単価)（CPU）です。我々は、より高度なCPUを使用しています（社内では、これをNet Per Paid Use、またはNCPPUと呼んでいます）。このCPU計算は、費用（購読料からILLを差し引いたもの）を有料利用（無料のソースで満たせない利用）で割ったものです。これは、購読料に見合う本当の価値を要約したもので、ジャーナルの価値に関する我々の最も重要な尺度です。詳しくはこちらの記事をご覧ください。[How do we caluculate cost-effectiveness(Cost Per Use, CPU)（費用対効果（Cost Per Use, CPU）の計算方法)](https://intercom.help/get-unsub/en/articles/4061107-how-do-we-calculate-cost-effectiveness-cost-per-use-cpu)

**cpu\_rank**

The journal's rank according to CPU, relative to other journals in this dataset. The most cost-effective journal has a rank of 1.\
このデータセットに含まれる他のジャーナルと比較した，CPUに応じたジャーナルのランク．最も費用対効果の高いジャーナルのランクは1です。\\

**cost**

The cost of this journal according to the Settings and Subscription status of the journals in this Scenario. It will be either Subscription Cost or ILL Cost (see next columns), depending on whether the journal is currently subscribed to or not in this scenario. このシナリオのジャーナルの設定と購読状況に応じた、該当ジャーナルのコストです。このシナリオでジャーナルが現在購読されているかどうかに応じて、購読コストまたはILLコスト（see next columns(次のコラムを参照)）のいずれかになります。

***

**instant\_usage\_percent**

The percent of Usage that is available instantly -- available as Open Access, PTA, or Subscription. 即座に利用可能な利用率の割合 -- オープンアクセス、PTA、購読として利用可能です。

**free\_instant\_usage\_percent**

The percent of Usage that can be fulfilled via Open Access or PTA. This excludes usage met only by ILL or Subscription. オープンアクセスまたはPTAで満たされる利用率のパーセンテージ。ILLまたは購読によってのみ満たされる利用を除く。

\\

### Costs <a href="#costs" id="costs"></a>

### Costs(コスト) <a href="#costs" id="costs"></a>

**subscription\_cost**

The title-by-title subscription cost of this journal. It includes a 'content fee' based on your settings, and annual price increases over the next five years (the cost shown is the average cost over the next five years). This data is based on public price lists unless you've uploaded a custom price list (available in a purchased account). This article has more details: How do we calculate title-by-title subscription costs? ジャーナルのタイトルごとの購読料です。お客様の設定に基づく「コンテンツ料」と、今後5年間の毎年の値上げが含まれています（表示されている費用は、今後5年間の平均費用です）。このデータは、カスタム価格表（購入済みアカウントで利用可能）をアップロードしていない限り、公開価格表に基づいています。詳しくはこちらの記事をご覧ください。How do we calculate title-by-title subscription costs?(タイトルごとの購読料をどのように計算するか?)をご覧ください。

**ill\_cost**

The ILL subscription cost of this journal. It is based on the ILL transaction cost and your ILL Request Rate, both of which are adjustable parameters. This article has more details: How do we calculate ILL requests and ILL cost? このジャーナルのILLコストです。これは、ILLトランザクションコストとILLリクエスト率に基づいており、これらはいずれも調整可能なパラメータです。詳しくはこちらの記事をご覧ください。\[How do we calculate ILL requests and ILL cost?(ILLリクエストとILLコストの計算方法)]\(../how-it-works/how-do-we-calculate-ill-requests and-ill-cost.md)

**subscription\_minus\_ill\_cost**

The net cost of the subscription, which is the Subscription cost above minus the ILL cost (since almost all universities will offer a journal by ILL if they didn't subscribe). For some journals with very high Usage and low subscription prices this number is actually negative -- subscribing is \*cheaper\* than filling all the anticipated ILL requests. 購読のNETコストについては、上記の購読費用からILL費用（購読しなかった場合、ほとんどすべての大学がジャーナルをILLで提供するため）を差し引いたものである。利用率が非常に高く購読料が安いジャーナルでは、この数値は実際にはマイナスになる--購読は、予想されるすべてのILLリクエストを満たすよりも、 \*cheaper(安い)\*という結果となります。

### Fulfillment <a href="#fulfillment" id="fulfillment"></a>

### Fulfillment（実現可能性） <a href="#fulfillment" id="fulfillment"></a>

**use\_oa\_percent**

The percent of Usage that can be fulfilled via as Green, Hybrid, or Bronze Open Access. Some of this content can be excluded in the settings (see the Open Access page for more info). グリーン、ハイブリッド、ブロンズのそれぞれのOAとして経由して満たすことができる使用状況の割合となります。このコンテンツの一部は、設定で除外することができます（詳しくは、オープンアクセスのページをご覧ください）。

**use\_backfile\_percent**

The percent of Usage that can be fulfilled via your PTA (Post-Termination Access) rights. PTA (Post-Termination Access)権により実現可能な利用率の割合となります。\
**use\_subscription\_percent**

Percent of Usage that can be fulfilled ONLY via title-by-title subscription in this scenario--after fulfilling requests via Open Access and PTA fulfillment wherever possible. このシナリオでは、タイトルごとの購読によってのみ満たされる利用率--可能な限りオープンアクセスおよびPTAによる要求を満たした後の利用率となります。

**use\_ill\_percent**

Percent of Usage that is fulfilled via ILL in this scenario. This is simply turnaways (Usage that can't be fulfilled by Open Access, PTA, or your title-by-title subscriptions) multiplied by your ILL Request Rate parameter. This article has more details: How do we calculate ILL requests and ILL cost? このシナリオでILL経由で満たされる利用率の割合。これは、Turnaways（オープンアクセス、PTA、またはタイトルごとの購読によって満たされない使用量）にILLリクエスト率パラメータを掛けたものです。詳しくはこちらの記事をご覧ください。\[How do we calculate ILL requests and ILL cost?(ILLリクエストとILLコストの計算方法)]\(../how-it-works/how-do-we-calculate-ill-requests and-ill-cost.md)

**use\_other\_delayed\_percent**

Percent of Usage that is fulfilled via Unknown paths in this scenario. This all Usage that isn't fulfilled by Open Access, PTA rights, title-by-title subscription or ILL. Instead, the user fulfills their information need some other way -- asks the author for a paper, asks a colleague, finds another similar paper that is good enough for their purposes, etc. このシナリオで、不明な経路で満たされた利用量の割合。これは、オープンアクセス、PTA権、タイトルごとの購読、ILLによって満たされないすべての利用となります。例えば、著者に論文を依頼する、同僚に依頼する、自分の目的に合った別の類似論文を見つける、などとなります。

**perpetual\_access\_years\_text**

The years when your institution has PTA (Post-Termination Access) to this title. Default: empty. 自機関がこのタイトルにPTA（Post-Termination Access）を持っている年数です。デフォルト：emptyとなります。\
**baseline\_access\_text**

Optional text for those who have already left their Big Deals, to annotate which journals they'd previously subscribed to. すでにBig Dealsをを解約した施設のために、以前購読していたジャーナルを注釈するためのオプションテキスト。

**bronze\_oa\_embargo\_months**

For some journals the publisher automatically makes the content free to read after a certain number of months. For those journals, this column lists the age of the articles (in months) when they will automatically become free to read on the publisher's site. ジャーナルによっては、出版社がある月数を過ぎると自動的にコンテンツを無料で読めるようにするものがあります。そのようなジャーナルについては、この欄は、出版社のサイトで自動的に無料で読めるようになる時期の論文の年齢（月単位）をリストアップしています。

### Usage Components <a href="#usage-components" id="usage-components"></a>

**downloads**

The number of times people in your institution will download papers from this journal. We base this on your COUNTER statistics and literature on [download decay curves](https://www.biorxiv.org/content/10.1101/795310v1) (how often an article is to be downloaded based on how long ago it was published). 自機関の研究者が、このジャーナルから論文をダウンロードする回数です。これは、自機関のCOUNTERレポートと[download decay curves](https://www.biorxiv.org/content/10.1101/795310v1)（論文が公開されてからどれくらいの期間でダウンロードされるか）に関する文献を基に算出しています。

**citations**

The number of times that a paper authored by someone in your institution will cite a paper in this journal. This number is based on the citations patterns of the previous five years. The importance of this number to overall Usage is determined by the Citation Weight parameter. 自機関の研究者が執筆した論文が、このジャーナルの論文を引用する回数です。この数値は、過去5年間の引用パターンに基づいています。利用状況全体に対するこの数値の重み付けは、Citation Weightパラメータで決定することができます。

**authorships**

The number of papers in this journal that have at least one author from your institution. This number is based on the authorship patterns of the previous five years. The importance of this number to overall Usage is determined by the Authorship Weight parameter. このジャーナルに掲載された論文のうち、所属機関から少なくとも1名の著者が出ている論文の数です。この数値は、過去5年間のオーサーシップパターンに基づいています。この数値が全体の利用率に占める重み付けは、Authorship Weightパラメータで決定することができます。

### Fuzzed <a href="#fuzzed" id="fuzzed"></a>

#### **\*\_fuzzed** <a href="#fuzzed" id="fuzzed"></a>

We include a few "fuzzed" columns, in case you want to share this data approximately but not exactly. For each column that's fuzzed, we ranked all the values in a column, then separated the values into three equal sized groups, and labelled them low, medium, and high. Low refers to the lowest value by rank, high refers to the highest value by rank, and medium in the middle. Where there is no value for the un-fuzzed value, we use a dash ("-"). このデータは、正確ではありませんが、おおよそを共有したい場合に備えて、いくつかの”fuzzed(ファジー化"された列を含んでいます。ファジー化された各列では、列内のすべての値をランク付けし、その値を3つの同じ大きさのグループに分けて、低、中、高とラベル付けしています。lowは順位が最も低い値、highは順位が最も高い値、mediumはその中間の値を指します。ファジングされていない値が存在しない場合は、ダッシュ（"-"）を使用しています。

If you want more fine grained resolution among titles you can refer to the un-fuzzed columns.\
タイトル間の解像度をより細かくしたい場合は、un-fuzzed columns( ファジーかしていないカラム） を参照することができます。\\

\\
