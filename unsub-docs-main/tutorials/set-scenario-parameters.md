# Set scenario parameters
# シナリオ・パラメータの設定

{% hint style="warning" %}
Have you created a scenario yet? If not go [do that now](create-and-work-with-scenarios.md).
シナリオはもう作成されましたか？もしまだなら、[do that now(今すぐ)](create-and-work-with-scenarios.md) をご覧ください。
{% endhint %}

Click the **Parameters** tab
**Parameters**タブをクリックください。

You should see a page of the nine parameters and their details
9つのパラメータとその詳細のページが表示されます。

![](../.gitbook/assets/parameters-tab.png)

The first thing to notice is that you can toggle on or off the description (details) for each parameter.
まず注目すべきは、各パラメーターの説明（詳細）のオン・オフを切り替えられる点です。

![](../.gitbook/assets/parameter-details.png)

By default the parameter details are shown.
デフォルトでは、パラメータの詳細が表示されます。

There are nine different parameters you can configure. We encourage you to look into each of them. However, for this tutorial we'll explore just one of the parameters: Bronze OA.&#x20;
設定できるパラメータは9種類です。それぞれについて調べてみることをお勧めします。しかし、このチュートリアルでは、パラメータのうちの1つだけを調べてみます。ブロンズOAです。&#x20;

Bronze OA is when a paper is made freely available on a publisher website without an open license - in which case the paper could be taken down at any time.&#x20;
ブロンズOAとは、論文がオープンライセンスなしで出版社のウェブサイトで自由に利用できるようにされることで、この場合、論文はいつでもオープンアクセスから取り下げられる可能性があります &#x20;

By default we include Bronze OA (Open Access) in our forecasts.&#x20;
デフォルトでは、予測にブロンズOA（オープンアクセス）が含まれています&#x20;

Looking at the Parameters tab, **Include Bronze OA** should look like this:
Parametersタブを見ると、**Include Bronze OA**は以下ように表示されてます。

![Include Bronze OA (Open Access) = true](../.gitbook/assets/scenario-params-bronze-oa-true.png)

Now, click anywhere on the area of the parameter name, description, or the value (in this case **true**). You'll then get a popup like:
ここで、パラメータ名、説明、または値（ここでは **true**）の領域のどこかをクリックします。クリックすると、このようなポップアップが表示されます。

![Bronze OA (Open Access) popup, toggled to True](../.gitbook/assets/scenario-params-bronze-oa-popup.png)

Click on the area on the popup with the blue switch and the text **Include Bronze OA**. That click should move the switch to the left and turn it white looking like:
ポップアップの青いスイッチと **Include Bronze OA** というテキストがある部分をクリックします。すると、スイッチが左に移動し、以下のような白色に変わります。

![Bronze OA (Open Access) popup, toggled to False](../.gitbook/assets/scenario-params-bronze-oa-popup-false.png)

Then click **Save**. You're done! Your scenario now will not include Bronze OA.&#x20;
そして、**Save(保存)**をクリックします。これで完了です。これで、シナリオにはブロンズOAが含まれなくなりました。

To make sure changing this parameter changed the scenario, let's compare screenshots of the scenario before and after changing the Bronze OA parameter. Although the entire scenario changes, let's focus on the Cost and Access bars on the left of the scenario.&#x20;
このパラメータを変更することでシナリオが変化したことを確認するために、Bronze OAパラメータを変更する前と後のシナリオのスクリーンショットを比較してみましょう。シナリオ全体が変化していますが、シナリオの左側にあるコストバーとアクセスバーに注目しましょう。&#x20;

**Include Bronze OA = true**

![](../.gitbook/assets/scenario-bronze-oa-true-just-bars.png)

**Include Bronze OA = false**

![](../.gitbook/assets/scenario-bronze-oa-false-just-bars.png)

Comparing the two images above, you can see that cost has changed, with higher ILL costs when Bronze OA is not included - more money needs to be spent on ILL to fulfill article requests. In addition, access has changed: open access fulfillment dropped from 35% when including Bronze OA to 30% when we didn't include Bronze OA.
上の2つの画像を比較すると、コストが変化していることがわかります。ブロンズOAを含めない場合、ILLコストが高くなり、論文のリクエストを満たすためにILLに多くの資金が必要になります。さらに、アクセスも変化しています。オープンアクセスのFulfillment(実現可能性)は、ブロンズOAを含めると35%から、ブロンズOAを含めない場合は30%に低下しています。



For a description of each scenario parameter see our article on [Scenario parameters](../reference/scenarios/scenario-parameters.md).
各シナリオパラメータの説明については、[Scinario parameters(シナリオパラメータ)](../reference/scenarios/scenario-parameters.md)の記事をご覧ください。

## **What's Next?**
## **次の作業について**

Now that you’ve created set scenario parameters, the next step is [Comparing Scenarios](comparing-scenarios.md)
シナリオのパラメータを設定したので、次は[Comparing Scenarios(シナリオの比較)](comparating-scenarios.md)を学びましょう。
