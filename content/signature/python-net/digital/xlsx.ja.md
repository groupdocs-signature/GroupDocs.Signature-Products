



---
############################# Static ############################
layout: "format"
date:  2024-11-20T08:57:23
draft: false
lang: ja
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Pythonを使用してXLSXにデジタル署名を作成"
head_description: "Pythonを使用してXLSXドキュメントにデジタル署名を追加するための数行のコードで実現できます。GroupDocs.Signature for Python via .NETを使用して、さまざまなファイル形式に署名しましょう。"

############################# Header ############################
title: "XLSXにデジタル署名" 
description: "GroupDocs.Signature for Python via .NETを介してデジタル証明書を適用することで、ドキュメントのセキュリティと信頼性を確保します。当社のソリューションにより、強力なツールを使用してドキュメントに署名したり、保護したりできます。"
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料で入手"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Python via .NETとは？"
    link: "/signature/python-net/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/)は、幅広いドキュメント処理タスクをサポートする包括的な署名ツールです。テキスト、画像、デジタル証明書、スタンプを60以上のファイル形式（PDF、MS Officeファイル、画像、ZIPなど）に追加できます。GroupDocs.Signature for Python via .NETを使用すると、必要に応じて署名を検索、検証、更新、または削除することも可能です。

############################# Steps ############################
steps:
    enable: true
    title: "Pythonでのデジタル証明書によるXLSXの保護方法"
    content: |
      [GroupDocs.Signature](/signature/python-net/)は、Python via .NET開発者がデジタル署名を追加してXLSXファイルを保護するのを支援します。堅牢なドキュメント保護機能で、ビジネスアプリケーションを強化しましょう。
      
      1. SignatureクラスにXLSXファイルをロードします。
      2. デジタル証明書とそのパスワードを適用して、ファイルを保護します。
      3. オプションで、ドキュメントページにデジタル署名のビジュアル表示を追加します。
      4. 文書に署名して、無許可の変更を防ぎます。
   
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

            # Signatureを使用してドキュメントにデジタル署名を行います
            with sg.Signature('input.xlsx') as signature:

                # デジタル証明書とそのパスワードを入力してください
                options = sg.DigitalSignOptions("certificate.pfx")
                options.Password = "1234567890"

                # オプションとして、署名の表示方法を設定します
                options.PageNumber = 1
                options.Left = 50
                options.Top = 50

                # デジタル証明書でドキュメントを最終化します
                result = signature.Sign("output.xlsx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "デジタル署名を使用してドキュメントを強化し、保護"
  description: "GroupDocs.Signature for Python via .NETライブラリは、すべての主要なファイル形式に署名するように設計されています。異なる種類の署名を簡単に追加、検証、更新、削除することで、ワークフローを簡素化します。"
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "GroupDocs.Signatureのコア機能"
  features:
    # feature loop
    - title: "ドキュメントに署名を追加"
      content: "サポートされているドキュメントの任意の位置に、テキスト、画像、バーコード、QRコード、またはスタンプ署名を正確に挿入します。また、画像のEXIFなど隠れたメタデータを管理して、デジタル署名によるドキュメントの完全性を保証できます。"

    # feature loop
    - title: "署名を検証および検索"
      content: "署名後、文書を簡単に検証して正しい処理を確認できます。強力な検索機能を使用して、ファイル内のすべての署名を取得し、管理できます。"

    # feature loop
    - title: "既存の署名を編集"
      content: "ほとんどの署名は完全にカスタマイズ可能です。テキストを編集したり、要素を移動したり、色を変更したり、サイズを調整したりして、ニーズに合わせることができます。"

    # feature loop
    - title: "不要な署名を削除"
      content: "当社のソリューションは、署名管理を完全にサポートし、必要に応じて任意のドキュメントから署名やデジタル証明書を削除できます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "デジタル署名でドキュメントを保護"
      content: |
        デジタル署名を適用してドキュメントを保護し、無許可変更を防ぐ方法を学びます。
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # 署名するドキュメントをロードします
              with sg.Signature('input.xlsx') as signature:

                  # 有効なデジタル証明書とそれに対応するパスワードを使用します
                  options = sg.DigitalSignOptions("certificate.pfx")
                  options.Password = "1234567890"

                  # 必要に応じて追加のテキスト情報を追加します
                  options.Reason = "Security issue"
                  options.Contact = "John Smith"
                  options.Location = "Office D.W."

                  # 署名のビジュアル表現には画像やその他のオプションを含めます
                  options.ImageFilePath = "image.png"
                  options.AllPages = True
                  options.VerticalAlignment = sg.VerticalAlignment.Center
                  options.HorizontalAlignment = sg.HorizontalAlignment.Left
                  options.Width = 60
                  options.Height = 80

                  options.Margin = sg.Padding()
                  options.Margin.Bottom = 10
                  options.Margin.Right = 10

                  # 署名済みのドキュメントを安全な場所に保存します
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
            link: "/examples/signature/formats/signature_digital.xlsx"
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
    title: "主要機能を探索"
    exclude: "digital"
    description: "さまざまな署名オプションと強力なドキュメント操作を提供しています。"
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
    title: "複数形式のドキュメントに署名"
    exclude: "XLSX"
    description: "Python via .NET APIを使用することで、60以上の異なる形式を処理し、署名を追加し、セキュリティのためにデジタル証明書を適用し、さまざまなページで署名を管理できます。"
    items: 
          
        # format loop 1
        - name: "PDF を保護"
          format: "PDF"
          link: "/signature/python-net/digital/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "DOCX を保護"
          format: "DOCX"
          link: "/signature/python-net/digital/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "PPTX を保護"
          format: "PPTX"
          link: "/signature/python-net/digital/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 4
        - name: "XLSX を保護"
          format: "XLSX"
          link: "/signature/python-net/digital/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---