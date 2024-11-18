



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:55
draft: false
lang: zh
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "使用C#应用程序为DOCX创建文本签名"
head_description: "利用C# API将文本签名嵌入DOCX文件中，支持PDF、Word、Excel、演示文稿、图片和ZIP等多种格式。"

############################# Header ############################
title: "无缝嵌入DOCX中的文本签名" 
description: "通过使用GroupDocs.Signature for .NET轻松将自定义文本签名集成到您的业务文档中。利用多样化的签名自定义功能优化组织流程。"
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "立即免费试用"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "探索GroupDocs.Signature for .NET解决方案"
    link: "/signature/net/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/)提供一个复杂的平台，用于嵌入高度可定制的文本签名，简化您的文档工作流程。调整文本签名的内容和视觉属性，使其无缝应用于各个页面，以提升文档管理并增强运营效率。

############################# Steps ############################
steps:
    enable: true
    title: "如何使用C#为DOCX创建和添加文本签名"
    content: |
      [GroupDocs.Signature](/signature/net/)便于将文本签名纳入DOCX文件内的.NET应用程序中。迅速通过我们的全面解决方案增强您的产品能力。
      
      1. 将DOCX文档作为参数传递给Signature类构造函数。
      2. 创建拥有必要签名文本的TextSignOptions。
      3. 定义签名的视觉属性。
      4. 将文本签名嵌入到文档的任何指定页面中。
   
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
        // 使用文档路径初始化Signature
        using (Signature signature = new Signature("input.docx"))
        {
            // 使用所需的签名文本创建TextSignOptions实例
            TextSignOptions options = new TextSignOptions("Approved")
            {
                // 配置文本颜色和字体属性
                ForeColor = Color.Red,
                Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" }
            };

            // 将文本签名集成到文档中
            SignResult result = signature.Sign("output.docx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "全面的文本签名管理"
  description: "GroupDocs.Signature for .NET通过在流行文件格式中添加可定制的文本签名，增强您的组织的文档工作流程。轻松管理这些签名的外观、位置和内容，以满足您的特定需求。"
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "探索GroupDocs.Signature的功能"
  features:
    # feature loop
    - title: "多样化的文档签名"
      content: "在受支持的文档的任意页面上应用多种签名，包括文本、图像、条形码、二维码和印章。利用元数据嵌入隐藏内容，同时通过使用数字证书保护敏感信息。"

    # feature loop
    - title: "签名搜索和验证"
      content: "通过利用我们强大的签名验证工具，确保您签署的文档的有效性和完整性。进行搜索以检索文档中所有签名的全面列表以进行进一步分析。"

    # feature loop
    - title: "更新或删除签名"
      content: "轻松修改先前嵌入的签名的内容、视觉属性或位置。如有必要，删除不必要的签名，以保持文档内容的准确性和相关性。"

    # feature loop
    - title: "专业化的文本签名"
      content: "实现文档特定的文本签名，如Word文档的水印或PDF的贴纸，以提供额外的定制和控制层。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "在文档中嵌入文本签名"
      content: |
        了解如何将文本签名纳入业务文档中，以简化流程。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 选择要签署的文档
          using (Signature signature = new Signature("input.docx"))
          {
              // 使用指定的内容制定文本选项
              TextSignOptions options = new TextSignOptions("Rescheduled to 03/04/2025")
              {
                    // 定义签名在页面上的尺寸和位置
                    Left = 100,
                    Top = 180,
                    Width = 230,
                    Height = 30,

                    // 为签名实现页面边缘的填充
                    Margin = new Padding() { Top = 20, Right = 20 },

                    // 定制文本颜色和字体样式
                    ForeColor = Color.OrangeRed,
                    Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" },

                    // 围绕文本签名加入边框
                    Border = new Border()
                    {
                        Color = Color.OrangeRed,
                        DashStyle = DashStyle.Dash,
                        Transparency = 0.5,
                        Visible = true,
                        Weight = 2
                    },

                    // 如有必要，可以实施背景定制
                    Background = new Background()
                    {
                        Color = Color.LightYellow,
                        Transparency = 0.8
                    },

                    // 可选地将文本保存为图像以确保兼容性
                    SignatureImplementation = TextSignatureImplementation.Image
              };

              // 保存集成了文本签名的文档
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
            link: "/examples/signature/formats/signature_text.docx"
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
    title: "高级功能和签名选项"
    exclude: "text"
    description: "我们的API支持七种签名类型的全生命周期管理，提供全面的CRUD功能，以管理、验证和定制您的签名。"
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
    title: "在多种文件格式中嵌入文本签名"
    exclude: "DOCX"
    description: "通过我们的.NET API，您可以将文本签名嵌入各种Office文档中。通过添加增强功能和安全性的文本签名，全面控制文档的生命周期。"
    items: 
          
        # format loop 1
        - name: "PDF 文本签名"
          format: "PDF"
          link: "/signature/net/text/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "DOCX 文本签名"
          format: "DOCX"
          link: "/signature/net/text/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "JPEG 文本签名"
          format: "JPEG"
          link: "/signature/net/text/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "PPTX 文本签名"
          format: "PPTX"
          link: "/signature/net/text/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "XLSX 文本签名"
          format: "XLSX"
          link: "/signature/net/text/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---