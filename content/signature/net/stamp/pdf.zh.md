



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:47
draft: false
lang: zh
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "通过 C# 为 PDF 文件生成圆形和方形印章"
head_description: "使用 GroupDocs.Signature for .NET 在 PDF 文件中生成并嵌入个性化印章。"

############################# Header ############################
title: "为 PDF 文件生成印章" 
description: "通过 GroupDocs.Signature for .NET 无缝集成自定义设计的印章到您文件的任何部分，提供印章放置和配置的广泛灵活性，以满足您的业务需求。"
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "获取您的免费下载"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for .NET 概述"
    link: "/signature/net/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) 是一款多功能工具，支持在文档中插入多种类型的签名，包括可定制的印章。支持超过60种文件格式，从PDF和Word文档到图像和ZIP文件，您可以通过文本、图像、条形码、元数据、数字证书和印章来丰富您的文档。此外，您可以全面控制搜索、验证、修改或移除应用于文件的任何签名。

############################# Steps ############################
steps:
    enable: true
    title: "如何使用 C# 将印章嵌入 PDF"
    content: |
      [GroupDocs.Signature](/signature/net/) 提供强大的印章创建功能，非常适合增强 .NET 应用程序。利用此工具在文档页面上设计和实施高度自定义的印章。
      
      1. 提供要添加印章的 PDF 文档。
      2. 利用 StampSignOptions 精确配置所有所需参数。
      3. 根据要求添加多个印章行。
      4. 应用配置好的印章并保存修改后的文档。
   
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
        // 将文档路径与 Signature 实例集成
        using (Signature signature = new Signature("input.pdf"))
        {
            // 使用所需的签名内容初始化 StampSignOptions
            StampSignOptions options = new StampSignOptions();
            options.Height = 180;
            options.Width = 180;

            // 整合一个或多个印章行
            options.OuterLines.Add(
                new StampLine()
                {
                    Text = "* The Best Company *",
                    TextRepeatType = StampTextRepeatType.FullTextRepeat,
                    Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                    Height = 22,
                    TextBottomIntent = 6,
                    TextColor = Color.WhiteSmoke,
                    BackgroundColor = Color.DarkSlateBlue
                }
            );

            // 保存已应用印章的文档
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "利用签名确保和增强文档完整性"
  description: "使用 GroupDocs.Signature for .NET 库，您可以将签名功能无缝集成到文档中。轻松添加、修改、验证或移除自定义印章和其他类型的签名，为安全文档管理提供灵活性和准确性。"
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "由 GroupDocs.Signature 支持的印章签名"
  features:
    # feature loop
    - title: "全面的文档签名"
      content: "通过在文件中的任何位置或页面放置签名，包括文本、图像、条形码、二维码和印章，以增强文档。此外，管理嵌入的元数据并应用数字证书来防止未经授权的更改。"

    # feature loop
    - title: "高效的签名搜索与验证"
      content: "签名后，验证文档签名的真实性和完整性。利用先进的搜索功能来检索和管理文档中嵌入的所有签名数据。"

    # feature loop
    - title: "修改和自定义签名"
      content: "轻松调整之前插入的签名。无论您需要更改内容、位置、大小还是颜色，我们的解决方案都提供完全的灵活性来修改签名。"

    # feature loop
    - title: "轻松移除签名"
      content: "当需要移除签名时，GroupDocs.Signature for .NET 提供一整套工具来删除任何类型的签名，包括印章、数字证书等，确保您的文档始终保持最新且符合规定。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "在文档中实现自定义印章"
      content: |
        了解如何制作和集成包含关键文本信息的自定义印章到您的文档中。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 提供要添加印章的文档
          using (Signature signature = new Signature("input.pdf"))
          {
              // 使用所需配置初始化印章选项
              StampSignOptions options = new StampSignOptions()
              {
                    // 定义印章在页面上的尺寸和位置
                    Height = 200,
                    Width = 200,
                    VerticalAlignment = VerticalAlignment.Bottom,
                    HorizontalAlignment = HorizontalAlignment.Right,
                    AllPages = true
              };

              // 整合带文本的外部圆形线条
              options.OuterLines.Add(
                    new StampLine()
                    {
                        Text = "* The best  choice *",
                        TextRepeatType = StampTextRepeatType.FullTextRepeat,
                        Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                        Height = 22,
                        TextBottomIntent = 6,
                        TextColor = Color.WhiteSmoke,
                        BackgroundColor = Color.DarkSlateBlue
                    }
              );

              // 如有必要，整合内部方形线条
              options.InnerLines.Add(
                    new StampLine()
                    { 
                        Text = "Company #1",
                        TextColor = Color.MediumVioletRed,
                        Font = new SignatureFont() { Size = 20, Bold = true },
                        Height = 40
                    }
              );

              // 完成并保存已加印章的文档
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
            link: "/examples/signature/formats/signature_stamp.pdf"
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
    title: "探索核心功能"
    exclude: "stamp"
    description: "发现广泛的选项以创建、管理和删除各种类型的签名，确保全面控制您的文档工作流。"
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
    title: "在各种文档格式中应用印章"
    exclude: "PDF"
    description: "GroupDocs.Signature API 允许您在超过60种行业标准文件类型中嵌入印章。轻松将自定义印章应用于文档中的任何位置，从而实现增强的文档跟踪和个性化。"
    items: 
          
        # format loop 1
        - name: "盖章 PDF"
          format: "PDF"
          link: "/signature/net/stamp/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "盖章 DOCX"
          format: "DOCX"
          link: "/signature/net/stamp/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "盖章 JPEG"
          format: "JPEG"
          link: "/signature/net/stamp/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "盖章 PPTX"
          format: "PPTX"
          link: "/signature/net/stamp/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "盖章 XLSX"
          format: "XLSX"
          link: "/signature/net/stamp/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---