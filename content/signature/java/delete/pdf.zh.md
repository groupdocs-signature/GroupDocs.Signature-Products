



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:41
draft: false
lang: zh
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "使用 Java 从 PDF 中删除签名"
head_description: "使用 GroupDocs.Signature for Java 可以轻松地从已签名的 PDF 文档中删除数字签名、条形码、文本、图像及元数据签名。"

############################# Header ############################
title: "从 PDF 中删除签名" 
description: "我们的解决方案不仅允许您签署业务文档，还提供使用 GroupDocs.Signature for Java 查找和删除各种类型签名的功能。"
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费下载"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Java 的介绍"
    link: "/signature/java/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) 提供全面的签名解决方案，能够处理多种类型的签名，如文本、图像、条形码、数字证书以及印章。该工具支持超过 60 种不同的文件格式，包括 PDF、MS Office 文档、图像文件、ZIP 压缩包，以及许多其他常用格式。此外，一旦应用了签名，您可以随时轻松搜索、验证、编辑或删除它们。

############################# Steps ############################
steps:
    enable: true
    title: "使用 Java 从 PDF 中删除电子签名的步骤"
    content: |
      [GroupDocs.Signature](/signature/java/) 使 Java 开发者能够通过遵循几个简单的步骤，在其应用程序中删除 PDF 文件中的电子签名。
      
      1. 将 PDF 路径传递给 Signature 类的一个实例。
      2. 使用 Search 方法从文档中检索签名。
      3. 删除一个或多个找到的签名。
      4. 分析文档处理的结果。
   
    code:
      platform: "java"
      copy_title: "复制"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "示例签名"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-signature</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "点击以复制"
        copy_done: "已复制"
      links:
        #  loop
        - title: "更多示例"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
        #  loop
        - title: "文档"
          link: "https://docs.groupdocs.com/signature/java/"
          
      content: |
        ```java {style=abap}
        // 将包含要删除的签名的文档传递给 Signature
        Signature signature = new Signature("input.pdf");

        // 检索文档中存在的数字签名
        DigitalSearchOptions options = new DigitalSearchOptions();
        List<DigitalSignature> signatures = signature.search(DigitalSignature.class, options);

        // 删除第一个找到的数字签名
        if(signatures.size() > 0)
        {
            DigitalSignature digitalSignature = signatures.get(0);
            boolean result = signature.delete("output.pdf", digitalSignature);

            // 处理删除结果
            if(result)
            {
                System.out.print("\nDigital PDF signature was deleted successfully");
            }
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "通过签名管理提升业务流程"
  description: "GroupDocs.Signature for Java 专为签署和管理业务文件格式而设计，使您能够根据需要添加、修改、验证或删除签名。"
  image: "/img/signature/features_delete.webp" # 500x500 px
  image_description: "GroupDocs.Signature 功能"
  features:
    # feature loop
    - title: "签署文档"
      content: "轻松地将文本、图像、条形码、二维码或印章签名添加到支持的文档的任何页面上。利用图像中的隐含元数据（如 EXIF），或者通过数字证书保护文档内容不被未授权的修改。"

    # feature loop
    - title: "搜索与验证"
      content: "通过验证签名以确保其有效性，充分利用已签名文档的潜力。您还可以通过简单的搜索检索文档中所有签名的完整列表。"

    # feature loop
    - title: "修改签名"
      content: "大多数之前添加的签名都可以调整。您可以轻松修改文本、重新定位签名或更改其颜色。"

    # feature loop
    - title: "删除签名"
      content: "我们的解决方案完全支持签名的 CRUD 操作，允许您根据需要从文档中删除各种类型的签名。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "删除所有条形码签名"
      content: |
        了解如何删除嵌入文档中的所有条形码签名。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 提供包含条形码签名的文档
          Signature signature = new Signature("input.pdf");

          // 删除所有条形码签名
          DeleteResult result = signature.delete("output.pdf", SignatureType.Barcode);

          // 处理删除的结果
          if (result.getSucceeded().size() > 0)
          {
              System.out.print("\nFollowing PDF barcode signatures were deleted:");
              int number = 1;
              for (BaseSignature temp : result.getSucceeded())
              {
                    System.out.print("Signature #"+number++ +
                    ": Type: "+temp.getSignatureType()+" Id:"+temp.getSignatureId()+
                    ", Text: "+((BarcodeSignature)temp).getText());
              }
          }
          ```
        platform: "java"
        copy_title: "复制"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-signature</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "点击以复制"
          copy_done: "已复制"
        links:
          #  loop
          - title: "更多示例"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "文档"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "准备开始了吗？"
  description: "免费试用 GroupDocs.Signature 的功能或请求许可证"
  items:
    #  loop
    - title: "Maven 下载"
      link: "https://releases.groupdocs.com/signature/java/"
      color: "red"
        #  loop
    - title: "许可证"
      link: "https://purchase.groupdocs.com/pricing/signature/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "了解我们的关键功能"
    exclude: "delete"
    description: "探索我们平台上可用的多种操作和签名方法"
    items: 
          
        # operation loop 1
        - name: "电子签名"
          operation: "esign"
          link: "/signature/java/esign/pdf/"
          description: "向支持的文件格式添加各种类型的签名"

        # operation loop 2
        - name: "向文档添加文本"
          operation: "text"
          link: "/signature/java/text/pdf/"
          description: "通过可自定义的文本签名增强文档内容"

        # operation loop 3
        - name: "图像签名"
          operation: "image"
          link: "/signature/java/image/pdf/"
          description: "在文档内的任意位置放置任何图像"

        # operation loop 4
        - name: "生成条形码"
          operation: "barcode"
          link: "/signature/java/barcode/pdf/"
          description: "创建并插入各种条形码到支持的文档中"

        # operation loop 5
        - name: "生成二维码"
          operation: "qrcode"
          link: "/signature/java/qrcode/pdf/"
          description: "生成用于文档签名的二维码"
          
        # operation loop 6
        - name: "数字证书"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "安全地进行商业操作并使用数字证书签署文档"

        # operation loop 7
        - name: "盖章签名"
          operation: "stamp"
          link: "/signature/java/stamp/pdf/"
          description: "使用盖章构造器创建自定义圆形或方形印章"
          
        # operation loop 8
        - name: "搜索签名"
          operation: "search"
          link: "/signature/java/search/pdf/"
          description: "在文档中定位任何之前添加的签名"
          
        # operation loop 9
        - name: "签名验证"
          operation: "verify"
          link: "/signature/java/verify/pdf/"
          description: "验证签名在应用后是否真实有效"
          
        # operation loop 10
        - name: "修改签名"
          operation: "modify"
          link: "/signature/java/modify/pdf/"
          description: "轻松编辑文档中的多种签名"
          
        # operation loop 11
        - name: "删除签名"
          operation: "delete"
          link: "/signature/java/delete/pdf/"
          description: "移除多种之前应用的签名"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "从各种文件格式中删除签名"
    exclude: "PDF"
    description: "我们的 GroupDocs.Signature for Java 解决方案支持从超过 60 种不同的文件格式中删除签名。"
    items: 
          
        # format loop 1
        - name: "删除 PDF 签名"
          format: "PDF"
          link: "/signature/java/delete/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "移除 DOCX 签名"
          format: "DOCX"
          link: "/signature/java/delete/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "删除 PPTX 签名"
          format: "PPTX"
          link: "/signature/java/delete/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 4
        - name: "删除 XLSX 签名"
          format: "XLSX"
          link: "/signature/java/delete/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---