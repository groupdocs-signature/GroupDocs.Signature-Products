



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:40
draft: false
lang: zh
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "在Python应用程序中编辑XLSX签名"
head_description: "使用Python API轻松修改XLSX文档中的签名，包括PDF、Word文件、Excel表格、演示文稿和图像。"

############################# Header ############################
title: "轻松更新XLSX签名" 
description: "借助GroupDocs.Signature for Python via .NET的高级功能，全面控制编辑主要格式（如PDF、Word、Excel、演示文稿和图像）中的各种电子签名。"
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
    title: "解锁GroupDocs.Signature for Python via .NET的功能"
    link: "/signature/python-net/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/)不仅提供强大的文档签名功能，还允许您轻松修改现有签名。针对PDF、Word、Excel和PowerPoint演示文稿等广泛使用的格式，轻松调整签名属性。

############################# Steps ############################
steps:
    enable: true
    title: "如何使用Python编辑XLSX中的签名"
    content: |
      [GroupDocs.Signature](/signature/python-net/)允许Python via .NET开发人员编辑已经嵌入在XLSX文件中的文本签名。通过先进的功能增强您的Python via .NET应用程序。
      
      1. 将XLSX文档加载到Signature实例中。
      2. 检索文档中所有签名的列表。
      3. 编辑任何识别到的签名的内容。
      4. 验证签名修改的结果。
   
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

            # 创建一个Signature对象并设定文档路径
            with sg.Signature('input.xlsx') as signature:

                # 在文档中搜索文本签名
                options = sg.TextSearchOptions()
                signatures = signature.Search(options)

                if signatures.Count > 0:

                    # 更新第一个找到的签名的内容
                    textSignature = signatures[0]
                    textSignature.Text = "New Text"
                    result = signature.Update(textSignature)

                    # 验证签名更新的结果
                    if result:
                        print("\nSignature was updated successfully")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "文档的完整签名管理"
  description: "GroupDocs.Signature for Python via .NET通过支持在所有主要文件格式中轻松添加、更新、搜索、验证或删除签名，简化了您的文档工作流程。"
  image: "/img/signature/features_modify.webp" # 500x500 px
  image_description: "高级签名编辑"
  features:
    # feature loop
    - title: "灵活的文档签名"
      content: "在文档的任何部分应用各种签名，包括文本、图像、条形码和印章。修改图像中的EXIF数据等嵌入元数据，并使用数字证书保护文档不被未授权修改。"

    # feature loop
    - title: "签名搜索与验证"
      content: "通过我们强大的工具轻松验证签名。检索文档中所有签名的完整列表，确保快速准确的验证。"

    # feature loop
    - title: "简化的签名更新"
      content: "轻松更新先前嵌入的签名。根据新要求调整签名的内容、样式、位置或其他方面。"

    # feature loop
    - title: "轻松删除签名"
      content: "全面掌控签名管理，能够从文档中删除任何类型的签名，为内容提供完全的灵活性。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "修改条形码签名"
      content: |
        此示例演示了如何以编程方式编辑文档中的条形码签名。
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # 加载包含条形码签名的文档
              with sg.Signature('input.xlsx') as signature:

                  # 搜索所有现有的条形码签名
                  options = sg.BarcodeSearchOptions()
                  signatures = signature.Search(options)

                  if signatures.Count > 0:

                      # 更改第一个找到的条形码的位置并保存文档
                      barcodeSignature = signatures[0]
                      barcodeSignature.Left = 100
                      barcodeSignature.Top = 100
                      result = signature.Update(barcodeSignature)

                      # 验证条形码修改是否成功
                      if result:
                          print("\nBarcode was updated successfully.")
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
    title: "探索完整的功能集"
    exclude: "modify"
    description: "浏览我们平台支持的广泛签名格式和操作列表。"
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
    title: "跨多个格式修改签名"
    exclude: "XLSX"
    description: "通过Python via .NET API，您可以轻松修改已签名的文档。从支持的格式中提取和更新签名数据，全面控制文档的完整性。"
    items: 
          
        # format loop 1
        - name: "修改 PDF 签名"
          format: "PDF"
          link: "/signature/python-net/modify/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "编辑 DOCX 签名"
          format: "DOCX"
          link: "/signature/python-net/modify/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "编辑 PPTX 签名"
          format: "PPTX"
          link: "/signature/python-net/modify/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 4
        - name: "修改 XLSX 签名"
          format: "XLSX"
          link: "/signature/python-net/modify/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---