



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:12
draft: false
lang: zh
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "使用 Python 应用程序对 PDF 文档进行电子签名"
head_description: "利用 Python API 的强大功能，以电子方式签署和保护 PDF 文档，例如 PDF、Word 文件、Excel 表格、演示文稿和图像。"

############################# Header ############################
title: "电子签名 PDF 文档" 
description: "使用 GroupDocs.Signature for Python via .NET 将各种电子签名嵌入到您的文档中，确保在 PDF、Word、Excel、演示文稿和图像等多种格式下的合规性和数据完整性。"
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费下载"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Python via .NET API 概述"
    link: "/signature/python-net/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) 提供了一整套为文档添加电子签名的工具。无论您需要签署、搜索、验证、更新还是删除数字签名，GroupDocs.Signature for Python via .NET 都能轻松处理多种格式—PDF、Word 文档、Excel 表格、PowerPoint 演示文稿及多种图像格式，而无需第三方软件。

############################# Steps ############################
steps:
    enable: true
    title: "使用 Python 对 PDF 进行电子签名的步骤"
    content: |
      使用 [GroupDocs.Signature](/signature/python-net/)，Python via .NET 开发人员可以无缝地将签名功能集成到 PDF 文档中。轻松将自定义签名添加到您的应用程序中。
      
      1. 将 PDF 文件加载到 Signature 实例中。
      2. 使用 SignOptions 配置签名设置。
      3. 自定义签名属性，例如大小、颜色和内容。
      4. 将签署的文档保存到所需位置。
   
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

            # 将文档加载到 Signature 实例中
            with sg.Signature('input.pdf') as signature:

                # 创建一个新的 QrCodeSignOptions 对象
                options = sg.QrCodeSignOptions("QR code text")

                # 设置所有必需选项
                options.Left = 100
                options.Top = 100
                options.ForeColor = sg.Color.Red

                # 将签署的文档保存到您的系统中
                result = signature.Sign("output.pdf", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "文档的高级电子签名功能"
  description: "我们的电子签名 API 提供高效的方式来签署、验证、修改和管理电子签名，并完全支持自动化。"
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "电子签名功能"
  features:
    # feature loop
    - title: "对办公文档进行电子签名"
      content: "可以在文档的任何位置轻松放置电子签名。通过数字证书、条形码、元数据和视觉元素自定义内容，同时确保文档的安全性和真实性。"

    # feature loop
    - title: "全面的签名管理"
      content: "一旦文档被签署，您可以查看和管理所有签名。可以根据需要更新或移除签名，确保对文档的完全控制。"

    # feature loop
    - title: "增强文档安全性"
      content: "使用数字证书保护您的文档。嵌入或提取元数据以改进跟踪、审计和合规性，确保内容的真实性。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "如何向文档添加图像签名"
      content: |
        此示例演示了如何将图像签名应用到文档的特定页面。
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg
        
          def run():

              # 加载您要签名的文档
              with sg.Signature('input.pdf') as signature:

                  # 在签名选项中设置图像的路径
                  options = sg.ImageSignOptions("image.jpg")

                  # 定义签名在目标页面上的大小和位置
                  options.VerticalAlignment = sg.VerticalAlignment.Bottom
                  options.HorizontalAlignment = sg.HorizontalAlignment.Right
                  options.Height = 150
                  options.Width = 200
                  options.Margin = sg.Padding(50)
                  options.AllPages = True

                  # 应用签名并保存已签署的文档
                  result = signature.Sign("output.pdf", options)
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
            link: "/examples/signature/formats/signature_esign.pdf"
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
    title: "探索我们的完整功能集"
    exclude: "esign"
    description: "我们为您提供各种签名选项和操作，以满足所有电子签名需求。"
    items: 
          
        # operation loop 1
        - name: "电子签名"
          operation: "esign"
          link: "/signature/python-net/esign/pdf/"
          description: "向支持的文件格式添加各种类型的签名"

        # operation loop 2
        - name: "向文档添加文本"
          operation: "text"
          link: "/signature/python-net/text/pdf/"
          description: "通过可自定义的文本签名增强文档内容"

        # operation loop 3
        - name: "图像签名"
          operation: "image"
          link: "/signature/python-net/image/pdf/"
          description: "在文档内的任意位置放置任何图像"

        # operation loop 4
        - name: "生成条形码"
          operation: "barcode"
          link: "/signature/python-net/barcode/pdf/"
          description: "创建并插入各种条形码到支持的文档中"

        # operation loop 5
        - name: "生成二维码"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/pdf/"
          description: "生成用于文档签名的二维码"
          
        # operation loop 6
        - name: "数字证书"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "安全地进行商业操作并使用数字证书签署文档"

        # operation loop 7
        - name: "盖章签名"
          operation: "stamp"
          link: "/signature/python-net/stamp/pdf/"
          description: "使用盖章构造器创建自定义圆形或方形印章"
          
        # operation loop 8
        - name: "搜索签名"
          operation: "search"
          link: "/signature/python-net/search/pdf/"
          description: "在文档中定位任何之前添加的签名"
          
        # operation loop 9
        - name: "签名验证"
          operation: "verify"
          link: "/signature/python-net/verify/pdf/"
          description: "验证签名在应用后是否真实有效"
          
        # operation loop 10
        - name: "修改签名"
          operation: "modify"
          link: "/signature/python-net/modify/pdf/"
          description: "轻松编辑文档中的多种签名"
          
        # operation loop 11
        - name: "删除签名"
          operation: "delete"
          link: "/signature/python-net/delete/pdf/"
          description: "移除多种之前应用的签名"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "对各种文件格式进行电子签名"
    exclude: "PDF"
    description: "通过 Python via .NET API，您可以对超过 60 种行业标准格式进行电子签名，为您的业务文档提供无与伦比的灵活性。"
    items: 
          
        # format loop 1
        - name: "电子签名 PDF"
          format: "PDF"
          link: "/signature/python-net/esign/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "电子签名 DOCX"
          format: "DOCX"
          link: "/signature/python-net/esign/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "电子签名 JPEG"
          format: "JPEG"
          link: "/signature/python-net/esign/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "电子签名 PPTX"
          format: "PPTX"
          link: "/signature/python-net/esign/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "电子签名 XLSX"
          format: "XLSX"
          link: "/signature/python-net/esign/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---