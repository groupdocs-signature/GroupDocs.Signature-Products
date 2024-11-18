



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:57
draft: false
lang: zh
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "使用 Python 在 DOCX 中添加文本签名"
head_description: "通过 Python API 将基于文本的签名嵌入到 DOCX 文件中，支持 PDF、Word、Excel、PowerPoint、图像和 ZIP 等格式。"

############################# Header ############################
title: "轻松将文本签名添加到 DOCX" 
description: "使用 GroupDocs.Signature for Python via .NET 无缝集成自定义文本签名到您的文档中。通过灵活的签名自定义选项简化工作流程。"
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "立即免费试用"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "探索 GroupDocs.Signature for Python via .NET 的强大功能"
    link: "/signature/python-net/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) 提供了一整套平台，用于嵌入可定制的文本签名，使文档工作流程更加顺畅。个性化文档中签名的内容和外观，以提高效率和增强文档管理。

############################# Steps ############################
steps:
    enable: true
    title: "如何使用 Python 创建 DOCX 文本签名"
    content: |
      [GroupDocs.Signature](/signature/python-net/) 使在 Python via .NET 应用程序中的 DOCX 文件中轻松集成文本签名。快速为您的产品添加功能支持。
      
      1. 将 DOCX 文档提供给 Signature 构造函数。
      2. 创建附有签名文本的 TextSignOptions。
      3. 设置签名的视觉属性。
      4. 将签名插入文档的所需页面。
   
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

            # 使用文档路径初始化 Signature
            with sg.Signature('input.docx') as signature:

                # 使用所需签名文本设置 TextSignOptions
                options = sg.TextSignOptions("Approved")

                # 选择签名的颜色和字体
                options.ForeColor = sg.Color.Red
                options.Font = sg.SignatureFont()
                options.Font.Size = 12
                options.Font.FamilyName = "Comic Sans MS"

                # 将文本签名应用到文档
                result = signature.Sign("output.docx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "全面的文本签名管理"
  description: "GroupDocs.Signature for Python via .NET 通过将自定义文本签名添加到流行格式来帮助您管理文档工作流程。轻松控制签名的外观、位置和内容，以满足您的需求。"
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "发现 GroupDocs.Signature 功能"
  features:
    # feature loop
    - title: "灵活的文档签名"
      content: "向任何文档页面添加各种签名类型——文本、图像、条形码、二维码和印章。使用元数据包括隐藏信息，并通过数字证书保护您的文件。"

    # feature loop
    - title: "验证和搜索签名"
      content: "利用先进工具检查您签署文档的完整性。对文件中的所有签名进行搜索和分析，以进一步验证。"

    # feature loop
    - title: "编辑或移除签名"
      content: "轻松更新现有签名的内容、外观或位置。移除过时的签名，以保持文档的时效性。"

    # feature loop
    - title: "专业的文本签名"
      content: "应用特定于文档的文本签名，比如 Word 文件的水印或 PDF 文件的印章，增加额外的控制和自定义层次。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "向文档添加文本签名"
      content: |
        了解如何将文本签名嵌入到文档中，以简化您的流程。
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # 选择要签名的文档
              with sg.Signature('input.docx') as signature:

                    # 用所需内容设置文本选项
                    options = sg.TextSignOptions("Rescheduled to 03/04/2025")

                    # 定义签名的大小和位置
                    options.Left = 100
                    options.Top = 180
                    options.Width = 230
                    options.Height = 30

                    # 设置页面边缘的填充
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # 选择文本颜色和字体样式
                    options.ForeColor = sg.Color.Red
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # 为文本签名添加边框
                    options.Border = sg.Border()
                    options.Border.Color = sg.Color.Red
                    options.Border.DashStyle = sg.DashStyle.DashLongDashDot
                    options.Border.Transparency = 0.5
                    options.Border.Visible = True
                    options.Border.Weight = 2

                    # 如有需要，自定义背景
                    options.Background = sg.Background()
                    options.Background.Color = sg.Color.Yellow
                    options.Background.Transparency = 0.8

                    # 可选地将签名保存为图像以确保兼容性
                    options.SignatureImplementation = sg.TextSignatureImplementation.Image

                    # 保存含有嵌入签名的文档
                    result = signature.Sign("output.docx", options)
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
            link: "/examples/signature/formats/signature_text.docx"
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
    title: "高级签名功能"
    exclude: "text"
    description: "我们的 API 支持七种签名类型的完整生命周期管理，让您可以创建、管理、验证和自定义签名。"
    items: 
          
        # operation loop 1
        - name: "电子签名"
          operation: "esign"
          link: "/signature/python-net/esign/docx/"
          description: "向支持的文件格式添加各种类型的签名"

        # operation loop 2
        - name: "向文档添加文本"
          operation: "text"
          link: "/signature/python-net/text/docx/"
          description: "通过可自定义的文本签名增强文档内容"

        # operation loop 3
        - name: "图像签名"
          operation: "image"
          link: "/signature/python-net/image/docx/"
          description: "在文档内的任意位置放置任何图像"

        # operation loop 4
        - name: "生成条形码"
          operation: "barcode"
          link: "/signature/python-net/barcode/docx/"
          description: "创建并插入各种条形码到支持的文档中"

        # operation loop 5
        - name: "生成二维码"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/docx/"
          description: "生成用于文档签名的二维码"
          
        # operation loop 6
        - name: "数字证书"
          operation: "digital"
          link: "/signature/python-net/digital/docx/"
          description: "安全地进行商业操作并使用数字证书签署文档"

        # operation loop 7
        - name: "盖章签名"
          operation: "stamp"
          link: "/signature/python-net/stamp/docx/"
          description: "使用盖章构造器创建自定义圆形或方形印章"
          
        # operation loop 8
        - name: "搜索签名"
          operation: "search"
          link: "/signature/python-net/search/docx/"
          description: "在文档中定位任何之前添加的签名"
          
        # operation loop 9
        - name: "签名验证"
          operation: "verify"
          link: "/signature/python-net/verify/docx/"
          description: "验证签名在应用后是否真实有效"
          
        # operation loop 10
        - name: "修改签名"
          operation: "modify"
          link: "/signature/python-net/modify/docx/"
          description: "轻松编辑文档中的多种签名"
          
        # operation loop 11
        - name: "删除签名"
          operation: "delete"
          link: "/signature/python-net/delete/docx/"
          description: "移除多种之前应用的签名"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "在多种格式中嵌入文本签名"
    exclude: "DOCX"
    description: "通过 Python via .NET API，您可以将文本签名添加到各种 Office 文档中，让您对文档生命周期拥有全面的控制，同时提高安全性。"
    items: 
          
        # format loop 1
        - name: "PDF 文本签名"
          format: "PDF"
          link: "/signature/python-net/text/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "DOCX 文本签名"
          format: "DOCX"
          link: "/signature/python-net/text/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "JPEG 文本签名"
          format: "JPEG"
          link: "/signature/python-net/text/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "PPTX 文本签名"
          format: "PPTX"
          link: "/signature/python-net/text/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "XLSX 文本签名"
          format: "XLSX"
          link: "/signature/python-net/text/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---