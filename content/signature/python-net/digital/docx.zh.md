



---
############################# Static ############################
layout: "format"
date:  2024-11-20T08:57:24
draft: false
lang: zh
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "使用 Python 在 DOCX 中创建数字签名"
head_description: "使用 Python 仅需几行代码即可数字签署 DOCX 文档。使用 GroupDocs.Signature for Python via .NET 签署多种文件格式。"

############################# Header ############################
title: "数字签署 DOCX" 
description: "通过 GroupDocs.Signature for Python via .NET 应用数字证书，确保文档的安全性和真实性。我们的解决方案使您能够使用强大的工具签署和保护文档。"
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费获取"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Python via .NET 是什么？"
    link: "/signature/python-net/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) 是一个综合签名工具，支持广泛的文档处理任务。它允许您向超过 60 种文件格式（包括 PDF、MS Office 文件、图像和 ZIP 文件）添加文本、图像、数字证书和印章。使用 GroupDocs.Signature for Python via .NET，您可以随时查找、验证、更新或删除签名。

############################# Steps ############################
steps:
    enable: true
    title: "如何在 Python 中使用数字证书保护 DOCX"
    content: |
      [GroupDocs.Signature](/signature/python-net/) 帮助 Python via .NET 开发人员通过添加数字签名来保护 DOCX 文件。加强您的业务应用程序的文档保护功能。
      
      1. 将 DOCX 文件加载到 Signature 类中。
      2. 应用数字证书及其密码以保护文件。
      3. 可选地在文档页面上添加数字签名的视觉显示。
      4. 签署文档，以防止未授权的更改。
   
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

            # 使用 Signature 数字签署文档
            with sg.Signature('input.docx') as signature:

                # 输入数字证书及其密码
                options = sg.DigitalSignOptions("certificate.pfx")
                options.Password = "1234567890"

                # 可选配置签名的外观
                options.PageNumber = 1
                options.Left = 50
                options.Top = 50

                # 使用数字证书完成文档签署
                result = signature.Sign("output.docx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "通过数字签名增强和保护文档"
  description: "GroupDocs.Signature for Python via .NET 库被设计用于签署所有主要文件格式。简化工作流程，轻松添加、验证、更新或删除不同类型的签名。"
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "GroupDocs.Signature 的核心功能"
  features:
    # feature loop
    - title: "向文档添加签名"
      content: "在受支持的文档中精确地插入文本、图像、条形码、二维码或印章签名。您还可以管理隐藏的元数据，例如图像中的 EXIF，以确保文档的完整性和数字签名。"

    # feature loop
    - title: "验证和搜索签名"
      content: "签署后，您可以轻松验证文档，以确保正确处理。利用强大的搜索功能检索和管理文件中的所有签名。"

    # feature loop
    - title: "编辑现有签名"
      content: "大多数签名可以完全自定义。您可以编辑文本、移动元素、改变颜色、调整大小等以满足您的需求。"

    # feature loop
    - title: "删除不必要的签名"
      content: "我们的解决方案支持完整的签名管理，允许您在需要时从任何文档中删除签名，包括数字证书。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "使用数字签名保护文档"
      content: |
        了解如何通过应用数字签名来保护您的文档，以防止未授权的修改。
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # 加载要签名的文档
              with sg.Signature('input.docx') as signature:

                  # 使用有效的数字证书及其相应密码
                  options = sg.DigitalSignOptions("certificate.pfx")
                  options.Password = "1234567890"

                  # 如有需要，添加任何额外的文本信息
                  options.Reason = "Security issue"
                  options.Contact = "John Smith"
                  options.Location = "Office D.W."

                  # 包含图像或其他选项以视觉方式表示签名
                  options.ImageFilePath = "image.png"
                  options.AllPages = True
                  options.VerticalAlignment = sg.VerticalAlignment.Center
                  options.HorizontalAlignment = sg.HorizontalAlignment.Left
                  options.Width = 60
                  options.Height = 80

                  options.Margin = sg.Padding()
                  options.Margin.Bottom = 10
                  options.Margin.Right = 10

                  # 将已签署的文档保存在安全位置
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
            link: "/examples/signature/formats/signature_digital.docx"
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
    exclude: "digital"
    description: "我们提供广泛的签名选项和强大的文档操作。"
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
    title: "签署多种格式的文档"
    exclude: "DOCX"
    description: "使用 Python via .NET API，您可以处理超过 60 种不同格式，添加签名、应用数字证书以确保安全，并在各个页面管理签名。"
    items: 
          
        # format loop 1
        - name: "保护 PDF"
          format: "PDF"
          link: "/signature/python-net/digital/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "保护 DOCX"
          format: "DOCX"
          link: "/signature/python-net/digital/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "保护 PPTX"
          format: "PPTX"
          link: "/signature/python-net/digital/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 4
        - name: "保护 XLSX"
          format: "XLSX"
          link: "/signature/python-net/digital/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---