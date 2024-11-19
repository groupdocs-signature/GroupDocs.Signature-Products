



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:36
draft: false
lang: zh
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "XLSX 数字签名验证使用 C#"
head_description: "利用强大的 GroupDocs.Signature for .NET 来验证嵌入在 XLSX 文件中的签名。验证 PDF、Word、Excel、演示文稿、图像和 ZIP 格式的签名是否合法。"

############################# Header ############################
title: "XLSX 数字签名验证" 
description: "高效验证 PDF、Word、Excel、演示文稿、图像或 ZIP 文件中所有支持的电子签名，使用 GroupDocs.Signature for .NET 的全面功能。"
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
    title: "GroupDocs.Signature for .NET 的主要应用"
    link: "/signature/net/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) 支持文件签名管理的完整 CRUD 能力。您可以使用多种签名类型（如文本、图像、条形码、数字证书、元数据和印章）在 60 多种不同格式中签名，包括 PDF、MS Office 文件、图像和 ZIP 压缩文件。除了签名外，它还允许您搜索、验证、更新或删除签名。

############################# Steps ############################
steps:
    enable: true
    title: "使用 C# 验证 XLSX 中的签名指南"
    content: |
      [GroupDocs.Signature](/signature/net/) 可以验证 XLSX 文档中特定签名的存在。.NET 开发人员可以通过集成我们解决方案提供的功能轻松增强其应用。
      
      1. 将 XLSX 文件加载到 Signature 实例中。
      2. 实例化并配置 VerifyOptions 以实现所需的验证结果。
      3. 开始验证过程。
      4. 查看和解读验证结果。
   
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
        // 用文档初始化一个 Signature 实例
        using (Signature signature = new Signature("input.xlsx"))
        {
            // 配置 TextVerifyOptions 以验证包含特定文本的签名
            TextVerifyOptions options = new TextVerifyOptions()
            {
                Text = "signature",
                MatchType = TextMatchType.Contains
            };

            // 对文档的签名进行验证
            VerificationResult result = signature.Verify(options);

            // 分析和解读验证结果
            if(result.IsValid)
            {
                Console.WriteLine($"\nDocument was verified successfully!");
                foreach (TextSignature item in result.Succeeded)
                {
                    Console.WriteLine($"\nValid signature is found with text: {item.Text}");
                }
            }
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "先进的文件签名"
  description: "GroupDocs.Signature 是一款全面解决方案，旨在简化广泛使用格式的文件签署和认证。它提供 7 种签名类型和完整的 CRUD 操作，以确保对您的文档内容进行全面的保护和管理。"
  image: "/img/signature/features_verify.webp" # 500x500 px
  image_description: "签名验证功能"
  features:
    # feature loop
    - title: "简化企业文件签署"
      content: "无缝地将定制的数字签名应用到您的文档的任何部分。支持文本、图像、条形码、元数据、印章和数字证书签名，GroupDocs.Signature for .NET 确保您的文档符合企业标准。"

    # feature loop
    - title: "完整的签名生命周期管理"
      content: "轻松管理文档中签名的整个生命周期。根据需要访问、验证、更新或删除任何签名，确保文档始终保持最新和准确。"

    # feature loop
    - title: "文档内容完整性保护"
      content: "通过嵌入数字证书来保护敏感文档，防止未经授权的修改。此外，添加隐藏的元数据以保护关键信息并加强内容完整性。"

    # feature loop
    - title: "量身定制的本地签名"
      content: "利用文档特定的签名类型，如 PDF 印章和 Word 水印。这些量身定制的签名非常适合品牌推广、水印或合规目的，为您的企业文档增添专业修饰。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "验证条形码签名"
      content: |
        此示例说明如何在文档中验证条形码签名的过程。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          using (Signature signature = new Signature("input.xlsx"))
          {
              // 配置验证选项以匹配具有特定文本条件的条形码
              BarcodeVerifyOptions options = new BarcodeVerifyOptions()
              {
                    Text = "12345",
                    MatchType = TextMatchType.StartsWith
              };

              // 验证嵌入文档中的签名
              VerificationResult result = signature.Verify(options);

              // 呈现验证过程的结果
              if (result.IsValid)
              {
                  Console.WriteLine($"\nDocument was verified successfully!");
                  foreach (BarcodeSignature item in result.Succeeded)
                  {
                      Console.WriteLine($"\nValid signature is found with text: {item.Text} 
                            and type: {item.EncodeType.TypeName}.");
                  }
              }
          }
          ```
        platform: "net"
        copy_title: "复制"
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
    title: "全面的操作和签名类型"
    exclude: "verify"
    description: "探索 GroupDocs.Signature 提供的丰富功能和签名管理操作，全面控制文档的签名过程。"
    items: 
          
        # operation loop 1
        - name: "电子签名"
          operation: "esign"
          link: "/signature/net/esign/xlsx/"
          description: "向支持的文件格式添加各种类型的签名"

        # operation loop 2
        - name: "向文档添加文本"
          operation: "text"
          link: "/signature/net/text/xlsx/"
          description: "通过可自定义的文本签名增强文档内容"

        # operation loop 3
        - name: "图像签名"
          operation: "image"
          link: "/signature/net/image/xlsx/"
          description: "在文档内的任意位置放置任何图像"

        # operation loop 4
        - name: "生成条形码"
          operation: "barcode"
          link: "/signature/net/barcode/xlsx/"
          description: "创建并插入各种条形码到支持的文档中"

        # operation loop 5
        - name: "生成二维码"
          operation: "qrcode"
          link: "/signature/net/qrcode/xlsx/"
          description: "生成用于文档签名的二维码"
          
        # operation loop 6
        - name: "数字证书"
          operation: "digital"
          link: "/signature/net/digital/xlsx/"
          description: "安全地进行商业操作并使用数字证书签署文档"

        # operation loop 7
        - name: "盖章签名"
          operation: "stamp"
          link: "/signature/net/stamp/xlsx/"
          description: "使用盖章构造器创建自定义圆形或方形印章"
          
        # operation loop 8
        - name: "搜索签名"
          operation: "search"
          link: "/signature/net/search/xlsx/"
          description: "在文档中定位任何之前添加的签名"
          
        # operation loop 9
        - name: "签名验证"
          operation: "verify"
          link: "/signature/net/verify/xlsx/"
          description: "验证签名在应用后是否真实有效"
          
        # operation loop 10
        - name: "修改签名"
          operation: "modify"
          link: "/signature/net/modify/xlsx/"
          description: "轻松编辑文档中的多种签名"
          
        # operation loop 11
        - name: "删除签名"
          operation: "delete"
          link: "/signature/net/delete/xlsx/"
          description: "移除多种之前应用的签名"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "跨格式签名验证"
    exclude: "XLSX"
    description: "GroupDocs.Signature for .NET 使您能够高效验证各类文档格式中的签名。设置可定制的验证参数，以确保文档的完整性和合规性。"
    items: 
          
        # format loop 1
        - name: "验证 PDF 签名"
          format: "PDF"
          link: "/signature/net/verify/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "验证 DOCX 签名"
          format: "DOCX"
          link: "/signature/net/verify/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "验证 PPTX 签名"
          format: "PPTX"
          link: "/signature/net/verify/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 4
        - name: "验证 XLSX 签名"
          format: "XLSX"
          link: "/signature/net/verify/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---