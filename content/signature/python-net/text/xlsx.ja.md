



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:15
draft: false
lang: ja
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Pythonを使用してXLSXにテキスト署名を追加"
head_description: "Python APIを活用して、PDF、Word、Excel、PowerPoint、画像、ZIPなどのフォーマットをサポートするXLSXファイルにテキストベースの署名を埋め込む。"

############################# Header ############################
title: "XLSXにテキスト署名を追加" 
description: "GroupDocs.Signature for Python via .NETを使用して、ドキュメントにカスタムテキスト署名をシームレスに統合します。柔軟な署名カスタマイズオプションでワークフローを簡素化。"
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "今すぐ無料で試してみる"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Python via .NETの力を探る"
    link: "/signature/python-net/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/)は、カスタマイズ可能なテキスト署名を埋め込むための包括的なプラットフォームを提供し、文書ワークフローをスムーズにします。文書全体で署名の内容と外観をパーソナライズして、効率を高め、文書管理を向上させます。

############################# Steps ############################
steps:
    enable: true
    title: "Pythonを使用してXLSXテキスト署名を作成する方法"
    content: |
      [GroupDocs.Signature](/signature/python-net/)は、Python via .NETアプリケーション内のXLSXファイルにおける簡単なテキスト署名の統合を可能にします。このソリューションで製品に機能を追加します。
      
      1. SignatureコンストラクタにXLSXドキュメントを提供。
      2. 署名テキストでTextSignOptionsを作成。
      3. 署名の視覚的特性を設定。
      4. ドキュメントの希望するページに署名を挿入。
   
    code:
      platform: "python-net"
      copy_title: "コピー"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "サンプル署名"
      install:
        command: "pip install groupdocs-signature-net"
        copy_tip: "クリックしてコピー"
        copy_done: "コピーしました"
      links:
        #  loop
        - title: "さらなる例"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
        #  loop
        - title: "ドキュメント"
          link: "https://docs.groupdocs.com/signature/python-net/"
          
      content: |
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Signatureをドキュメントパスで初期化
            with sg.Signature('input.xlsx') as signature:

                # 希望する署名テキストでTextSignOptionsを設定
                options = sg.TextSignOptions("Approved")

                # 署名の色とフォントを選択
                options.ForeColor = sg.Color.Red
                options.Font = sg.SignatureFont()
                options.Font.Size = 12
                options.Font.FamilyName = "Comic Sans MS"

                # ドキュメントにテキスト署名を適用
                result = signature.Sign("output.xlsx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "完全なテキスト署名管理"
  description: "GroupDocs.Signature for Python via .NETは、一般的なフォーマットにカスタムテキスト署名を追加することで、文書ワークフローを管理するのに役立ちます。署名の外観、配置、および内容を必要に応じて簡単に制御できます。"
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "GroupDocs.Signatureの機能を発見"
  features:
    # feature loop
    - title: "柔軟な文書署名"
      content: "テキスト、画像、バーコード、QRコード、スタンプなど、さまざまな署名タイプを任意の文書ページに追加します。メタデータを使用して隠れた情報を含め、デジタル証明書でファイルを保護します。"

    # feature loop
    - title: "署名の検証と検索"
      content: "高度なツールを使用して、署名された文書の完全性を確認します。ファイル内のすべての署名を検索および分析してさらなる検証を行います。"

    # feature loop
    - title: "署名の編集または削除"
      content: "既存の署名の内容、外観、または配置を簡単に更新します。最新の文書を維持するために古い署名を削除します。"

    # feature loop
    - title: "特化したテキスト署名"
      content: "Wordファイル用の透かしやPDF用のスタンプなど、文書特有のテキスト署名を適用して、さらなる制御とカスタマイズを加えます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "ドキュメントにテキスト署名を追加"
      content: |
        プロセスを効率化するためにドキュメントにテキスト署名を埋め込む方法を学びます。
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # 署名する文書を選択
              with sg.Signature('input.xlsx') as signature:

                    # 希望する内容でテキストオプションを設定
                    options = sg.TextSignOptions("Rescheduled to 03/04/2025")

                    # 署名のサイズと配置を定義
                    options.Left = 100
                    options.Top = 180
                    options.Width = 230
                    options.Height = 30

                    # ページの端からの余白を設定
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # テキストの色とフォントスタイルを選択
                    options.ForeColor = sg.Color.Red
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # テキスト署名の周りに境界線を追加
                    options.Border = sg.Border()
                    options.Border.Color = sg.Color.Red
                    options.Border.DashStyle = sg.DashStyle.DashLongDashDot
                    options.Border.Transparency = 0.5
                    options.Border.Visible = True
                    options.Border.Weight = 2

                    # 必要に応じて背景をカスタマイズ
                    options.Background = sg.Background()
                    options.Background.Color = sg.Color.Yellow
                    options.Background.Transparency = 0.8

                    # 互換性のために署名を画像として保存するオプション
                    options.SignatureImplementation = sg.TextSignatureImplementation.Image

                    # 埋め込まれた署名を持つ文書を保存
                    result = signature.Sign("output.xlsx", options)
          ```
        platform: "python-net"
        copy_title: "コピー"
        install:
          command: "pip install groupdocs-signature-net"
          copy_tip: "クリックしてコピー"
          copy_done: "コピーしました"
        top_links:
          #  loop
          - title: "結果をダウンロード"
            icon: "download"
            link: "/examples/signature/formats/signature_text.xlsx"
        links:
          #  loop
          - title: "さらなる例"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
          #  loop
          - title: "ドキュメント"
            link: "https://docs.groupdocs.com/signature/python-net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "始める準備はできましたか？"
  description: "GroupDocs.Signature の機能を無料で試すか、ライセンスをリクエストしてください"
  items:
    #  loop
    - title: "PyPi ダウンロード"
      link: "https://releases.groupdocs.com/signature/python-net/"
      color: "red"
        #  loop
    - title: "ライセンス"
      link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "高度な署名機能"
    exclude: "text"
    description: "当社のAPIは、7つの署名タイプの完全なライフサイクル管理をサポートしており、署名を作成、管理、検証、カスタマイズできます。"
    items: 
          
        # operation loop 1
        - name: "電子署名"
          operation: "esign"
          link: "/signature/python-net/esign/xlsx/"
          description: "対応ファイル形式にさまざまな種類の署名を追加"

        # operation loop 2
        - name: "ドキュメントにテキストを追加"
          operation: "text"
          link: "/signature/python-net/text/xlsx/"
          description: "カスタマイズ可能なテキスト署名でドキュメントの内容を強化"

        # operation loop 3
        - name: "画像署名"
          operation: "image"
          link: "/signature/python-net/image/xlsx/"
          description: "ドキュメントの任意の位置に任意の画像を配置"

        # operation loop 4
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/signature/python-net/barcode/xlsx/"
          description: "対応ドキュメントにさまざまなバーコードを作成して挿入"

        # operation loop 5
        - name: "QR コードを生成"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "ドキュメント署名用の QR コードを生成"
          
        # operation loop 6
        - name: "デジタル証明書"
          operation: "digital"
          link: "/signature/python-net/digital/xlsx/"
          description: "ビジネスを保護し、デジタル証明書で文書を署名"

        # operation loop 7
        - name: "スタンプ署名"
          operation: "stamp"
          link: "/signature/python-net/stamp/xlsx/"
          description: "スタンプコンストラクタを使用してカスタム円形または角形のスタンプを作成"
          
        # operation loop 8
        - name: "署名を検索"
          operation: "search"
          link: "/signature/python-net/search/xlsx/"
          description: "ドキュメント内の以前に追加した署名を見つける"
          
        # operation loop 9
        - name: "署名の検証"
          operation: "verify"
          link: "/signature/python-net/verify/xlsx/"
          description: "署名が適用された後に、その真正性を検証"
          
        # operation loop 10
        - name: "署名を修正"
          operation: "modify"
          link: "/signature/python-net/modify/xlsx/"
          description: "ドキュメント内のさまざまな署名を簡単に編集"
          
        # operation loop 11
        - name: "署名を削除"
          operation: "delete"
          link: "/signature/python-net/delete/xlsx/"
          description: "以前に適用した多くの署名を削除"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "複数のフォーマットにテキスト署名を埋め込む"
    exclude: "XLSX"
    description: "Python via .NET APIを使用して、さまざまなOffice文書にテキスト署名を追加し、文書ライフサイクルを完全に管理し、セキュリティを向上させることができます。"
    items: 
          
        # format loop 1
        - name: "PDF テキスト署名"
          format: "PDF"
          link: "/signature/python-net/text/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "DOCX テキスト署名"
          format: "DOCX"
          link: "/signature/python-net/text/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "JPEG テキスト署名"
          format: "JPEG"
          link: "/signature/python-net/text/jpeg/"
          description: "JPEG 画像"
          
        # format loop 4
        - name: "PPTX テキスト署名"
          format: "PPTX"
          link: "/signature/python-net/text/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 5
        - name: "XLSX テキスト署名"
          format: "XLSX"
          link: "/signature/python-net/text/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---