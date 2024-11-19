



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:42
draft: false
lang: zh
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "使用C#从DOCX中删除签名"
head_description: "使用GroupDocs.Signature for .NET可以轻松地从已签名的DOCX文档中删除数字、条形码、文本、图像和元数据签名。"

############################# Header ############################
title: "高效地从DOCX中移除签名" 
description: "我们的解决方案不仅限于签署商业文档，还提供全面的工具来查找和移除各种签名，使用GroupDocs.Signature for .NET。 "
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
       [GroupDocs.Signature for .NET](/signature/net/) 是一款强大的签名工具，支持添加多种类型的签名，包括文本、图像、条形码、数字证书和印章。该解决方案支持超过60种文件格式——包括PDF、MS Office、图像、ZIP及其他常用商业格式——确保灵活的文档管理。此外，应用的签名可以根据需要轻松地被定位、验证、修改或移除。

############################# Steps ############################
steps:
    enable: true
    title: "如何使用C#从DOCX中删除电子签名"
    content: |
      [GroupDocs.Signature](/signature/net/) 通过实施几个简单的步骤简化了.NET开发人员去除DOCX文件中的电子签名的任务。
      
      1. 将DOCX文件的路径提供给Signature类实例。
      2. 调用搜索方法以检索文档中的所有签名。
      3. 删除一个或多个检索到的签名。
      4. 检查文档处理的结果。
   
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
        // 将包含签名的文档传递给Signature实例
        using (Signature signature = new Signature("input.docx"))
        {
            // 检索文档中存在的数字签名
            DigitalSearchOptions options = new DigitalSearchOptions();

            List<DigitalSignature> signatures = signature.Search<DigitalSignature>(options);

            // 删除第一个识别的数字签名
            if(signatures.Count > 0)
            {
                DigitalSignature digitalSignature = signatures[0];
                bool result = signature.Delete(digitalSignature);

                // 删除第一个识别的数字签名
                if(result)
                {
                    Console.WriteLine($"Digital signature in DOCX was deleted successfully");
                }
            }
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "通过高级签名工具优化文档管理"
  description: "GroupDocs.Signature for .NET经过精心设计，以增强商业文件格式的签名和处理能力，实现签名的添加、修改、验证或删除。"
  image: "/img/signature/features_delete.webp" # 500x500 px
  image_description: "探索GroupDocs.Signature的多功能特性"
  features:
    # feature loop
    - title: "文档签名"
      content: "轻松将文本、图像、条形码、二维码或印章签名嵌入到支持的文档的任何页面中。此外，利用图像中的EXIF等隐藏元数据或使用数字证书保护文档完整性，防止未经授权的更改。"

    # feature loop
    - title: "签名搜索和验证"
      content: "利用我们的工具确保文档中签名的真实性。进行全面搜索以检索所有签名的完整列表，以确保全面的文档管理。"

    # feature loop
    - title: "签名修改"
      content: "轻松通过调整文本、移动位置或改变颜色来完善先前添加的签名，以满足特定需求。"

    # feature loop
    - title: "签名删除"
      content: "我们的解决方案提供签名的全面CRUD功能，使您能够在需要时高效地从文档中移除各种签名类型。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "消除所有条形码签名"
      content: |
        了解如何移除文档中嵌入的所有条形码签名。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 提供包含条形码签名的文档
          using (Signature signature = new Signature("input.docx"))
          {
              // 移除所有条形码签名
              DeleteResult result = signature.Delete(SignatureType.Barcode);

              // 评估删除过程的结果
              if (result.Succeeded.Count > 0)
              {
                  Console.WriteLine("Following DOCX barcode signatures were deleted:");                        
                  int number = 1;
                  foreach (BarcodeSignature temp in result.Succeeded)
                  {
                      Console.WriteLine($"Signature #{number++}: Type: {temp.SignatureType} 
                            Id:{temp.SignatureId}, Text: {temp.Text}");
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
    title: "查看我们的亮点功能"
    exclude: "delete"
    description: "我们很高兴提供广泛支持的签名类型和操作"
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
    title: "跨多个文件格式移除签名"
    exclude: "DOCX"
    description: "GroupDocs.Signature for .NET旨在方便地从超过60种文件格式中移除签名，确保广泛的兼容性和功能性。"
    items: 
          
        # format loop 1
        - name: "删除 PDF 签名"
          format: "PDF"
          link: "/signature/net/delete/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "移除 DOCX 签名"
          format: "DOCX"
          link: "/signature/net/delete/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "删除 PPTX 签名"
          format: "PPTX"
          link: "/signature/net/delete/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 4
        - name: "删除 XLSX 签名"
          format: "XLSX"
          link: "/signature/net/delete/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---