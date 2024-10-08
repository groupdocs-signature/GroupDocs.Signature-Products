---
############################# Static ############################
layout: "landing"
date: 2024-09-25T12:45:24
draft: false

lang: zh
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java" 
    # supported_platforms loop
    - title: "Python"
      tag: "python-net" 

############################# Head ############################
head_title: "Java 数字签名库 - GroupDocs.Signature"
head_description: "通过 GroupDocs.Signature 的电子签名为 Java 应用程序提供支持。快速、轻松地签署商业文件。"

############################# Header ############################
title: "签署文件 通过Java API"
description: "使用我们面向程序员和最终用户的灵活的 API 和基于应用程序的解决方案，在任何平台上签署数字文档和图像。"
words:
  for: "为了"

actions:
  main: "免费 Maven 下载"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "许可"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "准备好开始了吗？"
  description: "免费试用 GroupDocs.Signature 功能或申请许可证"

release:
  title: "版本 {0} 已发布"
  notes: "看看有什么新鲜事"
  downloads: "下载"

code:
  title: "使用 Java 签署 PDF 文件"
  more: "更多示例"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // 选择PDF文档
    Signature signature = new Signature("sample.pdf");
    
    // 提供文字
    TextSignOptions options = 
        new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // 签署文档并保存到文件
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature 概述"
  description: "用于在 Java 应用程序中执行文档签名和相关操作的 API"
  features:
    # feature loop
    - title: "使用 Java 数字签名改进业务文档"
      content: "快速且可定制的签名：GroupDocs.Signature for Java 为 PDF、图像和 Office 文档提供了广泛的数字签名选项。您可以使用文本、条形码、QR 码、数字证书、图片或隐藏元数据。文件处理快速高效。"

    # feature loop
    - title: "处理已签署的文件"
      content: "高级文档处理涉及使用 GroupDocs.Signature for Java 对签名文档进行强大的操作。您可以使用各种有用的条件搜索并验证已添加到业务文档中的签名。此外，您还可以访问有关文档的详细信息或获取其页面的预览图像。"

    # feature loop
    - title: "多种输出选择"
      content: "强大的签名选项允许您自定义使用 GroupDocs.Signature for Java 签名的文档的输出。您可以在任何文档页面上精确定位任何签名，并以多种方式配置其外观。 Java API 支持以多种受支持的格式保存签名的业务文档，并提供使用密码保护它们的选项。"

############################# Platforms ############################
platforms:
  enable: true
  title: "平台独立性"
  description: "GroupDocs.Signature for Java 支持以下操作系统、框架和包管理器"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "支持的文件格式"
  description: |
    GroupDocs.Signature for Java 支持以下[文件格式](https://docs.groupdocs.com/signature/java/supported-document-formats/) 的操作。
  groups:
    # group loop
    - color: "green"
      content: |
        ### 微软Office格式
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### 图像和其他格式
        * **便携的:** PDF
        * **图片:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **其他办公形式:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### 其他格式
        * **网络:** HTML, MHTML
        * **档案:** ZIP, TAR, 7Z
        * **证书:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Signature 功能"
  description: "使用数字签名签署 PDF、Office 文档和图像"

  items:
    # feature loop
    - icon: "sign"
      title: "添加签名"
      content: "通过将数字签名精确地放置在任何页面上的任何位置，使用各种支持的签名类型来签署文档。"

    # feature loop
    - icon: "custom"
      title: "定制结果"
      content: "通过调整颜色、字体、边框、旋转和其他功能来自定义签名外观，以达到所需的结果。"

    # feature loop
    - icon: "password"
      title: "使用密码保护文档"
      content: "对于许多受支持的文档类型，您可以使用密码保护签名文档。"

    # feature loop
    - icon: "protect"
      title: "防止未经授权的更改"
      content: "保护使用数字证书签名的重要业务文档免遭未经授权的修改。"

    # feature loop
    - icon: "convert"
      title: "获得所需格式的结果"
      content: "轻松获取任何受支持格式的签名结果文件。您还可以轻松地将 MS Word 文档转换为 PDF。"

    # feature loop
    - icon: "preview"
      title: "文档预览"
      content: "将文档的任何页面保存为图像以供将来处理。"

    # feature loop
    - icon: "search"
      title: "寻找签名"
      content: "可以获得有关特定文档中先前添加的签名的信息。"

    # feature loop
    - icon: "validate"
      title: "验证文件"
      content: "验证任何已签名文档上签名的正确性。"

    # feature loop
    - icon: "update"
      title: "管理签名"
      content: "将签名放置在文档页面上后，可以根据需要将其删除、移动或更新。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "代码示例"
  description: "Java 操作的典型 GroupDocs.Signature 的一些用例"
  items:
    # code sample loop
    - title: "使用 QR 码增强 PDF 文档"
      content: |
        通过将 [QR](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) 码添加到 PDF 文档的特定页面来增强业务流程可能很有价值。 有一个示例说明如何使用 GroupDocs.Signature for Java 添加 QR 码。
        {{< landing/code title="使用 QR 码增强 PDF 文档">}}
        ```java {style=abap}
        // 加载要签名的文档
        Signature signature = new Signature("file_to_sign.pdf");
        
        // 使用预定义文本创建 QR 码选项
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // 配置二维码编码类型以及在页面中的位置
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // 签署文档并将其保存为结果文件
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "使用数字签名来保护 DOCX"
      content: |
        您可以使用存储为数字证书的个人或公司签名来[保护文档](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/)。 在不使签名无效的情况下，无法更改使用证书保护的文档。
        {{< landing/code title="使用数字签名来保护 DOCX">}}
        ```java {style=abap}   
        // 加载要进行数字签名的文档
        Signature signature = new Signature("file_to_sign.docx");
        
        // 指定数字签名选项并提供证书文件的路径
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // 设置证书密码
        options.setPassword("1234567890");

        // 签署文档并将其保存到所需路径
        signature.sign("digitally_signed.docx", options);
        ```
        {{< /landing/code >}}

---