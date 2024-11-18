



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:09
draft: false
lang: zh
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "使用 Java 应用程序为 XLSX 文件电子签名"
head_description: "使用 Java API 处理 XLSX 文件并应用各种签名类型，包括 PDF、Word、Excel、演示文稿和图片。"

############################# Header ############################
title: "针对 XLSX 的电子签名" 
description: "使用 GroupDocs.Signature for Java 为所有流行的商业格式添加多种电子签名，包括 PDF、Word、Excel、演示文稿和图片。"
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
    title: "关于 GroupDocs.Signature for Java API"
    link: "/signature/java/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) 提供先进的电子签名功能。可以在文档和图像中添加、搜索、验证、修改和删除各种类型的电子签名，无需外部软件。轻松地对 PDF、Word 文档、Excel 表格、PowerPoint 演示文稿和流行图像格式进行电子签名。

############################# Steps ############################
steps:
    enable: true
    title: "使用 Java 签署 XLSX 的步骤"
    content: |
      [GroupDocs.Signature](/signature/java/) 使得向 XLSX 文件添加自定义签名成为可能。Java 开发者可以使用我们的软件将签署功能集成到他们的应用程序中。
      
      1. 将要签名的 XLSX 文件提供给 Signature 实例。
      2. 使用 SignOptions 定义签名详细信息。
      3. 自定义诸如大小、颜色和内容等各种属性。
      4. 将签名文件保存到所需位置。
   
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
        // 将文档加载到 Signature 实例中
        Signature signature = new Signature("input.xlsx");

        // 实例化 QrCodeSignOptions 对象
        QrCodeSignOptions options = new QrCodeSignOptions("QR code text");

        // 配置所有期望的选项
        options.setLeft(100);
        options.setTop(100);
        options.setForeColor(Color.RED);

        // 将添加二维码的文件保存到本地磁盘
        signature.sign("output.xlsx", options);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "文档电子签名"
  description: "我们的电子签名 API 精简了商业流程。可以以编程方式签署、搜索、更新、删除和验证各种签名。"
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "电子签名"
  features:
    # feature loop
    - title: "对办公文档进行电子签名"
      content: "可以将电子签名放置在文档的任何页面上的任何位置。使用文本、图像、条形码、元数据或数字证书增强文档内容。"

    # feature loop
    - title: "签名管理"
      content: "签名后，可以进一步处理文档。可以检索存在的所有签名列表，修改或根据需要删除它们。"

    # feature loop
    - title: "高级内容控制"
      content: "通过公司数字证书保护业务文档免受未授权更改的影响。添加或提取所有文档类型中的隐藏元数据条目。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "如何将图像签名添加到文档"
      content: |
        本示例演示如何在文档的特定页面上放置图像签名。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 将源文档作为参数提供
          Signature signature = new Signature("input.xlsx");

          // 在签名选项中指定图像路径
          ImageSignOptions options = new ImageSignOptions("image.jpg");

          // 设置图像的大小和目标页面
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setHeight(150);
          options.setWidth(200);
          Padding padding = new Padding(50);
          options.setMargin(padding);
          options.setAllPages(true);

          // 将签名应用于文档
          signature.sign("output.xlsx", options);

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
            link: "/examples/signature/formats/signature_esign.xlsx"
        links:
          #  loop
          - title: "更多示例"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "文档"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################## Actions ############################

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
    title: "探索我们的关键功能"
    exclude: "esign"
    description: "我们自豪地提供广泛支持的签名和操作。"
    items: 
          
        # operation loop 1
        - name: "电子签名"
          operation: "esign"
          link: "/signature/java/esign/xlsx/"
          description: "向支持的文件格式添加各种类型的签名"

        # operation loop 2
        - name: "向文档添加文本"
          operation: "text"
          link: "/signature/java/text/xlsx/"
          description: "通过可自定义的文本签名增强文档内容"

        # operation loop 3
        - name: "图像签名"
          operation: "image"
          link: "/signature/java/image/xlsx/"
          description: "在文档内的任意位置放置任何图像"

        # operation loop 4
        - name: "生成条形码"
          operation: "barcode"
          link: "/signature/java/barcode/xlsx/"
          description: "创建并插入各种条形码到支持的文档中"

        # operation loop 5
        - name: "生成二维码"
          operation: "qrcode"
          link: "/signature/java/qrcode/xlsx/"
          description: "生成用于文档签名的二维码"
          
        # operation loop 6
        - name: "数字证书"
          operation: "digital"
          link: "/signature/java/digital/xlsx/"
          description: "安全地进行商业操作并使用数字证书签署文档"

        # operation loop 7
        - name: "盖章签名"
          operation: "stamp"
          link: "/signature/java/stamp/xlsx/"
          description: "使用盖章构造器创建自定义圆形或方形印章"
          
        # operation loop 8
        - name: "搜索签名"
          operation: "search"
          link: "/signature/java/search/xlsx/"
          description: "在文档中定位任何之前添加的签名"
          
        # operation loop 9
        - name: "签名验证"
          operation: "verify"
          link: "/signature/java/verify/xlsx/"
          description: "验证签名在应用后是否真实有效"
          
        # operation loop 10
        - name: "修改签名"
          operation: "modify"
          link: "/signature/java/modify/xlsx/"
          description: "轻松编辑文档中的多种签名"
          
        # operation loop 11
        - name: "删除签名"
          operation: "delete"
          link: "/signature/java/delete/xlsx/"
          description: "移除多种之前应用的签名"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "使用电子签名签署流行的文件格式"
    exclude: "XLSX"
    description: "针对 Java 的电子签名 API 能够处理所有现代商业文件格式和文档格式。"
    items: 
          
        # format loop 1
        - name: "电子签名 PDF"
          format: "PDF"
          link: "/signature/java/esign/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "电子签名 DOCX"
          format: "DOCX"
          link: "/signature/java/esign/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "电子签名 JPEG"
          format: "JPEG"
          link: "/signature/java/esign/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "电子签名 PPTX"
          format: "PPTX"
          link: "/signature/java/esign/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "电子签名 XLSX"
          format: "XLSX"
          link: "/signature/java/esign/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---