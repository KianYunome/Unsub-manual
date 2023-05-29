# Mini bundle pricing(ミニバンドル価格)

Some publishers advertise a special price if you buy a few titles bundled together (and they often assign this "mini bundle" its own ISSN).(出版社によっては、いくつかのタイトルをまとめて購入すると特別価格になるとしています（そして出版社はしばしば、この「ミニバンドル」に独自のISSNを割り当てます）。)

Currently Unsub only supports pricing at the single-journal level. We have a few suggestions on how to handle "mini bundles", though not any perfect solution yet unfortunately.(現在、Unsubは単一ジャーナルレベルでの価格設定のみをサポートしています。ミニバンドル」をどのように扱うかについて、いくつかの提案をしていますが、残念ながらまだ完全な解決策ではありません。)

What some Unsub users have done is remove the non-primary bundled titles (so all the journals except for its "main" title) from their COUNTER files (like, delete those rows, then re-upload), so they don't show up in their forecasts, and then if it came to subscribing you'd get them for "free" from the publisher if the main journal is enough to warrant subscribing.(一部のUnsubユーザーは、COUNTERファイルから主要でないバンドルタイトル（つまり「メイン」タイトル以外のすべてのジャーナル）を削除して（行を削除して再アップロードするなど）、予測に表示されないようにしました。)

A different workaround others have done is to add the usage together for the bundles in their COUNTER file (you only have to modify the "total", we ignore the months columns) so that usage of the other titles are included in the main title.(他の方が行った別の回避策は、COUNTERファイルでバンドル版の使用量を合算し（「合計」だけを修正すればよく、月の列は無視します）、他のタイトルの使用量がメインタイトルに含まれるようしました。)

You could make the price be $0 for "free with a bundle", but then its Cost Per Use will be $0 and any way of subscribing by most cost effective journal first will pick it, which could get confusing.("Free with a bundle:バンドルで無料"の場合、価格を$0にすることもできますが、そうするとCost Per Useが$0になり、最も費用対効果の高いジャーナルを最初に購読する方法が選ばれるため、混乱する可能性があります。)
