



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:10
draft: false
lang: zh
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "通过 C# 电子签署 DOCX 文件"
head_description: "利用 DOCX 向文档添加多种电子签名类型，确保在 PDF、Word、Excel、演示文稿和图像等格式中的安全性和合规性。"

############################# Header ############################
title: "DOCX 文件的电子签署" 
description: "使用 GroupDocs.Signature for .NET 将多种电子签名嵌入到文档中，确保 PDF、Word、Excel、演示文稿和图像等格式的合规性和完整性。"
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费下载"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for .NET API简介"
    link: "/signature/net/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) 提供全面的电子签名能力。借助此工具，您可以无缝地在各种文档类型中添加、搜索、验证、更新和删除数字签名，无需使用第三方工具。它可以轻松支持 PDF 文件、Word 文档、Excel 表格、PowerPoint 演示文稿和多种图像格式的签名。

############################# Steps ############################
steps:
    enable: true
    title: "使用 C# 签署 DOCX 的步骤"
    content: |
      [GroupDocs.Signature](/signature/net/) 方便将自定义签名整合到 DOCX 文件中。.NET 开发者可以利用我们的软件无缝集成签名功能到他们的应用中。
      
      1. 将 DOCX 文件提供给 Signature 实例进行签署。
      2. 使用 SignOptions 指定签名参数。
      3. 配置大小、颜色和内容等属性。
      4. 将签名文件保存到所需位置。
   
    code:
      platform: "net"
      copy_title: "复制"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "示例签名"
      install:
        command: "dotnet add package GroupDocs.Signature"
        copy_tip: "点击以复制"
        copy_done: "已复制"
      links:
        #  loop
        - title: "更多示例"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "文档"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```csharp {style=abap}
        // 将文档加载到 Signature 实例中
        using (Signature signature = new Signature("input.docx"))
        {
            // 创建一个新的 QrCodeSignOptions 对象
            QrCodeSignOptions options = new QrCodeSignOptions("QR code text")
            {
                // 配置所有必要选项
                Left = 50,
                Top = 200,
                ForeColor = Color.Red
            };

            // 将签名的文档保存到本地存储
            SignResult result = signature.Sign("output.docx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "高级文档电子签名"
  description: "我们先进的电子签名 API 增强了业务工作流程，实现了电子签名的高效签署、验证、修改和管理，具备全面的自动化能力。"
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "电子签名功能"
  features:
    # feature loop
    - title: "办公文档的电子签署"
      content: "可以在文档的任意位置无缝插入电子签名。用数字证书、元数据、条形码或视觉元素自定义和丰富内容，同时确保真实性和安全性。"

    # feature loop
    - title: "全面的签名管理"
      content: "一旦签署，文档可以进一步轻松处理。访问现有签名的完整概述，便于准确更新或删除必要的签名。"

    # feature loop
    - title: "增强的内容安全"
      content: "使用数字证书保护文档的完整性。嵌入或提取元数据以增强文档追踪和审计，确保合规性和内容的真实性。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "如何将图像签名添加到文档中"
      content: |
        此示例说明了在文档特定页面上应用图像签名的过程。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 将源文档作为一个参数提供
          using (Signature signature = new Signature("input.docx"))
          {
              // 在签名配置中指定图像的路径
              ImageSignOptions options = new ImageSignOptions("image.jpg")
              {
                  // 定义签名的尺寸和目标页面
                  VerticalAlignment = VerticalAlignment.Bottom,
                  HorizontalAlignment = HorizontalAlignment.Right,
                  Height = 150,
                  Width = 200,
                  Margin = new Padding(50),
                  AllPages = true
              };

              // 执行将签名应用于文档
              SignResult result = signature.Sign("output.docx", options);
          }

          ```
        platform: "net"
        copy_title: "复制"
        install:
          command: "dotnet add package GroupDocs.Signature"
          copy_tip: "点击以复制"
          copy_done: "已复制"
        top_links:
          #  loop
          - title: "下载结果"
            icon: "download"
            link: "/examples/signature/formats/signature_esign.docx"
        links:
          #  loop
          - title: "更多示例"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
          #  loop
          - title: "文档"
            link: "https://docs.groupdocs.com/signature/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "准备开始了吗？"
  description: "免费试用 GroupDocs.Signature 的功能或请求许可证"
  items:
    #  loop
    - title: "Nuget 下载"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "许可证"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "探索我们功能的全貌"
    exclude: "esign"
    description: "我们自豪地提供广泛的签名选项和相关操作"
    items: 
          
        # operation loop 1
        - name: "电子签名"
          operation: "esign"
          link: "/signature/net/esign/docx/"
          description: "向支持的文件格式添加各种类型的签名"

        # operation loop 2
        - name: "向文档添加文本"
          operation: "text"
          link: "/signature/net/text/docx/"
          description: "通过可自定义的文本签名增强文档内容"

        # operation loop 3
        - name: "图像签名"
          operation: "image"
          link: "/signature/net/image/docx/"
          description: "在文档内的任意位置放置任何图像"

        # operation loop 4
        - name: "生成条形码"
          operation: "barcode"
          link: "/signature/net/barcode/docx/"
          description: "创建并插入各种条形码到支持的文档中"

        # operation loop 5
        - name: "生成二维码"
          operation: "qrcode"
          link: "/signature/net/qrcode/docx/"
          description: "生成用于文档签名的二维码"
          
        # operation loop 6
        - name: "数字证书"
          operation: "digital"
          link: "/signature/net/digital/docx/"
          description: "安全地进行商业操作并使用数字证书签署文档"

        # operation loop 7
        - name: "盖章签名"
          operation: "stamp"
          link: "/signature/net/stamp/docx/"
          description: "使用盖章构造器创建自定义圆形或方形印章"
          
        # operation loop 8
        - name: "搜索签名"
          operation: "search"
          link: "/signature/net/search/docx/"
          description: "在文档中定位任何之前添加的签名"
          
        # operation loop 9
        - name: "签名验证"
          operation: "verify"
          link: "/signature/net/verify/docx/"
          description: "验证签名在应用后是否真实有效"
          
        # operation loop 10
        - name: "修改签名"
          operation: "modify"
          link: "/signature/net/modify/docx/"
          description: "轻松编辑文档中的多种签名"
          
        # operation loop 11
        - name: "删除签名"
          operation: "delete"
          link: "/signature/net/delete/docx/"
          description: "移除多种之前应用的签名"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "数字签名各种文件格式"
    exclude: "DOCX"
    description: ".NET API 使您能够电子签署超过 60 种行业标准文件格式，为保护您的业务文档提供无与伦比的灵活性。"
    items: 
          
        # format loop 1
        - name: "电子签名 PDF"
          format: "PDF"
          link: "/signature/net/esign/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "电子签名 DOCX"
          format: "DOCX"
          link: "/signature/net/esign/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "电子签名 JPEG"
          format: "JPEG"
          link: "/signature/net/esign/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "电子签名 PPTX"
          format: "PPTX"
          link: "/signature/net/esign/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "电子签名 XLSX"
          format: "XLSX"
          link: "/signature/net/esign/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---