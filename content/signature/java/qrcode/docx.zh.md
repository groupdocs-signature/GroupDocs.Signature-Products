



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:01
draft: false
lang: zh
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "使用Java为DOCX生成二维码"
head_description: "GroupDocs.Signature API支持为DOCX文件生成二维码。从您的内容创建二维码并将其放置在任何页面上。"

############################# Header ############################
title: "为DOCX创建二维码" 
description: "利用GroupDocs.Signature for Java方便地创建包含文本和数字数据的2D条形码，并将其放置在各种文件的任何页面上。"
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费试用"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "了解更多关于GroupDocs.Signature for Java的信息"
    link: "/signature/java/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/)提供多种功能，以生成和嵌入各种类型的签名，适用于所有主要文档格式。它支持PDF、Word文档、Excel电子表格、PowerPoint演示文稿和图像。通过文本、图像、条形码、二维码、元数据、数字和印章签名来增强您的文档。

############################# Steps ############################
steps:
    enable: true
    title: "在DOCX的任何位置生成并放置二维码的步骤"
    content: |
      [GroupDocs.Signature](/signature/java/)可以在许多流行格式中生成二维码，并将其放置在DOCX页面上。支持10多种二维码类型，可以快速集成到Java应用程序中。使用我们的产品为文档签名并生成二维码。
      
      1. 获取需要用二维码签署的DOCX文件或流。
      2. 为QrCodeSignOptions提供文本。
      3. 自定义视觉选项，例如颜色、位置、大小等。
      4. 保存带有二维码的文件。
   
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
        // 将文档传递给新的Signature实例
        Signature signature = new Signature("input.docx");

        // 使用QrCodeSignOptions将二维码添加到文档中
        QrCodeSignOptions options = new QrCodeSignOptions("Text Content");

        // 指定签名类型和在页面上的位置
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(50);
        options.setTop(150);

        // 保存带有添加的二维码的文件
        signature.sign("output.docx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "将签名添加到您的文档"
  description: "GroupDocs.Signature for Java API支持对所有流行文件格式进行签名。生成、修改、搜索、验证和删除不同类型的签名。"
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "GroupDocs.Signature的主要特性"
  features:
    # feature loop
    - title: "签署文档"
      content: "GroupDocs.Signature支持使用文本、图像、条形码、二维码和印章签名进行签署。将它们放置在任何受支持文档格式的任意页面上。使用元数据签名管理文档元数据，并通过数字证书保护内容免受未经授权的更改。"

    # feature loop
    - title: "搜索和验证"
      content: "通过验证程序确保文档中的所有签名均有效。使用内置搜索功能检索文档中的所有签名完整列表。"

    # feature loop
    - title: "修改签名"
      content: "在签署后轻松修改签名属性。根据需要调整内容、位置、颜色、大小等属性。"

    # feature loop
    - title: "移除签名"
      content: "轻松删除不需要的签名。各种签名类型，包括数字证书，可以通过编程方式从文档中移除。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "如何自定义生成的二维码"
      content: |
        使用此示例学习如何在DOCX页面上放置新的二维码。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 获取需要签署的文档并传递给Signature
          Signature signature = new Signature("input.docx");

          // 使用二维码选项提供包含所需信息的文本
          QrCodeSignOptions signOptions = new QrCodeSignOptions("Archived on July 11, 2019");

          // 在页面上设置二维码的相对位置
          signOptions.setVerticalAlignment(VerticalAlignment.Top);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Right);

          // 设置签名的边距
          Padding padding = new Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // 指定二维码的颜色
          signOptions.setForeColor(Color.RED);

          // 定义消息的字体选项
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // 自定义二维码背景颜色和画刷
          Background background = new Background();
          background.setColor(Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new LinearGradientBrush(Color.GREEN, Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // 将二维码添加到文档中
          SignResult signResult = signature.sign("output.docx", signOptions);
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
            link: "/examples/signature/formats/signature_qrcode.docx"
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
    title: "查看我们的主要产品"
    exclude: "qrcode"
    description: "我们提供各种签名功能和高级操作"
    items: 
          
        # operation loop 1
        - name: "电子签名"
          operation: "esign"
          link: "/signature/java/esign/docx/"
          description: "向支持的文件格式添加各种类型的签名"

        # operation loop 2
        - name: "向文档添加文本"
          operation: "text"
          link: "/signature/java/text/docx/"
          description: "通过可自定义的文本签名增强文档内容"

        # operation loop 3
        - name: "图像签名"
          operation: "image"
          link: "/signature/java/image/docx/"
          description: "在文档内的任意位置放置任何图像"

        # operation loop 4
        - name: "生成条形码"
          operation: "barcode"
          link: "/signature/java/barcode/docx/"
          description: "创建并插入各种条形码到支持的文档中"

        # operation loop 5
        - name: "生成二维码"
          operation: "qrcode"
          link: "/signature/java/qrcode/docx/"
          description: "生成用于文档签名的二维码"
          
        # operation loop 6
        - name: "数字证书"
          operation: "digital"
          link: "/signature/java/digital/docx/"
          description: "安全地进行商业操作并使用数字证书签署文档"

        # operation loop 7
        - name: "盖章签名"
          operation: "stamp"
          link: "/signature/java/stamp/docx/"
          description: "使用盖章构造器创建自定义圆形或方形印章"
          
        # operation loop 8
        - name: "搜索签名"
          operation: "search"
          link: "/signature/java/search/docx/"
          description: "在文档中定位任何之前添加的签名"
          
        # operation loop 9
        - name: "签名验证"
          operation: "verify"
          link: "/signature/java/verify/docx/"
          description: "验证签名在应用后是否真实有效"
          
        # operation loop 10
        - name: "修改签名"
          operation: "modify"
          link: "/signature/java/modify/docx/"
          description: "轻松编辑文档中的多种签名"
          
        # operation loop 11
        - name: "删除签名"
          operation: "delete"
          link: "/signature/java/delete/docx/"
          description: "移除多种之前应用的签名"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "为其他文件格式生成二维码"
    exclude: "DOCX"
    description: "使用Java API为所有流行文件格式增强生成的二维码。添加2D条形码数据，便于扫描和处理。"
    items: 
          
        # format loop 1
        - name: "PDF 的二维码"
          format: "PDF"
          link: "/signature/java/qrcode/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "DOCX 的二维码"
          format: "DOCX"
          link: "/signature/java/qrcode/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "JPEG 的二维码"
          format: "JPEG"
          link: "/signature/java/qrcode/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "PPTX 的二维码"
          format: "PPTX"
          link: "/signature/java/qrcode/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "XLSX 的二维码"
          format: "XLSX"
          link: "/signature/java/qrcode/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---