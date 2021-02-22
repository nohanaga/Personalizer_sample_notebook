# Personalizer simulation in an Azure notebook

このチュートリアルでは、顧客がどのタイプのコーヒーを注文すべきかを提案する Personalizer ループシステムをシミュレートしています。ユーザーとその好みは、[user dataset](users.json) に保存されます。コーヒーに関する情報も利用可能で、[coffee dataset](coffee.json)に格納されています。

10,000 リクエストに対してシステムを実行し、システムがどれだけ速く正確に学習したかを示すグラフを作成します。

オフラインの反事実的影響評価を実行して、最適化された学習ポリシーを選択し、そのポリシーを適用する。

2,000 リクエストに対してシステムを再度実行し、システムの精度を示すグラフを作成します。

## 前提条件

* [Personalizer リソース](https://ms.portal.azure.com/#create/Microsoft.CognitiveServicesPersonalizer)

## このサンプルの使い方

説明書はすべてノートに書いてあります。ここでは省略して説明します。

1. Jupyter Notebook で Personalizer.ipynb ファイルを開き、以下の値を変更します。

    * `personalization_base_url` の `<your-resource-name>` の値を、Personalizer リソースの値に変更します。
    * 変数 `<your-resource-key>` の値を、Personalizer のリソースキーの 1 つに設定します。

1. 各セルを上から下へと実行します。各セルが完了するまで待ってから次のセルを実行します。

## 参考

* [Full sample](https://github.com/Azure-Samples/cognitive-services-personalizer-samples/tree/master/samples/azurenotebook)
* [Tutorial on docs.microsoft.com](https://docs.microsoft.com/azure/cognitive-services/personalizer/tutorial-use-azure-notebook-generate-loop-data)
