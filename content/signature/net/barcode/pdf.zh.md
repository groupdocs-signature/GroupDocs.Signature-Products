



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:06
draft: false
lang: zh
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "使用C# API生成PDF的条形码"
head_description: "只需几行代码即可使用C#生成条形码签名并保护PDF文档。利用GroupDocs.Signature进行广泛文件格式的签名。"

############################# Header ############################
title: "为PDF文档生成条形码" 
description: "利用GroupDocs.Signature for .NET在您的商业文档中任意位置放置条形码。我们的API提供广泛的条形码签名定制选项。"
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
    title: "GroupDocs.Signature for .NET概述"
    link: "/signature/net/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/)是一个复杂的文档签署解决方案，支持广泛的签名类型，包括文本、图像、条形码、数字证书和印章。兼容超过60种文件格式——如PDF、MS Office、图像、ZIP文件等——此工具不仅能够应用签名，还能根据需要搜索、验证、修改或删除签名。

############################# Steps ############################
steps:
    enable: true
    title: "在PDF文件中生成和嵌入条形码的步骤"
    content: |
      [GroupDocs.Signature](/signature/net/)支持在多个流行格式中生成条形码并将其放置在PDF页面上。支持超过60种条形码类型，通过集成我们的库，.NET应用程序可以轻松增强条形码签名功能。
      
      1. 提供要处理的PDF文件或流。
      2. 将条形码文本传递给BarcodeSignOptions实例。
      3. 定制条形码选项，如位置、大小等。
      4. 保存带有新附加条形码的文件。
   
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
        // 实例化一个新的Signature对象并设置文档路径
        using (Signature signature = new Signature("input.pdf"))
        {
            // 使用BarcodeSignOptions将条形码附加到文档
            BarcodeSignOptions options = new BarcodeSignOptions("Business data")
            {
                // 配置条形码类型和其他属性
                EncodeType = BarcodeTypes.Code128,
                Left = 50,
                Top = 150
            };

            // 保存已签名的文件
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "通过高级签名功能提升和保护您的文档"
  description: "GroupDocs.Signature for .NET库旨在促进在广泛使用的文件格式中进行全面的文档签名和处理。您可以轻松添加、调整、验证或删除不同类型的签名。"
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "GroupDocs.Signature的关键特性"
  features:
    # feature loop
    - title: "多功能文档签名"
      content: "高效地在支持的文档中的任意页面上使用文本、图像、条形码、二维码或印章进行签名。此外，可以嵌入隐藏的元数据，如图像中的EXIF数据，或使用数字证书保护文档内容避免未经授权的更改。"

    # feature loop
    - title: "全面的签名搜索和验证"
      content: "我们的工具提供强大的功能来处理已签名的文档。通过验证签名确保文档的完整性，并通过我们的搜索功能轻松检索文档中所有签名的全面列表。"

    # feature loop
    - title: "轻松编辑签名"
      content: "几乎所有已应用的签名都可以修改。方便地更新文本、调整位置或更改颜色以满足您的需求。"

    # feature loop
    - title: "高效的签名删除"
      content: "我们的方法完全支持签名的CRUD操作，可以快速删除您文档中任何不需要或过时的签名。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "如何生成条形码签名"
      content: |
        此示例展示了如何在PDF文档页面上嵌入自定义条形码。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          using (Signature signature = new Signature("input.pdf"))
          {
              // 使用所需文本制定签名选项
              BarcodeSignOptions options = new BarcodeSignOptions("Accepted")
              {
                  EncodeType = BarcodeTypes.Code39FullASCII,

                  // 确定页面上条形码的相对位置
                  VerticalAlignment = Domain.VerticalAlignment.Top,
                  HorizontalAlignment = Domain.HorizontalAlignment.Left,

                  // 定义条形码与页面边缘的内边距
                  Margin = new Padding() { Top = 180, Right = 20 },

                  // 指定条形码的颜色
                  ForeColor = Color.Red,

                  // 选择消息字体样式
                  Font = new SignatureFont { Size = 12, FamilyName = "Arial" },

                  // 指明消息的位置
                  CodeTextAlignment = CodeTextAlignment.Above
              };

              // 签署并保存文档
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
            link: "/examples/signature/formats/signature_barcode.pdf"
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
    title: "了解我们的主要功能"
    exclude: "barcode"
    description: "我们提供令人印象深刻的签名选项和操作"
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
    title: "在各种格式中签署文档"
    exclude: "PDF"
    description: "我们的.NET API支持对超过60种不同格式的签名。您可以轻松地在文档的任何页面或所需位置放置各种类型的签名。"
    items: 
          
        # format loop 1
        - name: "向 PDF 添加条形码"
          format: "PDF"
          link: "/signature/net/barcode/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "向 DOCX 添加条形码"
          format: "DOCX"
          link: "/signature/net/barcode/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "向 JPEG 添加条形码"
          format: "JPEG"
          link: "/signature/net/barcode/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "向 PPTX 添加条形码"
          format: "PPTX"
          link: "/signature/net/barcode/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "向 XLSX 添加条形码"
          format: "XLSX"
          link: "/signature/net/barcode/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---