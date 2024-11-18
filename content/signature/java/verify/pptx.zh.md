



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:15
draft: false
lang: zh
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "使用 Java 验证 PPTX 电子签名"
head_description: "GroupDocs.Signature for Java 可用于验证位于 PPTX 文件中的签名。 验证 PDF、Word 文档、Excel 表格、演示文稿、图像或 ZIP 存档中的签名。"

############################# Header ############################
title: "用于 PPTX 的电子签名验证" 
description: "使用 GroupDocs.Signature for Java 验证 PDF、Word、Excel、演示文稿、图像或 ZIP 文件中所有支持的电子签名。"
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "下载免费版"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Java 的应用"
    link: "/signature/java/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) 支持文档签名及更多功能的完整 CRUD 操作。 签署 60 种以上的文档格式，包括 PDF、MS Office 文件、图像和 ZIP 存档，支持文本、图像、条形码、数字证书、元数据和印章等多种类型。 还提供搜索、验证、修改或删除签名等附加操作。

############################# Steps ############################
steps:
    enable: true
    title: "使用 Java 验证 PPTX 中的签名的步骤"
    content: |
      [GroupDocs.Signature](/signature/java/) 可以验证 PPTX 文档中特定签名的存在。 Java 开发者可以通过添加我们解决方案提供的功能来增强其应用程序。
      
      1. 将 PPTX 文件加载到 Signature 实例中。
      2. 实例化并配置 VerifyOptions 以实现所需结果。
      3. 启动验证过程。
      4. 审查验证结果。
   
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
        // 实例化带有文档的 Signature
        Signature signature = new Signature("input.pptx");

        // 创建 TextVerifyOptions 以验证包含特定文本的签名
        TextVerifyOptions options = new TextVerifyOptions();
        options.setText("signature");
        options.setMatchType(TextMatchType.Contains);

        // 验证文档中的签名
        VerificationResult result = signature.verify(options);

        // 处理验证结果
        if (result.isValid())
        {
            System.out.print("\nDocument was verified successfully!");
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "全面的文档签名解决方案"
  description: "GroupDocs.Signature 通过 7 种类型的签名和完整的 CRUD 操作增强了流行的办公文档格式，为您的文档内容提供了强有力的保护。"
  image: "/img/signature/features_verify.webp" # 500x500 px
  image_description: "签名验证"
  features:
    # feature loop
    - title: "签署企业文档"
      content: "为任何文档添加专业数字签名。 我们的解决方案支持多种类型的签名，包括文本、图像、条形码、元数据、印章和数字证书。"

    # feature loop
    - title: "签名 CRUD 操作"
      content: "在许多情况下，已签署的文档需要进一步处理。 检索文档中所有签名的列表，验证它们，修改其属性，或在必要时将其删除。"

    # feature loop
    - title: "保护文档内容"
      content: "使用数字证书保护企业文档，以防止未经授权的更改。 嵌入隐含元数据以进一步保护文档内容。"

    # feature loop
    - title: "本机签名"
      content: "利用特定于文档的文本签名，例如 PDF 印章或 Word 水印，为企业用途创建量身定制的专业文档。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "验证条形码签名"
      content: |
        本示例演示如何验证文档中的条形码签名。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 提供包含条形码签名的文档
          final Signature signature = new Signature("input.pptx");

          // 配置选项以根据特定文本验证条形码
          BarcodeVerifyOptions options = new BarcodeVerifyOptions();
          options.setText("12345");
          options.setMatchType(TextMatchType.StartsWith);

          // 验证施加于文档的签名
          VerificationResult result = signature.verify(options);

          // 显示验证结果
          if (result.isValid())
          {
              System.out.print("\nDocument was verified successfully!");
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
    title: "支持的操作和签名类型"
    exclude: "verify"
    description: "探索 GroupDocs.Signature 支持的所有功能和签名操作。"
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
          
############################# More Formats #####################
more_formats:
    enable: true
    title: "跨文件格式的签名验证"
    exclude: "PPTX"
    description: "GroupDocs.Signature for Java 简化了验证文档中所有签名的过程。 设置自定义验证参数以确保已签署文档的完整性。"
    items: 
          
        # format loop 1
        - name: "验证 PDF 签名"
          format: "PDF"
          link: "/signature/java/verify/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "验证 DOCX 签名"
          format: "DOCX"
          link: "/signature/java/verify/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "验证 PPTX 签名"
          format: "PPTX"
          link: "/signature/java/verify/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 4
        - name: "验证 XLSX 签名"
          format: "XLSX"
          link: "/signature/java/verify/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---