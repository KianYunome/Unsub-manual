---
description: An important piece of fulfillment(Fulfillment(実現可能性)の重要なアイテム)
---

# Does Unsub account for Sci-Hub usage?(UnsubはSci-Hubの利用を考慮してますか?)

The Unsub Scenario view helps you visualize your fulfillment based on a variety of data inputs and parameter settings.(Unsub Scenario Viewは、様々なデータ入力とパラメータ設定に基づいたFulfillment(利用実現可能性)を視覚化するのに役立ちます。)

The "Unknown" portion of fulfillment (see figure below) can be a significant part of your fulfillment in some scenarios, especially if you have not added any title-by-title subscriptions. The Unknown grey portion of fulfillment is essentially "the reader is on their own".(Fullfilment(利用実現可能性)の「Unknown」部分（下図参照）は、特にタイトルごとの購読を追加していない場合、いくつかのシナリオでFulfillment(利用実現可能性)の重要な部分となる可能性があります。Fulfillment(利用実現可能性)の「Unknown」グレー部分は、基本的に「読み手による自己判断」となります。)

![](../.gitbook/assets/account-for-scihub.png)

A reader being on their own can mean many things, including asking the author of the paper for a PDF, asking a colleague for a PDF, and even using Sci-Hub.(読み手による自己判断というのは、論文の著者にPDFを頼む、同僚にPDFを頼む、さらにはSci-Hubを使うなど、いろいろな意味があります。)

You may be wondering if Unsub accounts for Sci-Hub in this grey Unknown portion of fulfillment.(このグレーのfulfillment(利用実現可能性)Unknownの割合の中で、どこまでSci-Hubで充足させることができるか気になるところです。)

Yes, Unsub does account for Sci-Hub, but not explicitly. Unsub has a parameter called "ILL Request Rate"; see [here](../reference/scenarios/scenario-parameters.md) and [here](how-do-we-calculate-ill-requests-and-ill-cost.md) for more on the ILL Request Rate parameter. This parameter has a default of 5%. That is, 1 out of every 20 times a paper is sought by a reader an ILL request happens. Presumably that rate goes down if people are using Sci-Hub more.(はい、UnsubはSci-Hubを考慮しますが、明示的ではありません。Unsubには「ILL Request Rate」というパラメータがあります。ILL Request Rate パラメータについては[こちら](../reference/scenarios/scenario-parameters.md)と[こちら]( how-do-we-calculate-ill-requests-and-ill-cost.md) を参照してください。このパラメータのデフォルトは5%です。つまり、ある論文が読者の20回の要求に1回の割合でILLリクエストが発生します。Sci-Hubの利用が増えれば、この比率は下がると思われます。)

One way you could indirectly model different Sci-Hub usage levels is to change the ILL Request Rate parameter - comparing different Unsub scenarios with different ILL Request Rate values.(間接的にSci-Hubの利用レベルの違いをモデル化する一つの方法として、ILL Request Rateパラメータを変更し、異なるILL Request Rateの値で異なるUnsubシナリオ作成して比較することができます。)
