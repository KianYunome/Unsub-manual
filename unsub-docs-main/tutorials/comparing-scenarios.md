# Comparing scenarios
# シナリオの比較

{% hint style="warning" %}
Have you created a scenario yet? If not go [do that now](create-and-work-with-scenarios.md).
シナリオはもう作成されましたか？まだなら、[do that now(今すぐやる)](create-and-work-with-scenarios.md)をご覧ください。
{% endhint %}

Within an Unsub package you can have as many scenarios as you like.&#x20;
Unsubパッケージ内では、好きなだけシナリオを作成することができます。&#x20;

Comparing different scenarios is a powerful way to compare different choices about subscribed titles and scenario parameters. Remember, scenarios within a package share the same COUNTER, PTA and title price data - those data do not differ among scenarios within a package.
異なるシナリオを比較することで、購読されたタイトルやシナリオのパラメータを比較することができます。パッケージ内のシナリオは、同じCOUNTER、PTA、タイトル価格データを共有していることに注意してください。

### Compare scenarios
###　　シナリオの比較

Here, we'll compare two scenarios. If you haven't created a scenario yet, follow the [Create a scenario](create-and-work-with-scenarios.md) tutorial to create a scenario now.&#x20;
ここでは、2つのシナリオを比較します。まだシナリオを作成していない場合は、チュートリアルの[Create a scenario(シナリオを作成する)](create-and-work-with-scenarios.md)に従って、今すぐシナリオを作成してください.&#x20;

After creating a scenario [make a copy of the scenario](../how-to-guides/copy-a-scenario.md).&#x20;

シナリオを作成したら、[make a copy of the scenario(シナリオのコピーを作成する)](../how-to-guides/copy-a-scenario.md)をクリックします。.&#x20;

On creating a copy of a scenario you are dropped into the copied scenario. In the copied scenario let's change one parameter setting then compare results.&#x20;
シナリオのコピーを作成すると、コピーされたシナリオにドロップされます。コピーしたシナリオのパラメータを1つ変更し、結果を比較します &#x20;

Click on the Parameters tab in your copied scenario. You should now see a page of the nine parameters.&#x20;
コピーしたシナリオのパラメータ(Parameters)タブをクリックします。これで、9つのパラメータが表示されます。&#x20;

![](../.gitbook/assets/parameters-tab.png)

For this tutorial we'll change one of the Fulfillment sources parameters: **Include Bronze OA**
このチュートリアルでは、Fulfillment（実現可能性）ソースのパラメータを1つ変更します。**Include Bronze OA(ブロンズOAを含める)**」を変更します。

By default **Include Bronze OA** is **true**. Click on that parameter and click the blue button to turn it to false, then click Save.
デフォルトでは **Include Bronze OA(ブロンズOAを含める)** は **true** です。このパラメータをクリックし、青いボタンをクリックしてfalseに変更し、[Save(保存)]をクリックします。

You should now see a change in your forecast.&#x20;
これで、forcastに変化が見られるはずです。&#x20;

Now navigate to the package page with your two scenarios: the original scenario you created, and the copied scenario.&#x20;
次に、2つのシナリオを含むパッケージページに移動します：作成したオリジナルのシナリオと、コピーしたシナリオです。&#x20;

You should see something like:
以下が表示されると思います。

![](../.gitbook/assets/two-scenarios.png)

In the above view you can easily see the difference in Cost and Access between your scenarios. In the example above the two scenarios are identical except for the **Include Bronze OA** parameter (true in "First Scenario", false in "Copy of First Scenario").&#x20;
上記の表示では、シナリオ間のコストとアクセスの違いを簡単に確認することができます。上の例では、**Include Bronze OA** パラメータ（"First Scenario "ではtrue、"Copy of First Scenario "ではfalse）以外、2つのシナリオは同じです。 &#x20;

Cost is about $24,000 less and access 3% higher in "First Scenario" relative to "Copy of First Scenario".&#x20;
First Scenario "では、"Copy of First Scenario "と比較して、コストは約24,000ドル低く、アクセスは3%高くなっています.&#x20;

As you add more scenarios you can compare cost and access across them all.&#x20;
さらにシナリオを追加すると、すべてのシナリオでコストとアクセスを比較することができます。 &#x20;

## **What's Next?**
## **次の作業について**

The next step is learning about the Unsub [Consortial Dashboard](consortial-dashboard.md).&#x20;
次は、Unsub [Consortial Dashboard](consortial-dashboard.md) について学習します。&#x20;
{% hint style="warning" %}
Note: Most Unsub users **DO NOT** have a consortial dashboard.
注意: ほとんどの Unsub ユーザは **DO NOT** [Consortial dashboard(コンソーシアム・ダッシュボード)](consortial-dashboard.md)を持っていません。
{% endhint %}
