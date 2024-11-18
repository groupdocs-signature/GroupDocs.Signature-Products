



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:11
draft: false
lang: ja
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "PythonアプリでXLSX文書に電子署名"
head_description: "Python APIを活用して、PDF、Wordファイル、Excelシート、プレゼンテーション、画像などのXLSX文書に電子署名を行い、安全性を確保します。"

############################# Header ############################
title: "XLSXを電子的に署名" 
description: "GroupDocs.Signature for Python via .NETを使用して、PDF、Word、Excel、プレゼンテーション、画像などの様々な文書に電子署名を埋め込み、コンプライアンスとデータの完全性を確保します。"
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料でダウンロード"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Python via .NET APIの概要"
    link: "/signature/python-net/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/)は文書に電子署名を追加するための完全なツールセットを提供します。署名、検索、検証、更新、またはデジタル署名の削除が必要な場合でも、GroupDocs.Signature for Python via .NETはPDF、Word文書、Excelシート、PowerPointプレゼンテーション、さまざまな画像形式など、複数のフォーマットで簡単に対応します。サードパーティのソフトウェアは不要です。

############################# Steps ############################
steps:
    enable: true
    title: "Pythonを使用してXLSXに電子署名を行う手順"
    content: |
      [GroupDocs.Signature](/signature/python-net/)を使用することで、Python via .NET開発者はXLSX文書に署名機能をシームレスに統合できます。カスタマイズした署名をアプリケーションに追加しましょう。
      
      1. SignatureインスタンスにXLSXファイルを読み込む。
      2. SignOptionsを使用して署名設定を構成する。
      3. サイズ、色、コンテンツなどの署名プロパティをカスタマイズする。
      4. 署名された文書を希望の場所に保存する。
   
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

            # Signatureインスタンスに文書を読み込む
            with sg.Signature('input.xlsx') as signature:

                # 新しいQrCodeSignOptionsオブジェクトを作成する
                options = sg.QrCodeSignOptions("QR code text")

                # すべての必要なオプションを設定する
                options.Left = 100
                options.Top = 100
                options.ForeColor = sg.Color.Red

                # 署名された文書をシステムに保存する
                result = signature.Sign("output.xlsx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "文書向けの高度な電子署名機能"
  description: "当社の電子署名APIは、署名、検証、変更、管理を効率的に行う方法を提供し、完全な自動化をサポートします。"
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "電子署名の機能"
  features:
    # feature loop
    - title: "オフィス文書に電子署名を行う"
      content: "電子署名を文書内の任意の場所に配置できます。デジタル証明書、バーコード、メタデータ、視覚要素でコンテンツをカスタマイズしながら、文書の安全性と信頼性を確保します。"

    # feature loop
    - title: "完全な署名管理"
      content: "文書に署名が行われると、すべての署名を表示して管理することができます。必要に応じて署名を更新または削除し、文書を完全に制御できます。"

    # feature loop
    - title: "文書のセキュリティを強化"
      content: "デジタル証明書で文書を保護します。メタデータを埋め込むか取得し、トラッキング、監査、コンプライアンスの向上を図り、コンテンツの信頼性を確保します。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "文書に画像署名を追加する方法"
      content: |
        この例では、文書の特定のページに画像署名を適用する方法を示します。
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg
        
          def run():

              # 署名する文書を読み込む
              with sg.Signature('input.xlsx') as signature:

                  # 署名オプションに画像のパスを設定する
                  options = sg.ImageSignOptions("image.jpg")

                  # ターゲットページ上の署名のサイズと配置を定義する
                  options.VerticalAlignment = sg.VerticalAlignment.Bottom
                  options.HorizontalAlignment = sg.HorizontalAlignment.Right
                  options.Height = 150
                  options.Width = 200
                  options.Margin = sg.Padding(50)
                  options.AllPages = True

                  # 署名を適用し、署名された文書を保存する
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
            link: "/examples/signature/formats/signature_esign.xlsx"
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
    title: "全機能セットを探る"
    exclude: "esign"
    description: "すべての電子署名ニーズに対応する幅広い署名オプションと操作を提供しています。"
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
    title: "幅広いファイルフォーマットに電子署名"
    exclude: "XLSX"
    description: "Python via .NET APIを使えば、60以上の業界標準フォーマットに電子署名が可能となり、ビジネス文書のセキュリティにおいて比類のない柔軟性を提供します。"
    items: 
          
        # format loop 1
        - name: "e-サイン PDF"
          format: "PDF"
          link: "/signature/python-net/esign/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "e-サイン DOCX"
          format: "DOCX"
          link: "/signature/python-net/esign/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "e-サイン JPEG"
          format: "JPEG"
          link: "/signature/python-net/esign/jpeg/"
          description: "JPEG 画像"
          
        # format loop 4
        - name: "e-サイン PPTX"
          format: "PPTX"
          link: "/signature/python-net/esign/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 5
        - name: "e-サイン XLSX"
          format: "XLSX"
          link: "/signature/python-net/esign/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---