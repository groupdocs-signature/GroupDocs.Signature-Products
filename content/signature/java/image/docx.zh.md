



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:09
draft: false
lang: zh
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "使用 Java 向 DOCX 文件添加图像签名"
head_description: "使用几行代码在 Java 的 DOCX 文件上添加图像签名。使用 GroupDocs.Signature for Java API 添加图像。"

############################# Header ############################
title: "使用图像签名签署 DOCX 文件" 
description: "使用 GroupDocs.Signature for Java 将图像插入各种办公文件格式，包括 PDF、Word、Excel 和图像文件。带有老板签名的图像可以增添亮点！"
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
    title: "了解 GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) 提供在商业文档中的任何页面和位置添加图像签名的能力。通过在 PDF、Word 文档、Excel 电子表格、PowerPoint 演示文稿和常见图像格式中添加图像来优化您的工作流程。

############################# Steps ############################
steps:
    enable: true
    title: "通过 Java 在 DOCX 的任何位置添加图像的步骤"
    content: |
      [GroupDocs.Signature](/signature/java/) 为 Java 应用程序增强了向 DOCX 文档的任何页面添加签名的能力。通过集成我们的库，提高产品的功能。
      
      1. 创建包含 DOCX 文档的 Signature 实例。
      2. 使用 ImageSignOptions 指定签名图像。
      3. 将图像放置在任何页面的任意位置。
      4. 将已签署的文档保存到新位置。
   
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
        // 使用文档路径实例化 Signature
        Signature signature = new Signature("input.docx");

        // 使用图像创建 ImageSignOptions 作为签名
        ImageSignOptions options = new ImageSignOptions("company_logo.jpg");

        // 将图像放置在所有页面的左上角
        options.setAllPages(true);
        options.setLeft(100);
        options.setTop(200);

        // 保存已签署的文档
        SignResult result = signature.sign("output.docx", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "全面的文档签署解决方案"
  description: "我们的 API 支持一系列签署功能，使您能够添加、修改、删除、搜索和验证多种签名类型，包括图像签名。"
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "图像签名"
  features:
    # feature loop
    - title: "将图像插入办公文档"
      content: "轻松在文档的任何页面任何位置放置图像签名。使用文本、图像、条形码、元数据和数字证书丰富您的内容。"

    # feature loop
    - title: "签名搜索和验证"
      content: "轻松验证已签署文档中签名的有效性。检索文档中的所有签名列表，并检查每个签名的详细信息。"

    # feature loop
    - title: "修改签名"
      content: "更新之前添加到文档中的任何签名的内容、外观、大小或位置。我们的 API 使修改签名变得简单高效。"

    # feature loop
    - title: "移除不必要的签名"
      content: "我们的 API 支持大多数签名类型的完整 CRUD 操作。当需要时，您可以轻松地从几乎所有支持的文档类型中移除签名。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "使用图像签名增强文档内容"
      content: |
        学习如何将图像附加到商业文档中以提供额外信息。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 选择要签署的文档
          Signature signature = new Signature("input.docx");

          // 使用图像路径创建图像选项
          ImageSignOptions options = new ImageSignOptions("manager_signature.jpg");

          // 设置图像签名的大小
          options.setWidth(100);
          options.setHeight(100);

          // 将图像放置在右下角
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);

          // 如有必要，应用页面角落的边距
          Padding padding = new Padding();
          padding.setRight(120);
          padding.setBottom(120);
          options.setMargin(padding);

          // 如有需要，给图像添加自定义边框
          Border border = new Border();
          border.setColor(Color.RED);
          border.setDashStyle(DashStyle.DashDotDot);
          border.setWeight(5);
          border.setVisible(true);
          options.setBorder(border);

          // 旋转签名以更好地对齐
          options.setRotationAngle(45);

          // 将更新后的文档保存到任何位置
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
            link: "/examples/signature/formats/signature_image.docx"
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
    title: "查看我们的领先功能"
    exclude: "image"
    description: "我们很高兴为您展示多种签名工具和操作"
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
    title: "将图像添加到其他文件格式"
    exclude: "DOCX"
    description: "使用 Java API，您可以向各种文档中插入支持的图像格式。轻松调整大小、选择位置并向文档添加图像签名。"
    items: 
          
        # format loop 1
        - name: "使用图像签名 PDF"
          format: "PDF"
          link: "/signature/java/image/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "使用图像签名 DOCX"
          format: "DOCX"
          link: "/signature/java/image/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "使用图像签名 JPEG"
          format: "JPEG"
          link: "/signature/java/image/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "使用图像签名 PPTX"
          format: "PPTX"
          link: "/signature/java/image/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "使用图像签名 XLSX"
          format: "XLSX"
          link: "/signature/java/image/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---