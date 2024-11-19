



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:24
draft: false
lang: zh
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "使用 Java 轻松将条形码添加到 JPEG 文件"
head_description: "在 Java 中创建并插入条形码签名到 JPEG 文档中。GroupDocs.Signature 使多种格式的签名集成更加灵活。"

############################# Header ############################
title: "为 JPEG 生成条形码" 
description: "使用 GroupDocs.Signature for Java 在商业文档的任意位置添加流行格式的条形码。我们的解决方案提供广泛的选项以自定义条形码签名。"
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
    title: "关于 GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) 是一种先进的签名解决方案，支持多种签名类型。您可以在超过 60 种文件格式中为文档签名，包括 PDF、MS Office、图像、ZIP 文件以及其他常用的业务格式，签名内容可以是文本、图像、条形码、数字证书、印章等。此外，已签名文档中的签名可以随时进行搜索、验证、修改或删除。

############################# Steps ############################
steps:
    enable: true
    title: "将条形码生成并添加到 JPEG 文件的步骤"
    content: |
      [GroupDocs.Signature](/signature/java/) 可以生成多种流行格式的条形码并将其放置在 JPEG 页面上。支持超过 60 种条形码类型，Java 应用程序可以通过集成我们的库轻松实现条形码签名功能。
      
      1. 提供要处理的 JPEG 文件或流。
      2. 将条形码文本传递给 BarcodeSignOptions 实例。
      3. 自定义条形码选项，如位置、大小等。
      4. 保存带有新添加条形码的文件。
   
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
        // 创建一个新的 Signature 实例并指定文档路径
        Signature signature = new Signature("input.jpeg");

        // 使用 BarcodeSignOptions 将条形码添加到文档
        BarcodeSignOptions options = new BarcodeSignOptions("Business data");

        // 设置条形码类型及其他属性
        options.setEncodeType(BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);

        // 保存签名后的文件
        signature.sign("output.jpeg", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "通过签名增强或保护文档内容"
  description: "GroupDocs.Signature for Java 库旨在签署和后续处理流行文件格式。快速灵活地添加、修改、验证或删除各种类型的签名。"
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "GroupDocs.Signature 的功能"
  features:
    # feature loop
    - title: "文档签名"
      content: "使用文本、图像、条形码、二维码或印章在支持的文档的任何页面上进行签名。可以在图像中添加隐藏元数据，例如 EXIF，或使用数字证书保护文档内容免受未经授权的修改。"

    # feature loop
    - title: "签名搜索和验证"
      content: "已签名文档可以完成更多操作。我们提供签名验证，以确保一切都处于正常状态。此外，您可以通过搜索获取所有文档签名的列表。"

    # feature loop
    - title: "修改签名"
      content: "大多数之前添加的签名可以进行修改。可以修正文本、调整位置或更改颜色。"

    # feature loop
    - title: "删除签名"
      content: "我们的解决方案支持签名的完全 CRUD 操作。许多类型的签名在必要时可以从文档中删除。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "如何创建条形码签名"
      content: |
        此示例演示如何在 JPEG 文档页面上放置自定义条形码。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 提供要签署的文档
          Signature signature = new Signature("input.jpeg");

          // 使用所需文本创建签名选项
          BarcodeSignOptions signOptions = new BarcodeSignOptions("Accepted");
          signOptions.setEncodeType(BarcodeTypes.Code39FullASCII);

          // 设置页面上相对条形码的位置
          signOptions.setVerticalAlignment(VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Left);

          // 设置离页面边缘的条形码填充
          Padding padding = new Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // 设置条形的颜色
          signOptions.setForeColor(Color.RED);

          // 定义消息字体样式
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Arial");
          signOptions.setFont(font);

          // 指定消息位置
          signOptions.setCodeTextAlignment(CodeTextAlignment.Above);

          // 签署并保存文档
          SignResult signResult = signature.sign("output.jpeg", signOptions);

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
        top_links:
          #  loop
          - title: "下载结果"
            icon: "download"
            link: "/examples/signature/formats/signature_barcode.jpeg"
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
    title: "发现我们的核心功能"
    exclude: "barcode"
    description: "我们自豪地展示广泛支持的签名和功能"
    items: 
          
        # operation loop 1
        - name: "电子签名"
          operation: "esign"
          link: "/signature/java/esign/jpeg/"
          description: "向支持的文件格式添加各种类型的签名"

        # operation loop 2
        - name: "向文档添加文本"
          operation: "text"
          link: "/signature/java/text/jpeg/"
          description: "通过可自定义的文本签名增强文档内容"

        # operation loop 3
        - name: "图像签名"
          operation: "image"
          link: "/signature/java/image/jpeg/"
          description: "在文档内的任意位置放置任何图像"

        # operation loop 4
        - name: "生成条形码"
          operation: "barcode"
          link: "/signature/java/barcode/jpeg/"
          description: "创建并插入各种条形码到支持的文档中"

        # operation loop 5
        - name: "生成二维码"
          operation: "qrcode"
          link: "/signature/java/qrcode/jpeg/"
          description: "生成用于文档签名的二维码"
          
        # operation loop 6
        - name: "数字证书"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "安全地进行商业操作并使用数字证书签署文档"

        # operation loop 7
        - name: "盖章签名"
          operation: "stamp"
          link: "/signature/java/stamp/jpeg/"
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
    title: "在其他格式中签署文档"
    exclude: "JPEG"
    description: "通过我们的 Java API 可以签署超过 60 种格式。可以在文档中的任何页面或位置应用各种签名。"
    items: 
          
        # format loop 1
        - name: "向 PDF 添加条形码"
          format: "PDF"
          link: "/signature/java/barcode/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "向 DOCX 添加条形码"
          format: "DOCX"
          link: "/signature/java/barcode/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "向 JPEG 添加条形码"
          format: "JPEG"
          link: "/signature/java/barcode/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "向 PPTX 添加条形码"
          format: "PPTX"
          link: "/signature/java/barcode/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "向 XLSX 添加条形码"
          format: "XLSX"
          link: "/signature/java/barcode/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---