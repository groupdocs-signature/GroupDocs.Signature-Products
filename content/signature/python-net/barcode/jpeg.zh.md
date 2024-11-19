



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:27
draft: false
lang: zh
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "在你的 JPEG 中嵌入条形码，使用 Python"
head_description: "高效地通过几行代码在 Python 中为 JPEG 文档添加条形码签名。GroupDocs.Signature 提供多种文档格式的无缝签名解决方案。"

############################# Header ############################
title: "为 JPEG 生成条形码" 
description: "使用 GroupDocs.Signature for Python via .NET，您可以在业务文档中需要的位置放置条形码。我们的解决方案提供灵活的条形码签名自定义选项。"
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
    title: "关于 GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) 是一款强大的文档签名工具，支持多种签名类型，包括文本、图片、条形码、数字证书和印章。兼容超过 60 种文件格式，如 PDF、MS Office、图片、ZIP 等，它不仅可以应用签名，还能让您根据需要搜索、验证、修改或删除签名。

############################# Steps ############################
steps:
    enable: true
    title: "在 JPEG 中生成和插入条形码的步骤"
    content: |
      [GroupDocs.Signature](/signature/python-net/) 允许您快速生成并嵌入条形码到 JPEG 文档中。支持超过 60 种条形码格式，Python via .NET 应用程序可以通过集成我们的库无缝添加条形码签名功能。
      
      1. 提供待处理的 JPEG 文件或流。
      2. 将条形码文本赋值给 BarcodeSignOptions 对象。
      3. 调整条形码选项，如位置和大小。
      4. 保存包含条形码的文档。
   
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

            # 初始化 Signature 对象，指定文档路径
            with sg.Signature('input.jpeg') as signature:

                # 使用 BarcodeSignOptions 为文档添加条形码
                options = sg.BarcodeSignOptions('Business data')

                # 设置条形码类型并配置其属性
                options.EncodeType = sg.BarcodeTypes.Code128
                options.Left = 50
                options.Top = 150

                # 保存已签名的文档
                result = signature.Sign('output.jpeg', options)
        ```          

############################# More features ############################
more_features:
  enable: true
  title: "使用高级签名功能提升文档品质"
  description: "GroupDocs.Signature for Python via .NET 库为在常用格式中签名和处理文档提供全面解决方案。您可以灵活添加、修改、验证或删除各种签名类型，以满足您的需求。"
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "GroupDocs.Signature 的关键特性"
  features:
    # feature loop
    - title: "灵活的文档签名"
      content: "使用文本、图片、条形码、二维码或印章在支持的文档的任何页面上签名。添加隐藏的元数据，如图片中的 EXIF 数据，并通过数字证书确保内容保护，以防止未授权更改。"

    # feature loop
    - title: "搜索和验证签名"
      content: "我们的工具通过启用签名验证确保文档的完整性。您还可以检索文档中所有签名的完整列表，以便于管理。"

    # feature loop
    - title: "轻松编辑签名"
      content: "轻松修改现有签名。调整文本、重新定位元素或更改颜色，以适应您的文档需求。"

    # feature loop
    - title: "轻松删除签名"
      content: "GroupDocs.Signature for Python via .NET 提供完整的 CRUD 功能，使您可以轻松删除文档中任何不需要的或过时的签名。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "创建并放置条形码签名"
      content: |
        此示例演示如何在 JPEG 文档中插入自定义条形码。
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # 提供待签名的文档
              with sg.Signature('input.jpeg') as signature:

                  # 设置条形码文本和签名选项
                  options = sg.BarcodeSignOptions('Accepted')
                  options.EncodeType = sg.BarcodeTypes.Code39FullASCII

                  # 选择条形码在页面上的位置
                  options.VerticalAlignment = sg.VerticalAlignment.Top
                  options.HorizontalAlignment = sg.HorizontalAlignment.Left

                  # 设置条形码与页面边缘之间的间距
                  options.Margin = sg.Padding()
                  options.Margin.Top = 180
                  options.Margin.Right = 20

                  # 指定条形码条的颜色
                  options.ForeColor = sg.Color.Red

                  # 选择条形码信息的字体样式
                  options.Font = sg.SignatureFont()
                  options.Font.Size = 12
                  options.Font.FamilyName = 'Arial'

                  # 设置信息文本的位置
                  options.CodeTextAlignment = sg.CodeTextAlignment.Above

                  # 签名并保存文档
                  result = signature.Sign('output.jpeg', options)
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
            link: "/examples/signature/formats/signature_barcode.jpeg"
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
    title: "探索我们的关键功能"
    exclude: "barcode"
    description: "我们为您的文档需求提供各种签名选项和操作。"
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
    title: "在多种格式中签名文档"
    exclude: "JPEG"
    description: "Python via .NET API 支持签名超过 60 种文件格式，允许您在文档的任何页面或特定位置添加各种类型的签名。"
    items: 
          
        # format loop 1
        - name: "向 PDF 添加条形码"
          format: "PDF"
          link: "/signature/python-net/barcode/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "向 DOCX 添加条形码"
          format: "DOCX"
          link: "/signature/python-net/barcode/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "向 JPEG 添加条形码"
          format: "JPEG"
          link: "/signature/python-net/barcode/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "向 PPTX 添加条形码"
          format: "PPTX"
          link: "/signature/python-net/barcode/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "向 XLSX 添加条形码"
          format: "XLSX"
          link: "/signature/python-net/barcode/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---