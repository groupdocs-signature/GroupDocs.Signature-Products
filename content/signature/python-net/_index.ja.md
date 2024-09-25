---
############################# Static ############################
layout: "landing"
date: 2024-09-25T13:59:03
draft: false

lang: ja
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java" 
    # supported_platforms loop
    - title: "Python"
      tag: "python-net"  

############################# Head ############################
head_title: "{index-content-python-net.head_title}"
head_description: "{index-content-python-net.head_description}"

############################# Header ############################
title: "{index-content-python-net.title}"
description: "{index-content-python-net.description}"
words:
  for: "のために"

actions:
  main: "{index-content-python-net.actions_main}"
  main_link: "https://pypi.org/project/groupdocs-signature-net/"
  alt: "ライセンス"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
  title: "始める準備はできていますか?"
  description: "GroupDocs.Signature 機能を無料で試すか、ライセンスをリクエストしてください"

release:
  title: "バージョン {0} がリリースされました"
  notes: "新機能を見る"
  downloads: "ダウンロード"

code:
  title: "{index-content-python-net.code_title}"
  more: "他の例"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
  install: "pip install groupdocs-signature-net"
  content: |
    ```python {style=abap}   
    import groupdocs.signature as sg

    def run():

        # PDFドキュメントを選択
        with sg.Signature('sample.pdf') as signature:

            # テキストを提供する
            options = sg.TextSignOptions("John Smith")
    
            # 色を設定する
            options.ForeColor = sg.Color.Red
    
            # 文書に署名してファイルに保存
            signature.Sign('signed.pdf', options)
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature の概要"
  description: "{index-content-python-net.overview_description}"
  features:
    # feature loop
    - title: "{index-content-python-net.overview_feature_1.title}"
      content: "{index-content-python-net.overview_feature_1.description}"

    # feature loop
    - title: "{index-content-python-net.overview_feature_2.title}"
      content: "{index-content-python-net.overview_feature_2.description}"

    # feature loop
    - title: "{index-content-python-net.overview_feature_3.title}"
      content: "{index-content-python-net.overview_feature_3.description}"

############################# Platforms ############################
platforms:
  enable: true
  title: "プラットフォームの独立性"
  description: "{index-content-python-net.platforms_description}"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "サポートされているファイル形式"
  description: |
    {index-content-python-net.formats_description}
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office形式
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### 画像とその他の形式
        * **ポータブル:** PDF
        * **画像:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **その他のオフィス形式:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### その他のフォーマット
        * **ウェブ:** HTML, MHTML
        * **アーカイブ:** ZIP, TAR, 7Z
        * **証明書:** PFX

############################# Features ############################
features:
  enable: true
  title: "{index-content-python-net.features.title}"
  description: "{index-content-python-net.features.description}"

  items:
    # feature loop
    - icon: "sign"
      title: "{index-content-python-net.features.feature_1.title}"
      content: "{index-content-python-net.features.feature_1.content}"

    # feature loop
    - icon: "custom"
      title: "{index-content-python-net.features.feature_2.title}"
      content: "{index-content-python-net.features.feature_2.content}"

    # feature loop
    - icon: "password"
      title: "{index-content-python-net.features.feature_3.title}"
      content: "{index-content-python-net.features.feature_3.content}"

    # feature loop
    - icon: "protect"
      title: "{index-content-python-net.features.feature_4.title}"
      content: "{index-content-python-net.features.feature_4.content}"

    # feature loop
    - icon: "convert"
      title: "{index-content-python-net.features.feature_5.title}"
      content: "{index-content-python-net.features.feature_5.content}"

    # feature loop
    - icon: "preview"
      title: "{index-content-python-net.features.feature_6.title}"
      content: "{index-content-python-net.features.feature_6.content}"

    # feature loop
    - icon: "search"
      title: "{index-content-python-net.features.feature_7.title}"
      content: "{index-content-python-net.features.feature_7.content}"

    # feature loop
    - icon: "validate"
      title: "{index-content-python-net.features.feature_8.title}"
      content: "{index-content-python-net.features.feature_8.content}"

    # feature loop
    - icon: "update"
      title: "{index-content-python-net.features.feature_9.title}"
      content: "{index-content-python-net.features.feature_9.content}"

############################# Code samples ############################
code_samples:
  enable: true
  title: "コードサンプル"
  description: "{index-content-python-net.code_samples_description}"
  items:
    # code sample loop
    - title: "{index-content-python-net.code_title_sample_1}"
      content: |
        {index-content-python-net.code_samples_sample_1_content_1} {index-content-python-net.code_samples_sample_1_content_2}
        {{< landing/code title="QRコードをPDFに貼り付ける方法。">}}
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # 署名する文書をロードします
            with sg.Signature('file_to_sign.pdf') as signature:

                # 事前定義されたテキストを使用して QR コード オプションを作成する
                options = sg.QrCodeSignOptions('The document is approved by John Smith')
        
                # QRコードのエンコードタイプとページ上の位置を設定する
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 100
                options.Top = 100
            
                # 文書に署名し、結果ファイルとして保存します
                signature.Sign('file_with_QR.pdf', options)
        ```
        {{< /landing/code >}}

    # code sample loop
    - title: "{index-content-python-net.code_title_sample_2}"
      content: |
        {index-content-python-net.code_samples_sample_2_content_1} {index-content-python-net.code_samples_sample_2_content_2}
        {{< landing/code title="文書の整合性を確保する方法は次のとおりです。">}}
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # デジタル署名する文書をロードします
            with sg.Signature('file_to_sign.docx') as signature:
        
                # デジタル署名オプションを指定し、証明書ファイルへのパスを指定します。
                options = sg.DigitalSignOptions('certificate.pfx')

                # 証明書のパスワードを設定する
                options.Password = '1234567890'

                # 文書に署名し、目的のパスに保存します
                signature.Sign('digitally_signed.docx', options)
        ```
        {{< /landing/code >}}

---
