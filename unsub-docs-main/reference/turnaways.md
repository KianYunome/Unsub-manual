---
description: Titles with only turnaways may show up in your dashboard(Turnawayのみを含むタイトルがダッシュボードに表示される場合)
---

# Turnaways

Unsub modeling uses many parameters, [many of which are user-configurable](scenarios/scenario-parameters.md). One of the many parameters we use is turnaways data.
Unsubのモデリングでは、多くのパラメータを使用し、[many of which are user-configurable(多くはユーザーが設定可能)](scenarios/scenario-parameters.md)。多くのパラメータの1つに、Turnawayデータがあります。

COUNTER 5 includes turnaways data in the TR\_J2 file (named "Journal Access Denied").
COUNTER 5では、TR_J2ファイル（ファイル名："Journal Access Denied"）にturnawaysのデータが収録されています。

We include all titles in the TR\_J2 file that have data for the metric **No\_License** unless they fall into one of the [exceptions explained here](../troubleshooting/why-dont-i-see-a-certain-title-in-my-dashboard.md).
TR_J2ファイルには，メトリック**No\_License**のデータを持つすべてのタイトルが含まれます．ただし，[exceptions explained here（例外の説明はこちら)](../troubleshooting/why-dont-i-see-a-certain-title-in-my-dashboard.md) に該当するものは除外されます．

We include those titles because they are cases of people attempting to access the full-text of an article that were redirected to the abstract.
これらのタイトルは、論文のフルテキストにアクセスしようとした人が、抄録にリダイレクトされたケースであるため、このタイトルが含まれています。

In Unsub we want to account for what people want to read - regardless of whether they have access to full-text or not. This is why we include turnaways: to better account for everything users want to read.
Unsubでは、フルテキストにアクセスできるかどうかに関係なく、人々が読みたいものを考慮したいと考えています。このため、Unsubでは、ユーザが読みたいものすべてに対応できるよう、turnawayのデータを収録しています。

Note**:** If you’re using COUNTER 4 we do not count turnaways because they are not included in COUNTER 4. However, if you use COUNTER 5 we do count turnaways.
注意**:** COUNTER 4を使用している場合、turnawayデータはCOUNTER 4に含まれていないためカウントされません。 しかし、COUNTER 5を使用している場合、turnawayはカウントされます。
