



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:32
draft: false
lang: zh
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "使用 Java 在 XLSX 中搜索数字签名"
head_description: "利用 GroupDocs.Signature for Java API 在 XLSX 文件中搜索签名。在 PDF、Word、Excel、演示文稿和图像中查找签名。"

############################# Header ############################
title: "在 XLSX 中搜索数字签名" 
description: "使用 GroupDocs.Signature for Java 检索嵌入在 PDF、Word、Excel、演示文稿或图像文件中的电子签名完整列表。"
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
       [GroupDocs.Signature for Java](/signature/java/) 提供强大的文件签名功能。它支持向60多种格式的文件添加文本、图像、条形码、数字证书和印章，包括 PDF、MS Office 文档、图像、ZIP 文件和其他常见业务格式。此外，您可以随时搜索、验证、修改或删除签名。

############################# Steps ############################
steps:
    enable: true
    title: "使用 Java 搜索 XLSX 签名的步骤"
    content: |
      [GroupDocs.Signature](/signature/java/) 提供强大的引擎来搜索 XLSX 文件中的任何数字签名。Java 开发人员可以有效地增强他们的应用程序。
      
      1. 提供 XLSX 文件路径以进行签名搜索。
      2. 使用 SearchOptions 来细化搜索结果。
      3. 执行搜索方法以获取结果。
      4. 分析找到的签名列表。
   
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

        // 使用文档路径创建 Signature 实例
        final Signature signature = new Signature("input.xlsx");

        // 实例化 TextSearchOptions 以覆盖所有页面
        TextSearchOptions options = new TextSearchOptions();
        options.setAllPages(true);

        // 搜索文档中的文本签名
        List<TextSignature> signatures = signature.search(TextSignature.class, options);
        System.out.print("\nSource document contains following text signature(s).");

        // 列出找到的签名以进行进一步分析
        for (TextSignature textSignature : signatures) {
            System.out.print("Found Text signature at page " + textSignature.getPageNumber() 
                + " with type [" + textSignature.getSignatureImplementation() + "] and 
                text '" + textSignature.getText() + "'.");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "全面的文档签名解决方案"
  description: "我们自豪地推出与所有主要文档格式兼容的签名解决方案。添加多种签名增强您的文档或保护其内容。"
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "签名搜索"
  features:
    # feature loop
    - title: "签署业务文档"
      content: "在文档的任意页中任意位置插入数字签名。使用多种签名类型，如文本、图像、条形码、元数据、印章或数字证书。"

    # feature loop
    - title: "管理签名"
      content: "签署后，文档可能需要进一步处理。搜索所有可用签名，并在必要时更新或删除它们。"

    # feature loop
    - title: "保护文档内容"
      content: "管理嵌入文档的隐藏元数据。添加新元数据或删除现有条目。使用企业数字证书保护文档内容不被未经授权的更改。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "搜索图像签名"
      content: |
        此示例演示如何在特定文档中找到图像签名。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 将源文档作为构造函数参数传入
          final Signature signature = new Signature("input.xlsx");

          // 搜索任何文本类型的签名
          List<ImageSignature> signatures = signature.search(ImageSignature.class, SignatureType.Image);
          System.out.print("\nSource document contains following image signature(s).");

          // 显示找到的签名的属性结果
          for (ImageSignature imageSignature : signatures)
          {
              System.out.print("Image signature found at page "+imageSignature.getPageNumber()+
                    " with size "+imageSignature.getSize()+". Created "+imageSignature.getCreatedOn()+
                    ", modified "+imageSignature.getModifiedOn());
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
    title: "支持的操作"
    exclude: "search"
    description: "我们的产品提供灵活的 API，用于签署文档和在签署后管理签名。"
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
    title: "在各种文件格式中搜索签名"
    exclude: "XLSX"
    description: "GroupDocs.Signature for Java API 使您能够从任何已签署的文件中检索签名列表。提取流行文件格式中的签名以进行进一步处理。"
    items: 
          
        # format loop 1
        - name: "搜索 PDF 中的签名"
          format: "PDF"
          link: "/signature/java/search/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "查找 DOCX 中的签名"
          format: "DOCX"
          link: "/signature/java/search/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "查找 PPTX 中的签名"
          format: "PPTX"
          link: "/signature/java/search/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 4
        - name: "搜索 XLSX 中的签名"
          format: "XLSX"
          link: "/signature/java/search/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---