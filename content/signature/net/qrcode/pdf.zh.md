



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:21
draft: false
lang: zh
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "使用C#为PDF文件生成二维码"
head_description: "利用GroupDocs.Signature API为PDF文件生成二维码。无缝嵌入二维码以增强功能性。"

############################# Header ############################
title: "为PDF生成二维码" 
description: "通过GroupDocs.Signature for .NET轻松生成2D条形码，使用文本或数字数据，并应用于多个页面和格式，包括PDF、Word、Excel等。"
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "开始免费试用"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "探索GroupDocs.Signature for .NET的功能"
    link: "/signature/net/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/)提供丰富的功能，使用户能够在各类主流文档格式中生成和嵌入各种类型的签名。无论是PDF、Word文档、Excel表格、PowerPoint演示文稿还是图像文件，您都可以使用文本签名、图像签名、条形码、二维码、元数据、数字签名和印章来提升文档品质。

############################# Steps ############################
steps:
    enable: true
    title: "如何在PDF的任何位置生成并插入二维码"
    content: |
      [GroupDocs.Signature](/signature/net/)支持在各种流行格式中生成二维码，并将其放置在PDF页面上。我们的库支持超过10种类型的二维码，可以无缝集成到.NET应用程序中。使用我们的产品，通过二维码签名来提升文档。
      
      1. 获取要与二维码签名的PDF文件或流。
      2. 向QrCodeSignOptions提供所需的文本。
      3. 自定义视觉参数，如颜色、位置、大小等。
      4. 保存带有嵌入二维码的文档。
   
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
        // 用文档初始化一个新的Signature实例
        using (Signature signature = new Signature("input.pdf"))
        {
            // 利用QrCodeSignOptions将二维码嵌入文档
            QrCodeSignOptions options = new QrCodeSignOptions("Text Content")
                {
                    // 指定签名类型并确定其在页面上的位置
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150
                };

            // 保存带有集成二维码的文档
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "全面的文档签名集成"
  description: "通过GroupDocs.Signature for .NET API，用户可以轻松生成、修改、搜索、验证和移除各种类型的签名，以无与伦比的精度简化文档工作流程。"
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "GroupDocs.Signature的主要特性"
  features:
    # feature loop
    - title: "支持多种签名类型的文档签名"
      content: "GroupDocs.Signature支持在任意文档格式中应用文本签名、图像签名、条形码、二维码和印章。可以精确放置签名在任意页面，并且通过元数据签名可以无缝管理元数据。通过加入数字证书来保护文档的完整性，从而防止未授权的更改。"

    # feature loop
    - title: "签名搜索和验证"
      content: "通过先进的验证流程验证文档签名的真实性和准确性。轻松检索文档中所有嵌入签名的详细列表，以便全面监督。"

    # feature loop
    - title: "可自定义的签名修改"
      content: "通过调整内容、位置、颜色、大小等属性来更新和改进已应用的签名，以满足您的具体需求。"

    # feature loop
    - title: "高效的签名移除"
      content: "通过编程方式移除不需要的签名，从而简化文档管理。无论是处理数字证书还是其他签名类型，移除流程可以快速而有效地完成。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "如何使用各种选项生成二维码？"
      content: |
        这个示例演示了如何在PDF页面上放置自定义二维码。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 检索要签名的文档，并将其传递给Signature
          using (Signature signature = new Signature("input.pdf"))
          {
              // 使用必要文本配置二维码选项
              QrCodeSignOptions options = new QrCodeSignOptions("Archived on July 11, 2019")
              {
                    // 确定二维码在页面上的相对位置
                    VerticalAlignment = Domain.VerticalAlignment.Top,
                    HorizontalAlignment = Domain.HorizontalAlignment.Right,

                    // 设置签名填充
                    Margin = new Padding() { Top = 20, Right = 20 },

                    // 指定二维码颜色
                    ForeColor = Color.Red,

                    // 定义消息的字体选项
                    Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" },

                    // 自定义二维码的背景颜色和画笔
                    Background = new Background()
                    {
                        Color = Color.LimeGreen,
                        Transparency = 0.5,
                        Brush = new Domain.Extensions.LinearGradientBrush(Color.LimeGreen, Color.DarkGreen)
                    }
              };

              // 将二维码嵌入文档
              SignResult result = signature.Sign("output.pdf", options);
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
            link: "/examples/signature/formats/signature_qrcode.pdf"
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
    title: "了解我们的签名解决方案"
    exclude: "qrcode"
    description: "我们自豪地展示多种签名类型和操作功能"
    items: 
          
        # operation loop 1
        - name: "电子签名"
          operation: "esign"
          link: "/signature/net/esign/pdf/"
          description: "向支持的文件格式添加各种类型的签名"

        # operation loop 2
        - name: "向文档添加文本"
          operation: "text"
          link: "/signature/net/text/pdf/"
          description: "通过可自定义的文本签名增强文档内容"

        # operation loop 3
        - name: "图像签名"
          operation: "image"
          link: "/signature/net/image/pdf/"
          description: "在文档内的任意位置放置任何图像"

        # operation loop 4
        - name: "生成条形码"
          operation: "barcode"
          link: "/signature/net/barcode/pdf/"
          description: "创建并插入各种条形码到支持的文档中"

        # operation loop 5
        - name: "生成二维码"
          operation: "qrcode"
          link: "/signature/net/qrcode/pdf/"
          description: "生成用于文档签名的二维码"
          
        # operation loop 6
        - name: "数字证书"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "安全地进行商业操作并使用数字证书签署文档"

        # operation loop 7
        - name: "盖章签名"
          operation: "stamp"
          link: "/signature/net/stamp/pdf/"
          description: "使用盖章构造器创建自定义圆形或方形印章"
          
        # operation loop 8
        - name: "搜索签名"
          operation: "search"
          link: "/signature/net/search/pdf/"
          description: "在文档中定位任何之前添加的签名"
          
        # operation loop 9
        - name: "签名验证"
          operation: "verify"
          link: "/signature/net/verify/pdf/"
          description: "验证签名在应用后是否真实有效"
          
        # operation loop 10
        - name: "修改签名"
          operation: "modify"
          link: "/signature/net/modify/pdf/"
          description: "轻松编辑文档中的多种签名"
          
        # operation loop 11
        - name: "删除签名"
          operation: "delete"
          link: "/signature/net/delete/pdf/"
          description: "移除多种之前应用的签名"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "为其他文档格式生成二维码"
    exclude: "PDF"
    description: "通过.NET API增强所有行业标准文件格式，能够嵌入二维码。将关键信息存储和编码为2D条形码，便于无缝扫描和数据检索。"
    items: 
          
        # format loop 1
        - name: "PDF 的二维码"
          format: "PDF"
          link: "/signature/net/qrcode/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "DOCX 的二维码"
          format: "DOCX"
          link: "/signature/net/qrcode/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "JPEG 的二维码"
          format: "JPEG"
          link: "/signature/net/qrcode/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "PPTX 的二维码"
          format: "PPTX"
          link: "/signature/net/qrcode/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "XLSX 的二维码"
          format: "XLSX"
          link: "/signature/net/qrcode/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---