# BoringColumnXMLConversionTool-for-ArcGISPro
## 概要
「ボーリング柱状図 XML 変換ツール for ArcGIS Pro」は、国土交通省「地質・土質調査成果電子納品要領」に基づいて作成されたボーリング交換用データ XML ファイルを読み込み、標題情報、および個別の調査・試験項目ごとのフィーチャクラスで構成されるファイル ジオデータベースにデータを変換するためのツールです。 
### リリース履歴
* 2023/9/11 :「ボーリング柱状図 XML 変換ツール for ArcGIS Pro」を公開

## 対応データ
本ツールでサポートする XML DTD バージョンは次の通りです。  
* DTD version 2.10 (BED0210.DTD) 
* DTD version 3.00 (BED0300.DTD) 
* DTD version 4.00 (BED0400.DTD)

基本的に DTD version 4.00 で規定される XML 要素、DTD version 2.10、3.00 で規定される XML 要素のうち version 4.00 に同等の要素がある要素を変換の対象とします。XML 要素とファイル ジオデータベースのフィーチャクラスのフィールドに「標題情報」については要素が、「コア情報」では要素の各子要素がマッピングされます。 

変換されるファイル ジオデータベースの詳細な定義は、「[ボーリング柱状図 XML 変換ツールスキーママッピング.xlsx](https://github.com/EsriJapan/BoringColumnXMLConversionTool-for-ArcGISPro/blob/main/Docs/%E3%83%9C%E3%83%BC%E3%83%AA%E3%83%B3%E3%82%B0%E6%9F%B1%E7%8A%B6%E5%9B%B3XML%E5%A4%89%E6%8F%9B%E3%83%84%E3%83%BC%E3%83%AB%E3%82%B9%E3%82%AD%E3%83%BC%E3%83%9E%E3%83%9E%E3%83%83%E3%83%94%E3%83%B3%E3%82%B0.xlsx)」をご参照ください。 
 

## 動作環境 
本ツールを実行するには、バージョン 3.1 以上の ArcGIS Pro と ArcGIS Data Interoperability エクステンション をインストールし（ArcGIS Pro とArcGIS Data Interoperability のインストーラーは、それぞれ別々に提供されております。My Esri からそれぞれのインストーラーを入手いただき、インストールして頂く必要があります）、ライセンスを有効化している必要があります。 

詳細な動作環境、およびData Interoperability エクステンション のインストール方法は、以下をご参照ください。
* [ArcGIS Pro の動作環境](https://www.esrij.com/products/arcgis-pro/spec/)
* [Data Interoperability エクステンションのインストール](https://pro.arcgis.com/ja/pro-app/latest/help/data/data-interoperability/install-the-data-interoperability-extension.htm)

## 利用方法
「[ボーリング柱状図 XML 変換ツール for ArcGIS Pro](https://github.com/EsriJapan/BoringColumnXMLConversionTool-for-ArcGISPro/releases/download/v1.0.0/boringColumnXmlConersionArcGISPro.zip)」をダウンロードして任意の場所に解凍してご利用ください。
このとき、ツールのフルパスにマルチバイト文字（日本語など）が含まれないようにしてください。

利用方法の詳細は「[ボーリング柱状図 XML 変換ツール for ArcGIS Pro 利用ガイド](https://github.com/EsriJapan/BoringColumnXMLConversionTool-for-ArcGISPro/blob/main/Docs/%E3%83%9C%E3%83%BC%E3%83%AA%E3%83%B3%E3%82%B0%E6%9F%B1%E7%8A%B6%E5%9B%B3%20XML%20%E5%A4%89%E6%8F%9B%E3%83%84%E3%83%BC%E3%83%AB%20for%20ArcGIS%20Pro%20%E5%88%A9%E7%94%A8%E3%82%AC%E3%82%A4%E3%83%89%20.pdf)」をご参照ください。 

## 免責事項
* 本ツールに含まれるカスタムツールは、サンプルとして提供しているものであり、動作に関する保証、および製品ライフサイクルに従った Esri 製品サポート サービスは提供しておりません。
* 本ツールに含まれるツールによって生じた損失及び損害等について、一切の責任を負いかねますのでご了承ください。
* 弊社で提供している Esri 製品サポートサービスでは、本ツールに関しての Ｑ＆Ａ サポートの受付を行っておりませんので、予めご了承の上、ご利用ください。詳細は[
ESRIジャパン GitHub アカウントにおけるオープンソースへの貢献について](https://github.com/EsriJapan/contributing)をご参照ください。

## ライセンス
Copyright 2023 Esri Japan Corporation.

Apache License Version 2.0（「本ライセンス」）に基づいてライセンスされます。あなたがこのファイルを使用するためには、本ライセンスに従わなければなりません。
本ライセンスのコピーは下記の場所から入手できます。

> http://www.apache.org/licenses/LICENSE-2.0

適用される法律または書面での同意によって命じられない限り、本ライセンスに基づいて頒布されるソフトウェアは、明示黙示を問わず、いかなる保証も条件もなしに「現状のまま」頒布されます。本ライセンスでの権利と制限を規定した文言については、本ライセンスを参照してください。

ライセンスのコピーは本リポジトリの[ライセンス ファイル](./LICENSE)で利用可能です。
