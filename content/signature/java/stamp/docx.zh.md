



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:46
draft: false
lang: zh
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "使用 Java 为 DOCX 添加印章"
head_description: "利用 GroupDocs.Signature 和 Java 创建自定义印章，并将它们放置在 DOCX 文档的任意页面上。"

############################# Header ############################
title: "为 DOCX 添加自定义印章" 
description: "使用 GroupDocs.Signature for Java 设计并应用圆形或方形印章于文档的任何部分。我们的解决方案提供广泛的自定义选项，以满足您所有的业务需求。"
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
       [GroupDocs.Signature for Java](/signature/java/) 是一款强大的工具，可以向文档添加各种印章签名。它支持超过 60 种不同的文件格式，包括 PDF、Word、Excel、图像和 ZIP 文件。您可以应用文本、图像、条形码、元数据、数字证书和印章签名。除了添加签名外，您还可以搜索、验证、修改和删除它们。

############################# Steps ############################
steps:
    enable: true
    title: "通过 Java 向 DOCX 添加印章的步骤"
    content: |
      [GroupDocs.Signature](/signature/java/) 提供了一种印章构造函数，该函数对 Java 应用程序非常有益。利用它为您的文档页面创建精美的自定义印章。
      
      1. 提供要添加印章的 DOCX 文档。
      2. 使用 StampSignOptions 配置所有必要参数。
      3. 添加所需数量的行。
      4. 应用印章并保存文档。
   
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
        // 使用包含 Signature 对象的文档路径
        Signature signature = new Signature("input.docx");

        // 实例化 StampSignOptions 并设置所需的签名文本
        StampSignOptions options = new StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // 添加一个或多个印章线
        StampLine outerLine = new StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(Color.WHITE);
        outerLine.setBackgroundColor(Color.BLUE);
        options.getOuterLines().add(outerLine);

        // 保存印章文档
        SignResult result = signature.sign("output.docx", options);
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "通过签名保护您的文档内容"
  description: "GroupDocs.Signature for Java 库旨在对流行文件格式进行签名和管理签名。轻松添加、修改、验证或删除印章和其他类型的签名。"
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "使用 GroupDocs.Signature 的印章签名"
  features:
    # feature loop
    - title: "对您的文档进行签名"
      content: "将可自定义的签名应用于文档的任何部分。从多种签名类型中选择，包括文本、图像、条形码、二维码和印章。此外，可以添加或修改隐藏的元数据以增强文档安全性。"

    # feature loop
    - title: "搜索和验证签名"
      content: "一旦文档被签名，使用我们的验证工具确保签名内容有效。搜索并检索所有签名的列表以进行进一步处理。"

    # feature loop
    - title: "根据需要更新签名"
      content: "轻松修改应用于文档的多种签名。更新诸如大小、颜色、位置、内容等属性。"

    # feature loop
    - title: "删除签名"
      content: "需要从文档中删除签名吗？我们的 API 完全支持签名删除，使您能够有效管理文档。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "使用特殊签名向文档添加自定义印章"
      content: |
        了解如何生成并将包含重要文本信息的自定义印章添加到文档中。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 提供要添加印章的文档
          Signature signature = new Signature("input.docx");

          // 实例化印章选项对象
          StampSignOptions options = new StampSignOptions();

          // 设置页面上的大小和位置
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setAllPages(true);

          // 添加一个或多个带有文本的外部圆形线
          StampLine outerLine1 = new StampLine();
          outerLine1.setText("* The best  choice *");
          outerLine1.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
          SignatureFont signatureFont1 = new SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName("Arial");
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(Color.WHITE);
          outerLine1.setBackgroundColor(Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // 添加一个或多个内部方形线
          StampLine innerLine1 = new StampLine();
          innerLine1.setText("Company #1");
          innerLine1.setTextColor(Color.RED);
          SignatureFont signFont1 = new SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);

          // 保存印章文档
          SignResult result = signature.sign("output.docx", options);
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
            link: "/examples/signature/formats/signature_stamp.docx"
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
    title: "探索我们的核心功能"
    exclude: "stamp"
    description: "利用多种选项添加、管理和删除签名。"
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
    title: "跨多种文件格式添加印章"
    exclude: "DOCX"
    description: "GroupDocs.Signature API 支持 60 多种格式的文件印章。在任何页面或区域放置印章，以改善文档管理和定制。"
    items: 
          
        # format loop 1
        - name: "盖章 PDF"
          format: "PDF"
          link: "/signature/java/stamp/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "盖章 DOCX"
          format: "DOCX"
          link: "/signature/java/stamp/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "盖章 JPEG"
          format: "JPEG"
          link: "/signature/java/stamp/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "盖章 PPTX"
          format: "PPTX"
          link: "/signature/java/stamp/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "盖章 XLSX"
          format: "XLSX"
          link: "/signature/java/stamp/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---