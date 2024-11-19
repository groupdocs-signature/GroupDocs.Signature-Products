



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:18
draft: false
lang: zh
format: Pptx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "使用 C# 为 PPTX 文件添加数字电子签名"
head_description: "使用 C# 在 PPTX 文件上添加数字签名，只需几行代码。使用 GroupDocs.Signature for .NET 签署多种文件格式。"

############################# Header ############################
title: "使用数字签名对 PPTX 进行电子签名" 
description: "通过使用 GroupDocs.Signature for .NET 的强大功能，用数字证书封装您的业务文件，以保护内容的完整性。我们提供多样化的解决方案来标记和保护您的文档。"
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
    title: "关于 GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) 是一种复杂的签名解决方案，能有效地处理各种文档处理任务。它允许您将文本、图像、数字证书和印章嵌入超过 60 种格式的文件中，包括 PDF、MS Office、图像、ZIP 文件及其他重要的商业格式。此外，签署的文档可以轻松地进行搜索、验证、修改或根据需要进行移除。

############################# Steps ############################
steps:
    enable: true
    title: "如何在 C# 中用数字证书保护 PPTX"
    content: |
      [GroupDocs.Signature](/signature/net/) 使 .NET 开发人员能够通过数字签名保护 PPTX 文档不被更改。增强您的业务应用程序，提供强大的数据保护能力。
      
      1. 将 PPTX 文档传递给 Signature 类构造函数。
      2. 使用数字证书及其密码来保护该文档。
      3. 可选地，在文档页面上添加数字签名的视觉表示。
      4. 签署文档以确保其未被更改。
   
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
        // 利用 Signature 对文档进行数字签名
        using (Signature signature = new Signature("input.pptx"))
        {
            // 提供数字证书及相关密码
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                Password = "1234567890",

                // 如有需要，配置视觉表现
                PageNumber = 1,
                Left = 50,
                Top = 50
            };

            // 使用数字证书保护文档
            SignResult result = signature.Sign("output.pptx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "通过签名增强或保护文档内容"
  description: "GroupDocs.Signature for .NET 库专为签署所有常见文件格式而设计。通过轻松添加、修改、验证或删除多种签名，简化您的业务流程。"
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "GroupDocs.Signature 的主要功能"
  features:
    # feature loop
    - title: "将签名嵌入文档"
      content: "在任何支持的文档的任何页面上精确嵌入文本、图像、条形码、二维码或印章签名。您还可以在图像和大多数文件类型中添加或编辑隐藏的元数据，如 EXIF。确保您文档内容的完整性，通过数字签名。"

    # feature loop
    - title: "搜索和验证签名"
      content: "后签名处理提供了许多可能性。验证您的签署文档是否已正确处理。为了更大的控制，您可以通过搜索功能检索所有签名的全面列表。"

    # feature loop
    - title: "修改签名"
      content: "大多数签名类型都可以完全编辑。您可以灵活调整文本，重新定位元素，改变颜色，调整大小等。"

    # feature loop
    - title: "移除多余的签名"
      content: "我们的解决方案提供签名的完整 CRUD 操作。如果需要，您可以从文档中删除多种签名类型，包括数字证书。"
      
  code_samples:
    # code sample loop
    - title: "使用数字签名保护文档"
      content: |
        了解如何使用数字签名防止文档修改。
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        // 提供待签署的文档
        using (Signature signature = new Signature("input.pptx"))
        {
            // 使用有效的数字证书及相应密码
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                Password = "1234567890",

                // 指定任何附加文本信息
                Reason = "Security issue",
                Contact = "John Smith",
                Location = "Office D.W.",

                // 添加图像及其他视觉表示选项
                ImageFilePath = "image.png",
                AllPages = true,
                VerticalAlignment = VerticalAlignment.Center,
                HorizontalAlignment = HorizontalAlignment.Left,
                Width = 60,
                Height = 80,

                Margin = new Padding() {  Bottom = 10, Right = 10 }
            };

            // 将安全文档保存到指定位置
            SignResult result = signature.Sign("output.pptx", options);
        }
        ```
        {{< /landing/code >}}


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
    title: "查看我们的突出功能"
    exclude: "digital"
    description: "我们提供多样化的签名格式和强大的操作"
    items: 
          
        # operation loop 1
        - name: "电子签名"
          operation: "esign"
          link: "/signature/net/esign/pptx/"
          description: "向支持的文件格式添加各种类型的签名"

        # operation loop 2
        - name: "向文档添加文本"
          operation: "text"
          link: "/signature/net/text/pptx/"
          description: "通过可自定义的文本签名增强文档内容"

        # operation loop 3
        - name: "图像签名"
          operation: "image"
          link: "/signature/net/image/pptx/"
          description: "在文档内的任意位置放置任何图像"

        # operation loop 4
        - name: "生成条形码"
          operation: "barcode"
          link: "/signature/net/barcode/pptx/"
          description: "创建并插入各种条形码到支持的文档中"

        # operation loop 5
        - name: "生成二维码"
          operation: "qrcode"
          link: "/signature/net/qrcode/pptx/"
          description: "生成用于文档签名的二维码"
          
        # operation loop 6
        - name: "数字证书"
          operation: "digital"
          link: "/signature/net/digital/pptx/"
          description: "安全地进行商业操作并使用数字证书签署文档"

        # operation loop 7
        - name: "盖章签名"
          operation: "stamp"
          link: "/signature/net/stamp/pptx/"
          description: "使用盖章构造器创建自定义圆形或方形印章"
          
        # operation loop 8
        - name: "搜索签名"
          operation: "search"
          link: "/signature/net/search/pptx/"
          description: "在文档中定位任何之前添加的签名"
          
        # operation loop 9
        - name: "签名验证"
          operation: "verify"
          link: "/signature/net/verify/pptx/"
          description: "验证签名在应用后是否真实有效"
          
        # operation loop 10
        - name: "修改签名"
          operation: "modify"
          link: "/signature/net/modify/pptx/"
          description: "轻松编辑文档中的多种签名"
          
        # operation loop 11
        - name: "删除签名"
          operation: "delete"
          link: "/signature/net/delete/pptx/"
          description: "移除多种之前应用的签名"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "以各种格式签署文件"
    exclude: "PPTX"
    description: ".NET API 使您能够处理超过 60 种不同格式。您可以在任何页面上无缝创建和嵌入多种签名，为内容安全应用数字证书，并高效管理文档中的现有签名。"
    items: 
          
        # format loop 1
        - name: "保护 PDF"
          format: "PDF"
          link: "/signature/net/digital/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "保护 DOCX"
          format: "DOCX"
          link: "/signature/net/digital/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "保护 PPTX"
          format: "PPTX"
          link: "/signature/net/digital/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 4
        - name: "保护 XLSX"
          format: "XLSX"
          link: "/signature/net/digital/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---