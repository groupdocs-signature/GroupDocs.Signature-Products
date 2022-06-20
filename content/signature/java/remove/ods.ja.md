---
layout: "auto-gen"
date: 2021-05-13T13:40:06+03:00
draft: false

head_title: "JavaのODSからデジタル署名を削除する"
head_description: "クリアするJavaライブラリ＆amp; GroupDocs.Signature APIを使用してODSファイルからデジタル署名を削除します-画像、バーコード、QRコード、スタンプ、テキスト、光学および光学を操作します。デジタル署名されたドキュメントからのメタデータ署名."

title: "Javaを介してODSからデジタル署名を削除する"
description: "ODSファイルからデジタル署名を削除するJavaeSignatureライブラリ。デジタル署名されたドキュメントからの画像、バーコード、QRコード、スタンプ、テキスト、光学、メタデータの署名を簡単に操作できます."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "無料トライアルをダウンロード"
    link: "https://downloads.groupdocs.com/signature/java"

submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:

            - link: "https://apireference.groupdocs.com/signature/java"
              text: "APIリファレンス"

            - link: "https://github.com/groupdocs-signature"
              text: "コード例"

            - link: "https://products.groupdocs.app/signature/family"
              text: "ライブデモ"

            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "価格設定"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java"
        link_buy: "https://purchase.groupdocs.com"

about:
    enable: true
    title: "GroupDocs.Signature for Java APIについて"
    content: |
        [GroupDocs.Signature for Java](/signature/java/)は、テキスト、画像、バーコード、スタンプ、フォームフィールド、QRコード、メタデータなどのさまざまな署名署名タイプを使用してドキュメントにデジタル署名する高度なJavaeSignatureライブラリです。ほんの数行のコードを追加するだけで、PDF、Microsoft Word、Excelワークシート、PowerPointプレゼンテーション、Adobe Photoshop、メタファイル、および画像ファイル形式内のデジタル署名を表示、追加、編集、検証、削除、および検索する機能をJavaアプリケーションに提供します。 e-signature APIは、要件に応じて署名プロパティをカスタマイズするための追加機能もサポートしています。

steps:
    enable: true
    title_left: "ODSからデジタル署名を削除する方法"
    content_left: |
        以下のJavaコード例は、数行のコードを追加するだけで、**JavaのODSファイルからテキスト署名を削除**する手順を明確に示しています。

        * ** Signature **クラスの新しいインスタンスを作成し、コンストラクターパラメーターとしてソースドキュメントパスを渡します。
        * 必要なプロパティを使用して**TextSearchOptions** オブジェクトをインスタンス化します。
        * ** search **メソッドを呼び出して、**TextSignatures**のリストを取得します。
        *ドキュメントから削除する**TextSignature** オブジェクトを選択します。
        * **Signature** オブジェクト**delete**メソッドを呼び出し、1つまたは複数の署名を渡します。
        * ** DeleteResult **の結果を分析して、署名が更新されたかどうかを確認します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for Java APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティングシステム: Microsoft Windows、Linux、MacOS
        * 開発環境: Visual Studio、Xamarin、MonoDevelop
        * フレームワーク: .NET Framework、.NET Standard、.NET Core、Mono
        * [NuGet](https://www.nuget.org/packages/groupdocs.signature)から最新バージョンのGroupDocs.SignatureforJavaをダウンロードします。
        
    code: |
        ```java
        //署名インスタンスを初期化します
        Signature signature = new Signature("signed.pdf");
         
        TextSearchOptions options = new TextSearchOptions();
         
        List signatures = signature.search(TextSignature.class,options);
        List signaturesToDelete = new ArrayList();
        //削除する署名を収集します
        for (TextSignature temp : signatures)
        {
            if (temp.getText().contains("JS"))
            {
                signaturesToDelete.add(temp);
            }
        }
        //署名を削除します
        DeleteResult deleteResult = signature.delete("signed.ods", signaturesToDelete);
        if (deleteResult.getSucceeded().size() == signaturesToDelete.size())
        {
            System.out.print("All signatures were successfully deleted!");
        }
        else
        {
            System.out.print("Successfully deleted signatures : " + deleteResult.getSucceeded().size());
            System.out.print("Not deleted signatures : " + deleteResult.getFailed().size());
        }
        System.out.print("List of deleted signatures:");
        for(BaseSignature temp : deleteResult.getSucceeded())
        {
            System.out.print("Signature# Id:"+temp.getSignatureId()+", Location: "+temp.getLeft()+"x"+temp.getTop()+". Size: "+temp.getWidth()+"x"+temp.getHeight());
        }
        ```
        
demos:
    enable: true
    title: "ODS署名ライブデモを削除する"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、ODSファイルの電子署名を今すぐ追加してください。
        ライブデモには次の利点があります
about_formats:
    enable: true
    format:
        - icon: "far fa-file-ods"
          title: "ODSファイル形式とは"
          content: |
            ODS拡張子の付いたファイルは、ユーザーが編集できるOpenDocumentスプレッドシートドキュメント形式を表します。データはODFファイル内の行と列に保存されます。これはXMLベースの形式であり、Open Document Formats（ODF）ファミリのいくつかのサブタイプの1つです。このフォーマットは、OASISによって公開および保守されているODF1.2仕様の一部として指定されています。 Windowsやその他のオペレーティングシステム上の多くのアプリケーションは、Microsoft Excel、NeoOffice、LibreOfficeなど、編集や操作のためにODSファイルを開くことができます。 ODSファイルは、さまざまなアプリケーションによってXLS、XLSXなどの他のスプレッドシート形式に変換することもできます。 ODSファイル形式の詳細

          link: "https://docs.fileformat.com/spreadsheet/ods/"

more_formats:
    enable: false
    title: "その他の利用可能なオプション"
    content: |
        ドキュメントと画像のマルチフォーマットデジタル署名削除API。以下に示すように、一般的なファイル形式のいくつかから署名を削除します。
    format: 
          link: "/signature/java/remove/pdf/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/java/remove/doc/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/java/remove/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/java/remove/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/java/remove/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/java/remove/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/java/remove/dotm/"
          description: "MicrosoftWordマクロ対応テンプレート"

          link: "/signature/java/remove/rtf/"
          description: "リッチテキストドキュメント"

          link: "/signature/java/remove/odt/"
          description: "ドキュメントテキストを開く"

          link: "/signature/java/remove/ott/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/java/remove/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/java/remove/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/java/remove/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/java/remove/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/java/remove/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/java/remove/xltx/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/java/remove/xltm/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/java/remove/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/java/remove/ots/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/java/remove/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/java/remove/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/java/remove/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/java/remove/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "/signature/java/remove/potm/"
          description: "MicrosoftPowerPointマクロ対応テンプレート"

          link: "/signature/java/remove/potx/"
          description: "MicrosoftPowerPointテンプレート"

          link: "/signature/java/remove/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "/signature/java/remove/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/java/remove/otp/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/java/remove/webp/"
          description: "WebP画像"

          link: "/signature/java/remove/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/java/remove/jpeg/"
          description: "JPEG画像"

          link: "/signature/java/remove/gif/"
          description: "グラフィック交換フォーマット"

          link: "/signature/java/remove/png/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/java/remove/bmp/"
          description: "ビットマップファイル形式"

          link: "/signature/java/remove/cdr/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/java/remove/svg/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/java/remove/psd/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/java/remove/wmf/"
          description: "Windowsメタファイル"

          link: "/signature/java/remove/emf/"
          description: "強化されたメタファイル形式"

          link: "/signature/java/remove/cmx/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/java/remove/djvu/"
          description: "既視感"

          link: "/signature/java/remove/ppsm/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

          link: "/signature/java/remove/dcm/"
          description: "医学におけるデジタルイメージングと通信"


back_to_top:
    enable: true
---
