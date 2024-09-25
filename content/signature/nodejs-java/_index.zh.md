---
############################# Static ############################
layout: "landing"
date: 2024-09-25T12:45:24
draft: false

lang: zh
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Node.js 数字签名 API - GroupDocs.Signature"
head_description: "将 Node.js 应用程序中的安全电子签名与 GroupDocs.Signature 集成。轻松高效地简化文档签名工作流程。"

############################# Header ############################
title: "签署文件 使用 Node.js API"
description: "使用我们面向程序员和最终用户的灵活的 API 和基于应用程序的解决方案，在任何平台上签署数字文档和图像。"
words:
  for: "为了"

actions:
  main: "从NPM下载"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "许可"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
  title: "准备好开始了吗？"
  description: "免费试用 GroupDocs.Signature 功能或申请许可证"

release:
  title: "版本 {0} 已发布"
  notes: "看看有什么新鲜事"
  downloads: "下载"

code:
  title: "通过 Node.js 签署 PDF"
  more: "更多示例"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // 选择PDF文档
    let signature = new Signature("sample.pdf");
    
    // 提供文字
    let options = new TextSignOptions("John Smith");
    
    // 设置颜色
    options.ForeColor = Color.Red;
    
    // 签署文档并保存到文件
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature 概述"
  description: "可在 Node.js 应用程序中使用的文档签名库"
  features:
    # feature loop
    - title: "使用 Node.js 的商业文档数字签名解决方案"
      content: "GroupDocs.Signature for Node.js via Java 为 PDF、Office 文档和图像提供了一整套数字签名选项。文本、条形码、图像、数字证书和元数据均可用。简化的文档处理确保效率。"

    # feature loop
    - title: "签名文档的高级操作"
      content: "GroupDocs.Signature 使您能够处理签名的文档。使用各种标准搜索和验证签名。此外，提取详细的文档信息或生成页面的预览图像。"

    # feature loop
    - title: "多种输出格式"
      content: "我们的解决方案提供对签名文档的输出格式的广泛控制。在任何页面上精确定位签名并自定义其外观。以多种受支持的格式保存签名文档，并可选择使用密码保护它们。"

############################# Platforms ############################
platforms:
  enable: true
  title: "平台独立性"
  description: "GroupDocs.Signature for Node.js via Java 使用各种操作系统执行文档处理"
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "支持的文件格式"
  description: |
    GroupDocs.Signature for Node.js via Java 有助于对[流行文件格式](https://docs.groupdocs.com/signature/java/supported-document-formats/) 进行操作。
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
  title: "GroupDocs.Signature 的功能"
  description: "使用数字签名签署 PDF、Office 文档和图像"

  items:
    # feature loop
    - icon: "sign"
      title: "商业签名"
      content: "采用各种签名类型来签署文档。将数字签名精确地放置在任何页面位置。"

    # feature loop
    - icon: "custom"
      title: "自定义签名外观"
      content: "通过调整颜色、字体、边框、旋转等来定制签名的视觉效果，以达到您想要的结果。"

    # feature loop
    - icon: "password"
      title: "受密码保护的文档"
      content: "对于许多受支持的文档格式，请使用密码保护签名文档以提高安全性。"

    # feature loop
    - icon: "protect"
      title: "防止未经授权的修改"
      content: "保护使用数字证书签名的重要业务文档免遭未经授权的更改。"

    # feature loop
    - icon: "convert"
      title: "所需的输出格式"
      content: "轻松获得任何受支持格式的签名文档。轻松将 MS Word 文档转换为 PDF 格式。"

    # feature loop
    - icon: "preview"
      title: "文件预览"
      content: "将各个文档页面保存为图像以供将来需要。"

    # feature loop
    - icon: "search"
      title: "签名搜索"
      content: "检索有关文档中先前添加的签名的信息。"

    # feature loop
    - icon: "validate"
      title: "文件验证"
      content: "验证任何文档中签名的真实性。"

    # feature loop
    - icon: "update"
      title: "签名管理"
      content: "删除、重新定位或修改任何文档页面上的任何签名。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "代码示例"
  description: "展示典型 GroupDocs.Signature for Node.js via Java 操作的说明性示例"
  items:
    # code sample loop
    - title: "使用二维码标记 PDF"
      content: |
        将[条形码](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/)合并到特定的PDF文档页面可以简化业务流程。 本节提供使用 GroupDocs.Signature for Node.js via Java 添加 QR 码的示例。
        {{< landing/code title="如何将二维码转为 PDF。">}}
        ```javascript {style=abap}
        // 加载要签名的文档
        let signature = new Signature("file_to_sign.pdf");
        
        // 使用预定义文本创建 QR 码选项
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // 配置二维码编码类型以及在页面中的位置
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // 签署文档并将其保存为结果文件
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "使用数字签名保护 DOCX"
      content: |
        通过基于数字证书的签名来[保护您的文档](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/)。 数字签名可保护您的业务文档免遭内容更改。
        {{< landing/code title="以下是如何确保文档完整性。">}}
        ```javascript {style=abap}   
        // 加载要进行数字签名的文档
        let signature = new Signature("file_to_sign.docx");
        
        // 指定数字签名选项并提供证书文件的路径
        let options = new DigitalSignOptions("certificate.pfx");

        // 设置证书密码
        options.Password = "1234567890";

        // 签署文档并将其保存到所需路径
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
