



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:49
draft: false
lang: zh
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "使用Python在JPEG中创建圆形和方形印章"
head_description: "通过GroupDocs.Signature for Python via .NET API生成并插入个性化印章到JPEG文件中。"

############################# Header ############################
title: "为JPEG创建印章" 
description: "使用GroupDocs.Signature for Python via .NET轻松将自定义设计的印章添加到文档的任何部分，提供灵活的放置和配置，以满足您的业务需求。"
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
    title: "GroupDocs.Signature for Python via .NET概述"
    link: "/signature/python-net/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) 是一个全面的工具，允许您在文档中插入各种签名类型，包括自定义印章。支持超过60种文件格式——从PDF和Word文档到图像和ZIP文件，您可以通过文本、图像、条形码、元数据、数字证书和印章来增强您的文档。您还可以完全控制搜索、验证、编辑或删除任何应用的签名。

############################# Steps ############################
steps:
    enable: true
    title: "如何使用Python向JPEG添加印章"
    content: |
      [GroupDocs.Signature](/signature/python-net/) 提供强大的印章创建工具，以增强Python via .NET应用程序。利用它为您的文档页面设计和实施自定义印章。
      
      1. 提供您想要盖章的JPEG文档。
      2. 使用StampSignOptions配置所有必要设置。
      3. 如果需要，添加多个印章行。
      4. 应用印章并保存更新后的文档。
   
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

            # 将文档路径附加到Signature实例
            with sg.Signature('input.jpeg') as signature:

                # 设置带有所需印章详细信息的StampSignOptions
                options = sg.StampSignOptions()
                options.Height = 180
                options.Width = 180

                # 向印章添加一行或多行
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

                # 保存带有应用印章的文档
                result = signature.Sign("output.jpeg", options)
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "使用签名来保护和改善文档完整性"
  description: "借助GroupDocs.Signature for Python via .NET库，您可以无缝地向文档添加签名功能。轻松创建、修改、验证或删除自定义印章和其他签名类型，为您的文档工作流提供灵活性和安全性。"
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "由GroupDocs.Signature提供支持的印章签名"
  features:
    # feature loop
    - title: "完整的文档签署"
      content: "通过在任意页面的任何位置添加文本、图像、条形码、二维码和印章等签名来提升您的文档。管理嵌入的元数据并应用数字证书以防止未经授权的更改。"

    # feature loop
    - title: "高效的签名搜索和验证"
      content: "签署后，使用高级搜索工具查找所有嵌入的签名。轻松验证或管理签名数据，以确保文档的完整性。"

    # feature loop
    - title: "编辑和自定义签名"
      content: "轻松修改先前添加的签名。无论您想更改内容、位置、大小还是颜色，GroupDocs.Signature for Python via .NET都为您提供完全控制以根据需要调整签名。"

    # feature loop
    - title: "轻松删除签名"
      content: "如果需要删除签名，GroupDocs.Signature for Python via .NET提供所有必要的工具来删除任何类型的签名，包括印章和数字证书，帮助您保持文档的更新和合规。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "如何向文档添加自定义印章"
      content: |
        此示例展示了如何在文档中创建并插入带有特定文本细节的自定义印章。
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # 提供您想盖章的文档
              with sg.Signature('input.jpeg') as signature:

                    # 设置带有所需设置的印章选项
                    options = sg.StampSignOptions()

                    # 定义印章的大小和在页面上的位置
                    options.Height = 200
                    options.Width = 200
                    options.VerticalAlignment = sg.VerticalAlignment.Bottom
                    options.HorizontalAlignment = sg.HorizontalAlignment.Right
                    options.AllPages = True

                    # 添加带有文本的外圆形线条
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

                    # 可选地，添加内方形线条
                    innerLine = sg.StampLine()
                    innerLine.Text = "Company #1"
                    innerLine.TextColor = sg.Color.MediumVioletRed
                    innerLine.Font = sg.SignatureFont()
                    innerLine.Font.Size = 20
                    innerLine.Font.Bold = True
                    innerLine.Height = 40
                    options.InnerLines.Add(innerLine)

                    # 最终保存盖章的文档
                    result = signature.Sign("output.jpeg", options)
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
            link: "/examples/signature/formats/signature_stamp.jpeg"
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
    title: "探索关键功能"
    exclude: "stamp"
    description: "查找创建、管理和删除签名的各种选项，让您对文档工作流拥有完全的控制。"
    items: 
          
        # operation loop 1
        - name: "电子签名"
          operation: "esign"
          link: "/signature/python-net/esign/jpeg/"
          description: "向支持的文件格式添加各种类型的签名"

        # operation loop 2
        - name: "向文档添加文本"
          operation: "text"
          link: "/signature/python-net/text/jpeg/"
          description: "通过可自定义的文本签名增强文档内容"

        # operation loop 3
        - name: "图像签名"
          operation: "image"
          link: "/signature/python-net/image/jpeg/"
          description: "在文档内的任意位置放置任何图像"

        # operation loop 4
        - name: "生成条形码"
          operation: "barcode"
          link: "/signature/python-net/barcode/jpeg/"
          description: "创建并插入各种条形码到支持的文档中"

        # operation loop 5
        - name: "生成二维码"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "生成用于文档签名的二维码"
          
        # operation loop 6
        - name: "数字证书"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "安全地进行商业操作并使用数字证书签署文档"

        # operation loop 7
        - name: "盖章签名"
          operation: "stamp"
          link: "/signature/python-net/stamp/jpeg/"
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
    title: "将印章应用于各种文档格式"
    exclude: "JPEG"
    description: "使用GroupDocs.Signature API，您可以将自定义印章插入到超过60种标准文件类型中。轻松在文档中的任何位置应用印章，提升个性化和追踪能力。"
    items: 
          
        # format loop 1
        - name: "盖章 PDF"
          format: "PDF"
          link: "/signature/python-net/stamp/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "盖章 DOCX"
          format: "DOCX"
          link: "/signature/python-net/stamp/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "盖章 JPEG"
          format: "JPEG"
          link: "/signature/python-net/stamp/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "盖章 PPTX"
          format: "PPTX"
          link: "/signature/python-net/stamp/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "盖章 XLSX"
          format: "XLSX"
          link: "/signature/python-net/stamp/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---