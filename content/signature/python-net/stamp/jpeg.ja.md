



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:49
draft: false
lang: ja
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Pythonを使用してJPEGに円形および四角形のスタンプを作成"
head_description: "GroupDocs.Signature for Python via .NET APIを使用して、JPEGファイルにパーソナライズされたスタンプを生成して挿入します。"

############################# Header ############################
title: "JPEG用のスタンプを作成" 
description: "GroupDocs.Signature for Python via .NETを使用して、ドキュメントの任意の部分にカスタムデザインのスタンプを追加できます。ビジネスニーズに応じた配置と設定の柔軟性を提供します。"
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
    title: "GroupDocs.Signature for Python via .NETの概要"
    link: "/signature/python-net/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/)は、カスタムスタンプを含むさまざまな署名タイプを文書に挿入できる包括的なツールです。PDFやWord文書から画像、ZIPファイルまで、60以上のファイル形式をサポートしており、テキスト、画像、バーコード、メタデータ、デジタル証明書、スタンプでドキュメントを強化できます。適用された署名を検索、確認、編集、削除するための完全なコントロールも備えています。

############################# Steps ############################
steps:
    enable: true
    title: "Pythonを使用してJPEGにスタンプを追加する方法"
    content: |
      [GroupDocs.Signature](/signature/python-net/)は、Python via .NETアプリケーションを強化するための堅牢なスタンプ作成ツールを提供します。これを使用して、文書ページ用のカスタムスタンプを設計および実装します。
      
      1. JPEG文書をスタンプするために提供してください。
      2. StampSignOptionsを使用して、必要な設定をすべて構成します。
      3. 必要に応じて複数のスタンプ行を追加します。
      4. スタンプを適用し、更新された文書を保存します。
   
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

            # Signatureインスタンスに文書パスを添付
            with sg.Signature('input.jpeg') as signature:

                # 必要なスタンプの詳細を設定するためにStampSignOptionsを設定
                options = sg.StampSignOptions()
                options.Height = 180
                options.Width = 180

                # スタンプに1行以上を追加
                outerLine = sg.StampLine()
                outerLine.Text = "* The Best Company *"
                outerLine.TextRepeatType = sg.StampTextRepeatType.FullTextRepeat
                outerLine.Font = sg.SignatureFont()
                outerLine.Font.Size = 12
                outerLine.Font.FamilyName = "Arial"
                outerLine.Height = 22
                outerLine.TextBottomIntent = 6
                outerLine.TextColor = sg.Color.WhiteSmoke
                outerLine.BackgroundColor = sg.Color.DarkSlateBlue
                options.OuterLines.Add(outerLine)

                # 適用されたスタンプで文書を保存
                result = signature.Sign("output.jpeg", options)
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "署名を使用して文書の整合性を確保および向上"
  description: "GroupDocs.Signature for Python via .NETライブラリを使用すると、ドキュメントに署名機能をシームレスに追加できます。カスタムスタンプやその他の署名タイプを作成、変更、確認、削除することができ、文書ワークフローに柔軟性とセキュリティを提供します。"
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "GroupDocs.Signatureによるスタンプ署名"
  features:
    # feature loop
    - title: "完全な文書署名"
      content: "テキスト、画像、バーコード、QRコード、スタンプなどの署名を任意のページの任意の位置に追加して、ドキュメントを向上させましょう。埋め込まれたメタデータを管理し、不正変更から保護するためにデジタル証明書を適用できます。"

    # feature loop
    - title: "効率的な署名検索と確認"
      content: "署名後、先進的な検索ツールを使用して、すべての埋め込まれた署名を見つけてください。文書の整合性を確保するために、署名データを簡単に確認または管理できます。"

    # feature loop
    - title: "署名の編集とカスタマイズ"
      content: "以前に追加した署名に変更を加えることができます。コンテンツ、位置、サイズ、または色を変更したい場合でも、GroupDocs.Signature for Python via .NETは必要に応じて署名を調整するための完全なコントロールを提供します。"

    # feature loop
    - title: "署名を簡単に削除"
      content: "署名を削除する必要がある場合は、GroupDocs.Signature for Python via .NETがスタンプやデジタル証明書を含む任意のタイプを削除するために必要なすべてのツールを提供して、ドキュメントを最新かつ準拠させることができます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "文書にカスタムスタンプを追加する方法"
      content: |
        この例では、特定のテキスト詳細を含むカスタムスタンプを作成して文書に挿入する方法を示します。
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # スタンプする文書を提供します
              with sg.Signature('input.jpeg') as signature:

                    # 希望の設定でスタンプオプションを設定します
                    options = sg.StampSignOptions()

                    # スタンプのサイズとページ上の配置を定義します
                    options.Height = 200
                    options.Width = 200
                    options.VerticalAlignment = sg.VerticalAlignment.Bottom
                    options.HorizontalAlignment = sg.HorizontalAlignment.Right
                    options.AllPages = True

                    # テキストを含む外側の円形ラインを追加します
                    outerLine = sg.StampLine()
                    outerLine.Text = "* The best  choice *"
                    outerLine.TextRepeatType = sg.StampTextRepeatType.FullTextRepeat
                    outerLine.Font = sg.SignatureFont()
                    outerLine.Font.Size = 12
                    outerLine.Font.FamilyName = "Arial"
                    outerLine.Height = 22
                    outerLine.TextBottomIntent = 6
                    outerLine.TextColor = sg.Color.WhiteSmoke
                    outerLine.BackgroundColor = sg.Color.DarkSlateBlue
                    options.OuterLines.Add(outerLine)

                    # 必要に応じて、内側の四角形のラインも追加します
                    innerLine = sg.StampLine()
                    innerLine.Text = "Company #1"
                    innerLine.TextColor = sg.Color.MediumVioletRed
                    innerLine.Font = sg.SignatureFont()
                    innerLine.Font.Size = 20
                    innerLine.Font.Bold = True
                    innerLine.Height = 40
                    options.InnerLines.Add(innerLine)

                    # スタンプを施した文書を最終化して保存します
                    result = signature.Sign("output.jpeg", options)
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
            link: "/examples/signature/formats/signature_stamp.jpeg"
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
    title: "主要な機能を探る"
    exclude: "stamp"
    description: "署名を作成、管理、削除するための幅広いオプションを見つけ、文書ワークフローを完全に制御することができます。"
    items: 
          
        # operation loop 1
        - name: "電子署名"
          operation: "esign"
          link: "/signature/python-net/esign/jpeg/"
          description: "対応ファイル形式にさまざまな種類の署名を追加"

        # operation loop 2
        - name: "ドキュメントにテキストを追加"
          operation: "text"
          link: "/signature/python-net/text/jpeg/"
          description: "カスタマイズ可能なテキスト署名でドキュメントの内容を強化"

        # operation loop 3
        - name: "画像署名"
          operation: "image"
          link: "/signature/python-net/image/jpeg/"
          description: "ドキュメントの任意の位置に任意の画像を配置"

        # operation loop 4
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/signature/python-net/barcode/jpeg/"
          description: "対応ドキュメントにさまざまなバーコードを作成して挿入"

        # operation loop 5
        - name: "QR コードを生成"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "ドキュメント署名用の QR コードを生成"
          
        # operation loop 6
        - name: "デジタル証明書"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "ビジネスを保護し、デジタル証明書で文書を署名"

        # operation loop 7
        - name: "スタンプ署名"
          operation: "stamp"
          link: "/signature/python-net/stamp/jpeg/"
          description: "スタンプコンストラクタを使用してカスタム円形または角形のスタンプを作成"
          
        # operation loop 8
        - name: "署名を検索"
          operation: "search"
          link: "/signature/python-net/search/pdf/"
          description: "ドキュメント内の以前に追加した署名を見つける"
          
        # operation loop 9
        - name: "署名の検証"
          operation: "verify"
          link: "/signature/python-net/verify/pdf/"
          description: "署名が適用された後に、その真正性を検証"
          
        # operation loop 10
        - name: "署名を修正"
          operation: "modify"
          link: "/signature/python-net/modify/pdf/"
          description: "ドキュメント内のさまざまな署名を簡単に編集"
          
        # operation loop 11
        - name: "署名を削除"
          operation: "delete"
          link: "/signature/python-net/delete/pdf/"
          description: "以前に適用した多くの署名を削除"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "さまざまな文書形式にスタンプを適用"
    exclude: "JPEG"
    description: "GroupDocs.Signature APIを使用すると、60以上の標準ファイルタイプにカスタムスタンプを挿入できます。文書内の任意の場所にスタンプを簡単に適用し、パーソナライズと追跡を向上させることができます。"
    items: 
          
        # format loop 1
        - name: "PDF にスタンプ"
          format: "PDF"
          link: "/signature/python-net/stamp/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "DOCX にスタンプ"
          format: "DOCX"
          link: "/signature/python-net/stamp/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "JPEG にスタンプ"
          format: "JPEG"
          link: "/signature/python-net/stamp/jpeg/"
          description: "JPEG 画像"
          
        # format loop 4
        - name: "PPTX にスタンプ"
          format: "PPTX"
          link: "/signature/python-net/stamp/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 5
        - name: "XLSX にスタンプ"
          format: "XLSX"
          link: "/signature/python-net/stamp/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---