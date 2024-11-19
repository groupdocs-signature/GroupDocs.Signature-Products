



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:32
draft: false
lang: zh
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "在DOCX中使用C#搜索电子签名"
head_description: "利用GroupDocs.Signature for .NET API的能力，搜索嵌入PDF、Word、Excel、演示文稿和图像中的签名。"

############################# Header ############################
title: "在DOCX中搜索数字签名" 
description: "无缝提取嵌入在PDF、Word、Excel、演示文稿和图像等多种格式中的电子签名的全面列表，全部由GroupDocs.Signature for .NET提供支持。"
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "开始免费下载"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "探索GroupDocs.Signature for .NET的功能"
    link: "/signature/net/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/)提供尖端的数字文档签名功能。它支持包括PDF、MS Office文档、图像和ZIP文件在内的60多种文件格式，允许您添加、搜索、验证、修改或删除多种签名，例如文本、图像、条形码、二维码、数字证书和印章。

############################# Steps ############################
steps:
    enable: true
    title: "如何使用C#搜索DOCX签名"
    content: |
      [GroupDocs.Signature](/signature/net/)提供了一个强大的引擎，用于查找DOCX文件中的数字签名。.NET开发者可以轻松地将我们的解决方案集成到他们的应用程序中。
      
      1. 提供DOCX文件的路径进行签名搜索。
      2. 使用SearchOptions来细化搜索条件。
      3. 调用Search方法以检索结果。
      4. 评估识别出的签名列表。
   
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
        // 用指定的文档路径初始化一个Signature对象
        using (Signature signature = new Signature("input.docx"))
        {
            // 创建一个包含所有页面的TextSearchOptions实例
            TextSearchOptions options = new TextSearchOptions()
            {
                AllPages = true
            };

            // 执行搜索以识别文档中的任何基于文本的签名
            List<TextSignature> signatures = signature.Search<TextSignature>(options);
            Console.WriteLine($"\nSource document contains following text signature(s).");

            // 汇编检测到的签名列表以进行详细检查               
            foreach (TextSignature textSignature in signatures)
            {
                Console.WriteLine($"Found Text signature at page {textSignature.PageNumber} with type
                    [{textSignature.SignatureImplementation}] and text '{textSignature.Text}'.");
            }
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "完整的文档签名生态系统"
  description: "发现一个先进的、功能丰富的文档签名解决方案，专为增强和保护您的文档而设计，支持各种格式的多种签名类型。"
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "签名搜索和管理"
  features:
    # feature loop
    - title: "签署和保护业务文档"
      content: "在文档的任意位置添加数字签名。GroupDocs.Signature支持多种类型的签名，包括文本、图像、条形码、元数据、印章和数字证书，以确保文档的真实性和合规性。"

    # feature loop
    - title: "全面的签名管理"
      content: "签署后，利用搜索功能提取所有嵌入的签名。根据需要修改或删除签名，提供您对文档完整性的完全控制。"

    # feature loop
    - title: "保护文档的完整性"
      content: "利用先进工具管理嵌入文档中的隐藏元数据。添加或删除元数据条目，并应用公司的数字证书，以保护免受未经授权的编辑并确保文档的真实性。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "搜索图像签名"
      content: |
        此示例说明在指定文档中检测图像签名的过程。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 将源文档作为参数提供给构造函数
          using (Signature signature = new Signature("input.docx"))
          {
              // 搜索任何类型的文本签名
              List<ImageSignature> signatures = signature.Search<ImageSignature>(SignatureType.Image);
              Console.WriteLine($"\nSource document contains following image signature(s).");

              // 展示包含细节属性的识别签名结果
              foreach (ImageSignature imageSignature in signatures)
              {
                    Console.WriteLine($"Found Image signature at page {imageSignature.PageNumber} 
                    and size {imageSignature.Size}.");
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
    title: "核心功能"
    exclude: "search"
    description: "我们的API提供广泛的灵活性，允许用户签署文档并进行全面的后签名操作，例如搜索、验证和修改签名。"
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
    title: "从多种文件格式中提取签名"
    exclude: "DOCX"
    description: "GroupDocs.Signature for .NET API使您能够从广泛的文档类型中提取和管理签名。轻松从所有主要文件格式中获取嵌入的签名，以供进一步分析或处理。"
    items: 
          
        # format loop 1
        - name: "搜索 PDF 中的签名"
          format: "PDF"
          link: "/signature/net/search/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "查找 DOCX 中的签名"
          format: "DOCX"
          link: "/signature/net/search/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "查找 PPTX 中的签名"
          format: "PPTX"
          link: "/signature/net/search/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 4
        - name: "搜索 XLSX 中的签名"
          format: "XLSX"
          link: "/signature/net/search/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---