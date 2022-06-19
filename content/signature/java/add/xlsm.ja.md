---
layout: "auto-gen"
date: 2021-05-13T13:39:52+03:00
draft: false

head_title: "JavaでXLSMファイルにデジタル署名を追加する方法"
head_description: "GroupDocs.SigantureAPIを使用してJavaのXLSMファイルにデジタル署名を追加する方法を学ぶ-一般的なビジネスドキュメントや画像ファイル形式にカスタマイズされた電子署名を追加する."

title: "JavaのXLSMにデジタル署名を追加する"
description: "Javaライブラリを使用して一般的なデジタル署名タイプを追加することにより、XLSMファイルを保護します。必要に応じて、電子署名のプロパティを操作し、ドキュメント内に事前署名オプションを設定します."
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
        [GroupDocs.Signature for Java](/signature/java/)は、テキスト、画像、バーコード、スタンプ、フォームフィールド、QRコード、メタデータなどのさまざまな署名タイプを使用してドキュメントにデジタル署名するための高度なJavaライブラリです。ほんの数行のコードを追加するだけで、PDF、Microsoft Word、Excelワークシート、PowerPointプレゼンテーション、Adobe Photoshop、メタファイル、および画像ファイル形式内のデジタル署名を追加、編集、検証、削除、および検索する機能をJavaアプリケーションに提供します。 e-signature APIは、要件に応じて署名プロパティをカスタマイズするための追加機能もサポートしています。

steps:
    enable: true
    title_left: "XLSMファイルにデジタル署名を追加する方法"
    content_left: |
        以下のコード例は、数行のコードを追加するだけで、** Javaの[GroupDocs.Signature](/signature/java/)ライブラリを使用してXLSMファイルにデジタル署名を追加する方法**に関する手順を明確に示しています。

        * [Signature](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature)クラスの新しいインスタンスを作成し、コンストラクターパラメーターとしてソースドキュメントパスを渡します。
        * [DigitalSignOptions](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature.options.sign/DigitalSignOptions)オブジェクトを必要な証明書とパスワードでインスタンス化します。
        * [Sign](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature#sign(java.io.OutputStream,%20com.groupdocs.signature.options.sign.SignOptions）)に電話してください[Signature](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature)クラスインスタンスのメソッド。 DigitalSignOptionsをそれに渡します。
        * [SignResult](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature.domain/SignResult)の結果を分析して、必要に応じて新しく作成された署名を確認します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for Java APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        *オペレーティングシステム: Microsoft Windows、Linux、MacOS
        *開発環境: Visual Studio、Xamarin、MonoDevelop
        *フレームワーク: .NET Framework、.NET Standard、.NET Core、Mono
        * [NuGet](https://www.nuget.org/packages/groupdocs.signature)から最新バージョンのGroupDocs.SignatureforJavaをダウンロードします。
        
    code: |
        ```java
        Signature signature = new Signature("sample.xlsm"); 
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
         
        //パスワードを証明します
        options.setPassword("1234567890");
        //デジタル証明書の詳細
        options.setReason("Sign");
        options.setContact("JohnSmith");
        options.setLocation("Office1");
         
        //ドキュメントページに表示されるデジタル証明書としての画像
        options.setImageFilePath("sample.jpg");
        //
        options.setAllPages(true);
        options.setWidth(80);
        options.setHeight(60);
        options.setVerticalAlignment(VerticalAlignment.Bottom);
        options.setHorizontalAlignment(HorizontalAlignment.Right);
        Padding padding = new Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);
         
        SignResult signResult = signature.sign("signed.xlsm", options);
        //分析結果
        System.out.print("List of newly created signatures:");
        int number = 1;
        for(BaseSignature temp : signResult.getSucceeded())
        {
            System.out.print("Signature #"+ number++ +": Type: "+temp.getSignatureType()+" Id:"+temp.getSignatureId()+
                    ",Location: "+temp.getLeft()+"x"+temp.getTop()+". Size: "+temp.getWidth()+"x"+temp.getHeight());
        }
        ```
        
demos:
    enable: true
    title: "XLSM署名ライブデモを追加する"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、XLSMファイルの電子署名を今すぐ追加してください。
        ライブデモには次の利点があります
about_formats:
    enable: true
    format:
        - icon: "far fa-file-xlsm"
          title: "XLSMファイル形式とは"
          content: |
            XLSM拡張子の付いたファイルは、マクロをサポートするSpreasheetファイルの一種です。アプリケーションの観点からは、マクロはプロセスの自動化に使用される一連の命令です。マクロは、繰り返し実行されるステップを記録するために使用され、マクロを再度実行することによってアクションの実行を容易にします。マクロは、VisualBasicEditorを使用してExcelワークブック内からMicrosoftのVisualBasicfor Applications（VBA）でプログラムされ、そこから直接実行/デバッグできます。

          link: "https://docs.fileformat.com/spreadsheet/xlsm/"

more_formats:
    enable: false
    title: "その他の利用可能なオプション"
    content: |
        ドキュメントと画像用のマルチフォーマットデジタル署名API。以下に説明するように、一般的なファイル形式のいくつかに署名を追加します。
    format: 
          link: "/signature/java/add/pdf/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/java/add/doc/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/java/add/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/java/add/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/java/add/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/java/add/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/java/add/dotm/"
          description: "MicrosoftWordマクロ対応テンプレート"

          link: "/signature/java/add/rtf/"
          description: "リッチテキストドキュメント"

          link: "/signature/java/add/odt/"
          description: "ドキュメントテキストを開く"

          link: "/signature/java/add/ott/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/java/add/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/java/add/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/java/add/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/java/add/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/java/add/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/java/add/xltx/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/java/add/xltm/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/java/add/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/java/add/ots/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/java/add/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/java/add/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/java/add/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/java/add/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "/signature/java/add/potm/"
          description: "MicrosoftPowerPointマクロ対応テンプレート"

          link: "/signature/java/add/potx/"
          description: "MicrosoftPowerPointテンプレート"

          link: "/signature/java/add/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "/signature/java/add/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/java/add/otp/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/java/add/webp/"
          description: "WebP画像"

          link: "/signature/java/add/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/java/add/jpeg/"
          description: "JPEG画像"

          link: "/signature/java/add/gif/"
          description: "グラフィック交換フォーマット"

          link: "/signature/java/add/png/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/java/add/bmp/"
          description: "ビットマップファイル形式"

          link: "/signature/java/add/cdr/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/java/add/svg/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/java/add/psd/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/java/add/wmf/"
          description: "Windowsメタファイル"

          link: "/signature/java/add/emf/"
          description: "強化されたメタファイル形式"

          link: "/signature/java/add/cmx/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/java/add/djvu/"
          description: "既視感"

          link: "/signature/java/add/ppsm/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

          link: "/signature/java/add/dcm/"
          description: "医学におけるデジタルイメージングと通信"


back_to_top:
    enable: true
---
