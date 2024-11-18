



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:54
draft: false
lang: zh
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "使用 Java 创建 PPTX 文本签名"
head_description: "利用 Java API 将文本签名插入 PPTX 文件。无缝处理常见文档格式，包括 PDF、Word、Excel、演示文稿、图像和 ZIP。"

############################# Header ############################
title: "为 PPTX 创建文本签名" 
description: "使用 GroupDocs.Signature for Java 轻松向您的商业文档添加自定义文本签名。通过签名定制选项简化组织工作流程。"
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费开始"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Java 解决方案简介"
    link: "/signature/java/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) 提供灵活且可定制的文本签名，以简化您的文档管理任务。配置文本签名的内容和设计，并将其应用于任何页面，从而提高组织的文档工作流程。

############################# Steps ############################
steps:
    enable: true
    title: "使用 Java 向 PPTX 添加文本签名的步骤"
    content: |
      [GroupDocs.Signature](/signature/java/) 可以集成到 Java 应用程序中，以向 PPTX 文档添加文本签名。开发人员可以通过使用我们的解决方案迅速增强产品功能。
      
      1. 将 PPTX 文档作为 Signature 类构造函数的参数。
      2. 使用适当的文本实例化 TextSignOptions。
      3. 配置签名的视觉选项。
      4. 将文本签名添加到文档的任意页面。
   
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
        // 将文档路径传递给 Signature 构造函数
        Signature signature = new Signature("input.pptx");

        // 使用签名文本实例化 TextSignOptions
        TextSignOptions options = new TextSignOptions("Approved");
        
        // 设置文本颜色和字体属性
        options.setForeColor(Color.RED);
        SignatureFont signatureFont = new SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName("Comic Sans MS");
        options.setFont(signatureFont);

        // 将文本签名附加到文档
        SignResult result = signature.sign("output.pptx", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "管理文档文本签名"
  description: "使用 GroupDocs.Signature for Java，您可以通过向常见文件格式添加文本签名来简化公司的文档工作流程。轻松配置签名的外观和内容。"
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "GroupDocs.Signature 的主要特性"
  features:
    # feature loop
    - title: "文档签名"
      content: "将文本、图像、条形码、二维码或印章签名应用于支持文档的任何页面。利用元数据嵌入隐藏内容，并使用数字证书保护您的文档。"

    # feature loop
    - title: "签名搜索和验证"
      content: "使用我们的签名验证工具确保已签名文档的完整性。您还可以检索和搜索文档中的所有嵌入签名。"

    # feature loop
    - title: "修改或删除签名"
      content: "修改之前添加的签名的内容、位置和外观，或将其从文档中完全删除。"

    # feature loop
    - title: "本地文本签名"
      content: "添加特定于文档的文本签名，例如 PDF 中的贴纸或 Word 文档中的水印，以增强自定义效果。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "使用文本签名标记文档"
      content: |
        了解如何向商业文档附加文本信息以改善业务流程。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 选择要签名的文档
          Signature signature = new Signature("input.pptx");

          // 创建带有所需文本的文本选项
          TextSignOptions options = new TextSignOptions("Rescheduled to 03/04/2025");

          // 指定签名在页面上的大小和位置
          options.setLeft(100);
          options.setTop(180);
          options.setWidth(230);
          options.setHeight(30);

          // 签名支持距离页面角落的填充
          Padding padding = new Padding();
          padding.setBottom(20);
          padding.setRight(20);
          options.setMargin(padding);

          // 文本颜色和字体样式可以自定义
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);

          // 文本签名可以包含边框
          Border border = new Border();
          border.setColor(Color.RED);
          border.setDashStyle(DashStyle.Dash);
          border.setTransparency(0.5);
          border.setVisible(true);
          border.setWeight(2);
          options.setBorder(border);

          // 也可以进行背景自定义
          Background background = new Background();
          background.setColor(Color.YELLOW);
          background.setTransparency(0.8);
          options.setBackground(background);

          // 文本可以作为图像保存以提高兼容性
          options.setSignatureImplementation(TextSignatureImplementation.Image);

          // 保存添加了文本的文档
          SignResult result = signature.sign("output.pptx", options);
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
            link: "/examples/signature/formats/signature_text.pptx"
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
    title: "关键特性和签名选项"
    exclude: "text"
    description: "我们的解决方案支持七种不同类型的签名的完整 CRUD 操作以及更多功能。"
    items: 
          
        # operation loop 1
        - name: "电子签名"
          operation: "esign"
          link: "/signature/java/esign/pptx/"
          description: "向支持的文件格式添加各种类型的签名"

        # operation loop 2
        - name: "向文档添加文本"
          operation: "text"
          link: "/signature/java/text/pptx/"
          description: "通过可自定义的文本签名增强文档内容"

        # operation loop 3
        - name: "图像签名"
          operation: "image"
          link: "/signature/java/image/pptx/"
          description: "在文档内的任意位置放置任何图像"

        # operation loop 4
        - name: "生成条形码"
          operation: "barcode"
          link: "/signature/java/barcode/pptx/"
          description: "创建并插入各种条形码到支持的文档中"

        # operation loop 5
        - name: "生成二维码"
          operation: "qrcode"
          link: "/signature/java/qrcode/pptx/"
          description: "生成用于文档签名的二维码"
          
        # operation loop 6
        - name: "数字证书"
          operation: "digital"
          link: "/signature/java/digital/pptx/"
          description: "安全地进行商业操作并使用数字证书签署文档"

        # operation loop 7
        - name: "盖章签名"
          operation: "stamp"
          link: "/signature/java/stamp/pptx/"
          description: "使用盖章构造器创建自定义圆形或方形印章"
          
        # operation loop 8
        - name: "搜索签名"
          operation: "search"
          link: "/signature/java/search/pptx/"
          description: "在文档中定位任何之前添加的签名"
          
        # operation loop 9
        - name: "签名验证"
          operation: "verify"
          link: "/signature/java/verify/pptx/"
          description: "验证签名在应用后是否真实有效"
          
        # operation loop 10
        - name: "修改签名"
          operation: "modify"
          link: "/signature/java/modify/pptx/"
          description: "轻松编辑文档中的多种签名"
          
        # operation loop 11
        - name: "删除签名"
          operation: "delete"
          link: "/signature/java/delete/pptx/"
          description: "移除多种之前应用的签名"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "向各种文件格式添加文本签名"
    exclude: "PPTX"
    description: "利用 Java API 将文本签名插入 Office 文档，确保在文档生命周期的每个阶段完全控制内容。"
    items: 
          
        # format loop 1
        - name: "PDF 文本签名"
          format: "PDF"
          link: "/signature/java/text/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "DOCX 文本签名"
          format: "DOCX"
          link: "/signature/java/text/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "JPEG 文本签名"
          format: "JPEG"
          link: "/signature/java/text/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "PPTX 文本签名"
          format: "PPTX"
          link: "/signature/java/text/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "XLSX 文本签名"
          format: "XLSX"
          link: "/signature/java/text/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---