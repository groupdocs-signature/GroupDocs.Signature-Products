



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:14
draft: false
lang: zh
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "使用 Python 搜索 XLSX 中的电子签名"
head_description: "利用 GroupDocs.Signature for Python via .NET API 搜索嵌入在 PDF、Word、Excel、演示文稿和图像等格式中的电子签名。"

############################# Header ############################
title: "XLSX 数字签名搜索" 
description: "利用 GroupDocs.Signature for Python via .NET 提取来自多个格式（包括 PDF、Word、Excel、演示文稿和图像）的电子签名的完整列表。"
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "立即下载"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "释放 GroupDocs.Signature for Python via .NET 的潜力"
    link: "/signature/python-net/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) 提供了签署和管理数字文档的高级功能。支持超过 60 种文件格式，包括 PDF、Office 文档、图像和 ZIP 文件，您可以添加、搜索、验证、修改或删除签名，例如文本、图像、条形码、二维码、数字证书和印章。

############################# Steps ############################
steps:
    enable: true
    title: "如何使用 Python 在 XLSX 中搜索签名"
    content: |
      [GroupDocs.Signature](/signature/python-net/) 提供强大的引擎，用于检测 XLSX 文件中的数字签名。Python via .NET 开发人员可以轻松增强其应用程序的功能。
      
      1. 提供用于签名搜索的 XLSX 文件路径。
      2. 使用 SearchOptions 来细化搜索标准。
      3. 调用 Search 方法以检索结果。
      4. 审查识别的签名列表。
   
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

            # 使用文档的文件路径初始化 Signature 对象
            with sg.Signature('input.xlsx') as signature:

                # 创建 TextSearchOptions 的实例以搜索所有页面
                options = sg.TextSearchOptions()
                options.AllPages = True

                # 运行搜索以定位文档中的任何基于文本的签名
                signatures = signature.Search(options)
                print("\nSource document contains following text signature(s).")

                # 收集找到的签名列表以进行详细审查
                for textSignature in signatures:
                    print("\nFound Text signature at page ", textSignature.PageNumber)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "完整的文档签署平台"
  description: "体验功能强大、丰富的签署解决方案，使用多种签名类型保护您的文档，涵盖各种文件格式。"
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "搜索和管理签名"
  features:
    # feature loop
    - title: "签署并保护商业文档"
      content: "在文档中的任意位置添加电子签名。GroupDocs.Signature 支持多种签名类型，包括文本、图像、条形码、元数据、印章和数字证书，确保文档的真实性和安全性。"

    # feature loop
    - title: "全面的签名管理"
      content: "文档签署后，使用搜索功能找到所有嵌入的签名。根据需要修改或删除签名，您可以全面控制文档的完整性。"

    # feature loop
    - title: "确保文档的完整性"
      content: "使用高级工具管理文档中的隐藏元数据。添加或删除元数据，并应用数字证书以保护您的文档免受未授权更改，确保其真实性。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "搜索图像签名"
      content: |
        该示例演示如何在特定文档中查找图像签名。
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # 将源文档传递给构造函数
              with sg.Signature('input.xlsx') as signature:

                    # 搜索任何基于文本的签名
                    signatures = signature.Search(sg.SignatureType.Image)
                    print("\nSource document contains following image signature(s).")

                    # 显示识别的签名的详细属性
                    for imageSignature in signatures:
                        print("\nFound image signature at page ", imageSignature.PageNumber)
          ```
        platform: "python-net"
        copy_title: "复制"
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
    title: "核心功能"
    exclude: "search"
    description: "我们的 API 提供广泛的灵活性，使用户能够签署文档并执行签署后的操作，如搜索、验证和编辑签名。"
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
    title: "从多种文件格式中提取签名"
    exclude: "XLSX"
    description: "GroupDocs.Signature for Python via .NET API 允许您从多种文档格式中提取和管理签名。轻松从主要文件类型中检索嵌入的签名，以进行进一步分析或处理。"
    items: 
          
        # format loop 1
        - name: "搜索 PDF 中的签名"
          format: "PDF"
          link: "/signature/python-net/search/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "查找 DOCX 中的签名"
          format: "DOCX"
          link: "/signature/python-net/search/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "查找 PPTX 中的签名"
          format: "PPTX"
          link: "/signature/python-net/search/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 4
        - name: "搜索 XLSX 中的签名"
          format: "XLSX"
          link: "/signature/python-net/search/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---