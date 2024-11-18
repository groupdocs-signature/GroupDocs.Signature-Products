



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:53
draft: false
lang: zh
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "在XLSX文件中使用Python插入图像签名"
head_description: "仅需几行代码即可在Python中将图像签名嵌入XLSX文档。利用GroupDocs.Signature for Python via .NET API 无缝添加基于图像的签名。"

############################# Header ############################
title: "在XLSX中添加图像签名" 
description: "使用GroupDocs.Signature for Python via .NET将图像签名轻松整合到各种办公文档格式中，包括PDF、Word、Excel和图像文件。添加您经理的签名图像可以提升专业形象，增强视觉冲击力和文档的真实性。"
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
    title: "探索GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) 提供多种选项用于在商业文档中嵌入图像签名。借助我们强大的库，将图像添加到PDF、Word文档、Excel表格、PowerPoint演示文稿和流行的图像格式中，简化工作流程。

############################# Steps ############################
steps:
    enable: true
    title: "如何使用Python在XLSX文件中插入图像签名"
    content: |
      使用[GroupDocs.Signature](/signature/python-net/)为Python via .NET应用程序提供准确在XLSX文档中随处添加图像签名的功能。通过集成我们的解决方案来提升您的产品。
      
      1. 创建一个带有XLSX文档的Signature实例。
      2. 使用所需的签名图像配置ImageSignOptions。
      3. 准确将图像定位于文档中的所选位置。
      4. 将签名文档保存到指定位置。
   
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

            # 用文档路径初始化Signature
            with sg.Signature('input.xlsx') as signature:

                # 使用选定的签名图像设置ImageSignOptions
                options = sg.ImageSignOptions("company_logo.jpg")

                # 在每页的左上角定位图像
                options.AllPages = True
                options.Left = 100
                options.Top = 200
                
                # 保存已签名的文档
                result = signature.Sign("output.xlsx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "全面的文档签名功能"
  description: "我们的API支持广泛的签名功能。您可以轻松添加、更新、删除、搜索和验证不同类型的签名，包括基于图像的签名。"
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "图像签名集成"
  features:
    # feature loop
    - title: "将图像插入办公文档"
      content: "可以在文档中的任何位置嵌入电子签名和图像。通过添加图像、条形码、文本、元数据或数字证书来提升文档的功能性和安全性。"

    # feature loop
    - title: "签名搜索和验证"
      content: "通过验证签名的真实性来确保文档的完整性。检索文档中所有签名的详细列表，并评估其各自的属性。"

    # feature loop
    - title: "编辑现有签名"
      content: "轻松更新文档中签名的内容、外观、大小或位置，以满足不断变化的需求。"

    # feature loop
    - title: "删除不必要的签名"
      content: "我们的API提供全面控制，使您能够在需要时从大多数支持的文件格式中删除签名。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "使用图像签名增强文档"
      content: |
        了解如何在您的商业文档中嵌入图像签名以丰富内容。
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # 选择要签名的文档
              with sg.Signature('input.xlsx') as signature:

                    # 使用图像文件路径设置图像选项
                    options = sg.ImageSignOptions("manager_signature.jpg")

                    # 指定图像签名的大小
                    options.Width = 100
                    options.Height = 100

                    # 将图像定位于页面的右下角
                    options.VerticalAlignment = sg.VerticalAlignment.Bottom
                    options.HorizontalAlignment = sg.HorizontalAlignment.Right

                    # 根据需要设置页面边缘的填充
                    options.Margin = sg.Padding()
                    options.Margin.Bottom = 120
                    options.Margin.Right = 120

                    # 可选地，在图像周围添加边框
                    options.Border = sg.Border()
                    options.Border.Visible = True
                    options.Border.Color = sg.Color.OrangeRed
                    options.Border.DashStyle = sg.DashStyle.DashDotDot
                    options.Border.Weight = 5

                    # 旋转图像以确保正确对齐
                    options.RotationAngle = 45

                    # 保存已更新的文档
                    result = signature.Sign("output.xlsx", options)
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
            link: "/examples/signature/formats/signature_image.xlsx"
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
    title: "探索我们的功能"
    exclude: "image"
    description: "发现我们平台提供的不同签名类型和操作。"
    items: 
          
        # operation loop 1
        - name: "电子签名"
          operation: "esign"
          link: "/signature/python-net/esign/xlsx/"
          description: "向支持的文件格式添加各种类型的签名"

        # operation loop 2
        - name: "向文档添加文本"
          operation: "text"
          link: "/signature/python-net/text/xlsx/"
          description: "通过可自定义的文本签名增强文档内容"

        # operation loop 3
        - name: "图像签名"
          operation: "image"
          link: "/signature/python-net/image/xlsx/"
          description: "在文档内的任意位置放置任何图像"

        # operation loop 4
        - name: "生成条形码"
          operation: "barcode"
          link: "/signature/python-net/barcode/xlsx/"
          description: "创建并插入各种条形码到支持的文档中"

        # operation loop 5
        - name: "生成二维码"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "生成用于文档签名的二维码"
          
        # operation loop 6
        - name: "数字证书"
          operation: "digital"
          link: "/signature/python-net/digital/xlsx/"
          description: "安全地进行商业操作并使用数字证书签署文档"

        # operation loop 7
        - name: "盖章签名"
          operation: "stamp"
          link: "/signature/python-net/stamp/xlsx/"
          description: "使用盖章构造器创建自定义圆形或方形印章"
          
        # operation loop 8
        - name: "搜索签名"
          operation: "search"
          link: "/signature/python-net/search/xlsx/"
          description: "在文档中定位任何之前添加的签名"
          
        # operation loop 9
        - name: "签名验证"
          operation: "verify"
          link: "/signature/python-net/verify/xlsx/"
          description: "验证签名在应用后是否真实有效"
          
        # operation loop 10
        - name: "修改签名"
          operation: "modify"
          link: "/signature/python-net/modify/xlsx/"
          description: "轻松编辑文档中的多种签名"
          
        # operation loop 11
        - name: "删除签名"
          operation: "delete"
          link: "/signature/python-net/delete/xlsx/"
          description: "移除多种之前应用的签名"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "在多种文件格式中嵌入图像"
    exclude: "XLSX"
    description: "使用Python via .NET API将图像插入多种文档格式。轻松调整大小、定位、选择特定页面并应用基于图像的签名，让您全面掌控文档的布局。"
    items: 
          
        # format loop 1
        - name: "使用图像签名 PDF"
          format: "PDF"
          link: "/signature/python-net/image/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "使用图像签名 DOCX"
          format: "DOCX"
          link: "/signature/python-net/image/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "使用图像签名 JPEG"
          format: "JPEG"
          link: "/signature/python-net/image/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "使用图像签名 PPTX"
          format: "PPTX"
          link: "/signature/python-net/image/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "使用图像签名 XLSX"
          format: "XLSX"
          link: "/signature/python-net/image/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---