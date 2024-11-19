



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:22
draft: false
lang: ja
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Pythonを使用してPPTXファイル用のQRコードを生成"
head_description: "GroupDocs.Signature APIを使用してPPTXファイルにQRコードを生成および埋め込む。どのページにもQRコードを簡単に配置して追加機能を提供。"

############################# Header ############################
title: "PPTX用のQRコードを生成" 
description: "テキストまたは数値データを使用して2Dバーコードを効果的に作成し、PDF、Word、Excelなどのさまざまなページおよび形式に適用できるGroupDocs.Signature for Python via .NET。"
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料トライアル"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Python via .NETの機能を探る"
    link: "/signature/python-net/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/)は、ユーザーが主要な文書形式全体でさまざまな署名タイプを生成および埋め込むことを可能にする幅広い機能を提供します。PDF、Word、Excel、PowerPoint、または画像であろうと、テキスト、画像、バーコード、QRコード、メタデータ、デジタル、またはスタンプ署名で文書を強化してください。

############################# Steps ############################
steps:
    enable: true
    title: "PPTXにQRコードを生成および挿入する手順"
    content: |
      [GroupDocs.Signature](/signature/python-net/)を使用すると、一般的な形式でQRコードを作成し、PPTXのページに配置できます。10種類以上のQRコードタイプをサポートしているため、Python via .NETアプリケーションにこの機能をシームレスに統合できます。私たちの製品を使用してQRコード署名で文書を強化してください。
      
      1. PPTXファイルまたはQRコードを追加するストリームを取得します。
      2. QrCodeSignOptionsに必要なテキストを提供します。
      3. 色、位置、サイズなどの視覚設定をカスタマイズします。
      4. QRコードを埋め込んだ文書を保存します。
   
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

            # 文書で新しいSignatureインスタンスを初期化
            with sg.Signature('input.pptx') as signature:

                # QrCodeSignOptionsを使用して文書にQRコードを埋め込む
                options = sg.QrCodeSignOptions("Text Content")

                # 署名タイプを指定し、ページ上の位置を設定
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 50
                options.Top = 150

                # QRコードを埋め込んだ文書を保存
                result = signature.Sign("output.pptx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "文書用の完全な署名統合"
  description: "GroupDocs.Signature for Python via .NET APIを使用すると、ユーザーはさまざまな署名タイプを生成、変更、検索、検証、削除でき、文書のワークフローを正確に簡素化します。"
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "GroupDocs.Signatureの主要機能"
  features:
    # feature loop
    - title: "複数の署名タイプを適用"
      content: "GroupDocs.Signatureでは、テキスト、画像、バーコード、QRコード、およびスタンプ署名を任意の文書に適用できます。署名を任意のページに正確に配置し、メタデータを簡単に管理できます。デジタル証明書を使用して、未承認の変更から文書を保護します。"

    # feature loop
    - title: "署名を検索および検証"
      content: "高度な検証ツールを使用して、文書の署名が正当であるかどうかを確認します。文書に埋め込まれたすべての署名の詳細リストを簡単に取得し、より良い監視を行います。"

    # feature loop
    - title: "既存の署名を変更"
      content: "適用済みの署名を、コンテンツ、位置、色、サイズなどの属性を調整して特定のニーズに合わせて更新できます。"

    # feature loop
    - title: "署名を簡単に削除"
      content: "不要な署名を迅速に削除して文書管理を簡素化します。デジタル証明書や他の署名タイプでも、効率的な削除が可能です。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "生成されたQRコードをカスタマイズ"
      content: |
        この例では、PPTXページにカスタマイズされたQRコードを配置する方法を示しています。
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # 署名する文書を取得し、Signatureに渡します。
              with sg.Signature('input.pptx') as signature:

                    # 必要なテキストを使用してQRコードオプションを設定します。
                    options = sg.QrCodeSignOptions("Archived on July 11, 2019")

                    # QRコードのページ上の位置を設定します。
                    options.VerticalAlignment = sg.Domain.VerticalAlignment.Top
                    options.HorizontalAlignment = sg.Domain.HorizontalAlignment.Right

                    # 署名のパディングを設定します。
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # QRコードの色を選択します。
                    options.ForeColor = sg.Color.Red

                    # メッセージのフォントオプションを定義します。
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # QRコードの背景色とブラシを設定します。
                    options.Background = sg.Background()
                    options.Background.Color = Color.LimeGreen
                    options.Background.Transparency = 0.5
                    options.Background.Brush = sg.LinearGradientBrush(sg.Color.LimeGreen, sg.Color.DarkGreen)

                    # QRコードを文書に埋め込みます。
                    result = signature.Sign("output.pptx", options)
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
            link: "/examples/signature/formats/signature_qrcode.pptx"
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
    title: "私たちの署名ソリューションを探る"
    exclude: "qrcode"
    description: "私たちは、文書ニーズを満たすための多様な署名タイプと操作を提供します。"
    items: 
          
        # operation loop 1
        - name: "電子署名"
          operation: "esign"
          link: "/signature/python-net/esign/pptx/"
          description: "対応ファイル形式にさまざまな種類の署名を追加"

        # operation loop 2
        - name: "ドキュメントにテキストを追加"
          operation: "text"
          link: "/signature/python-net/text/pptx/"
          description: "カスタマイズ可能なテキスト署名でドキュメントの内容を強化"

        # operation loop 3
        - name: "画像署名"
          operation: "image"
          link: "/signature/python-net/image/pptx/"
          description: "ドキュメントの任意の位置に任意の画像を配置"

        # operation loop 4
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/signature/python-net/barcode/pptx/"
          description: "対応ドキュメントにさまざまなバーコードを作成して挿入"

        # operation loop 5
        - name: "QR コードを生成"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/pptx/"
          description: "ドキュメント署名用の QR コードを生成"
          
        # operation loop 6
        - name: "デジタル証明書"
          operation: "digital"
          link: "/signature/python-net/digital/pptx/"
          description: "ビジネスを保護し、デジタル証明書で文書を署名"

        # operation loop 7
        - name: "スタンプ署名"
          operation: "stamp"
          link: "/signature/python-net/stamp/pptx/"
          description: "スタンプコンストラクタを使用してカスタム円形または角形のスタンプを作成"
          
        # operation loop 8
        - name: "署名を検索"
          operation: "search"
          link: "/signature/python-net/search/pptx/"
          description: "ドキュメント内の以前に追加した署名を見つける"
          
        # operation loop 9
        - name: "署名の検証"
          operation: "verify"
          link: "/signature/python-net/verify/pptx/"
          description: "署名が適用された後に、その真正性を検証"
          
        # operation loop 10
        - name: "署名を修正"
          operation: "modify"
          link: "/signature/python-net/modify/pptx/"
          description: "ドキュメント内のさまざまな署名を簡単に編集"
          
        # operation loop 11
        - name: "署名を削除"
          operation: "delete"
          link: "/signature/python-net/delete/pptx/"
          description: "以前に適用した多くの署名を削除"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "さまざまな文書形式にQRコードを埋め込む"
    exclude: "PPTX"
    description: "Python via .NET APIを使用して、業界標準の文書形式にQRコードを埋め込みます。重要な情報を2Dバーコードに保存してエンコードし、スキャンとデータ取得を容易にします。"
    items: 
          
        # format loop 1
        - name: "QRコード for PDF"
          format: "PDF"
          link: "/signature/python-net/qrcode/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "QRコード for DOCX"
          format: "DOCX"
          link: "/signature/python-net/qrcode/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "QRコード for JPEG"
          format: "JPEG"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "JPEG 画像"
          
        # format loop 4
        - name: "QRコード for PPTX"
          format: "PPTX"
          link: "/signature/python-net/qrcode/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 5
        - name: "QRコード for XLSX"
          format: "XLSX"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---