



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:23
draft: false
lang: zh
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "使用Python为PPTX文件生成二维码"
head_description: "使用GroupDocs.Signature API生成并嵌入二维码到PPTX文件中。将二维码轻松放置在任何页面上，以添加额外的功能。"

############################# Header ############################
title: "为PPTX生成二维码" 
description: "使用文本或数字数据轻松创建2D条形码，并将其应用于各种页面和格式，包括PDF、Word、Excel等，使用GroupDocs.Signature for Python via .NET。"
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费试用"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "探索GroupDocs.Signature for Python via .NET的功能"
    link: "/signature/python-net/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) 提供广泛的能力，使用户能够在主要文档格式中生成并嵌入不同类型的签名。无论是PDF、Word、Excel、PowerPoint还是图片，通过文本、图片、条形码、二维码、元数据、数字或印章签名来增强您的文档。

############################# Steps ############################
steps:
    enable: true
    title: "在PPTX中生成和插入二维码的步骤"
    content: |
      [GroupDocs.Signature](/signature/python-net/) 使您能够在流行格式中创建二维码，并将其放置在PPTX页面上。支持超过10种二维码类型，您可以无缝将此功能集成到Python via .NET应用程序中。使用我们的产品，通过二维码签名增强您的文档。
      
      1. 获取将要添加二维码的PPTX文件或流。
      2. 为QrCodeSignOptions提供所需的文本。
      3. 自定义视觉设置，如颜色、位置和大小。
      4. 保存包含嵌入二维码的文档。
   
    code:
      platform: "python-net"
      copy_title: "复制"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "示例签名"
      install:
        command: "pip install groupdocs-signature-net"
        copy_tip: "点击以复制"
        copy_done: "已复制"
      links:
        #  loop
        - title: "更多示例"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
        #  loop
        - title: "文档"
          link: "https://docs.groupdocs.com/signature/python-net/"
          
      content: |
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # 初始化一个新的Signature实例与文档
            with sg.Signature('input.pptx') as signature:

                # 使用QrCodeSignOptions将二维码嵌入文档
                options = sg.QrCodeSignOptions("Text Content")

                # 指定签名类型并设置其在页面上的位置
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 50
                options.Top = 150

                # 保存包含嵌入二维码的文档
                result = signature.Sign("output.pptx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "文档的完整签名集成"
  description: "使用GroupDocs.Signature for Python via .NET API，用户可以生成、修改、搜索、验证和删除不同类型的签名，简化文档工作流程，同时确保精确性。"
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "GroupDocs.Signature的主要特性"
  features:
    # feature loop
    - title: "应用多种签名类型"
      content: "GroupDocs.Signature 允许将文本、图片、条形码、二维码和印章签名应用于任何文档。您可以精确地在任何页面上放置签名，并轻松管理元数据。使用数字证书保护您的文档，避免未经授权的更改。"

    # feature loop
    - title: "搜索和验证签名"
      content: "使用高级验证工具验证文档签名的真实性和准确性。轻松获取嵌入文档中的所有签名的详细列表，以便更好地进行监管。"

    # feature loop
    - title: "修改现有签名"
      content: "您可以通过调整内容、位置、颜色、大小和其他属性来更新先前应用的签名，以满足您的特定需求。"

    # feature loop
    - title: "轻松删除签名"
      content: "通过快速删除不需要的签名来简化文档管理。无论是数字证书还是其他类型的签名，删除过程都可以高效完成。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "自定义生成的二维码"
      content: |
        本示例展示了如何在PPTX页面上放置自定义的二维码。
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # 获取待签名的文档并传递给Signature
              with sg.Signature('input.pptx') as signature:

                    # 配置二维码选项，使用所需文本
                    options = sg.QrCodeSignOptions("Archived on July 11, 2019")

                    # 设置二维码在页面上的位置
                    options.VerticalAlignment = sg.Domain.VerticalAlignment.Top
                    options.HorizontalAlignment = sg.Domain.HorizontalAlignment.Right

                    # 设置签名的填充
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # 选择二维码的颜色
                    options.ForeColor = sg.Color.Red

                    # 为消息定义字体选项
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # 设置二维码的背景颜色和画刷
                    options.Background = sg.Background()
                    options.Background.Color = Color.LimeGreen
                    options.Background.Transparency = 0.5
                    options.Background.Brush = sg.LinearGradientBrush(sg.Color.LimeGreen, sg.Color.DarkGreen)

                    # 将二维码嵌入到文档中
                    result = signature.Sign("output.pptx", options)
          ```
        platform: "python-net"
        copy_title: "复制"
        install:
          command: "pip install groupdocs-signature-net"
          copy_tip: "点击以复制"
          copy_done: "已复制"
        top_links:
          #  loop
          - title: "下载结果"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.pptx"
        links:
          #  loop
          - title: "更多示例"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
          #  loop
          - title: "文档"
            link: "https://docs.groupdocs.com/signature/python-net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "准备开始了吗？"
  description: "免费试用 GroupDocs.Signature 的功能或请求许可证"
  items:
    #  loop
    - title: "PyPi 下载"
      link: "https://releases.groupdocs.com/signature/python-net/"
      color: "red"
        #  loop
    - title: "许可证"
      link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "探索我们的签名解决方案"
    exclude: "qrcode"
    description: "我们提供多种签名类型和操作，以满足您的文档需求。"
    items: 
          
        # operation loop 1
        - name: "电子签名"
          operation: "esign"
          link: "/signature/python-net/esign/pptx/"
          description: "向支持的文件格式添加各种类型的签名"

        # operation loop 2
        - name: "向文档添加文本"
          operation: "text"
          link: "/signature/python-net/text/pptx/"
          description: "通过可自定义的文本签名增强文档内容"

        # operation loop 3
        - name: "图像签名"
          operation: "image"
          link: "/signature/python-net/image/pptx/"
          description: "在文档内的任意位置放置任何图像"

        # operation loop 4
        - name: "生成条形码"
          operation: "barcode"
          link: "/signature/python-net/barcode/pptx/"
          description: "创建并插入各种条形码到支持的文档中"

        # operation loop 5
        - name: "生成二维码"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/pptx/"
          description: "生成用于文档签名的二维码"
          
        # operation loop 6
        - name: "数字证书"
          operation: "digital"
          link: "/signature/python-net/digital/pptx/"
          description: "安全地进行商业操作并使用数字证书签署文档"

        # operation loop 7
        - name: "盖章签名"
          operation: "stamp"
          link: "/signature/python-net/stamp/pptx/"
          description: "使用盖章构造器创建自定义圆形或方形印章"
          
        # operation loop 8
        - name: "搜索签名"
          operation: "search"
          link: "/signature/python-net/search/pptx/"
          description: "在文档中定位任何之前添加的签名"
          
        # operation loop 9
        - name: "签名验证"
          operation: "verify"
          link: "/signature/python-net/verify/pptx/"
          description: "验证签名在应用后是否真实有效"
          
        # operation loop 10
        - name: "修改签名"
          operation: "modify"
          link: "/signature/python-net/modify/pptx/"
          description: "轻松编辑文档中的多种签名"
          
        # operation loop 11
        - name: "删除签名"
          operation: "delete"
          link: "/signature/python-net/delete/pptx/"
          description: "移除多种之前应用的签名"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "在各种文档格式中嵌入二维码"
    exclude: "PPTX"
    description: "使用Python via .NET API将二维码嵌入到任何行业标准文档格式中。将重要信息存储和编码为2D条形码，以便于扫描和数据检索。"
    items: 
          
        # format loop 1
        - name: "PDF 的二维码"
          format: "PDF"
          link: "/signature/python-net/qrcode/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "DOCX 的二维码"
          format: "DOCX"
          link: "/signature/python-net/qrcode/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "JPEG 的二维码"
          format: "JPEG"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "PPTX 的二维码"
          format: "PPTX"
          link: "/signature/python-net/qrcode/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "XLSX 的二维码"
          format: "XLSX"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---