---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:01
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: zh
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Net"
platform_tag: "net"

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

############################# Head ############################
head_title: ".NET、Java、云 API 和在线文档签名应用程序"
head_description: "获得适用于 .NET、Java 和基于云的应用程序的一体化文档电子签名解决方案。使用简单的拖放功能在线签署常见文档格式"

############################# Header ############################
title: "签署文件<br>通过.NET API"
description: "使用我们面向程序员和最终用户的灵活的 API 和基于应用程序的解决方案，在任何平台上签署数字文档和图像。"
words:
  for: "为了"

actions:
  main: "免费 NuGet 下载"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "许可"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "准备好开始了吗？"
  description: "免费试用 GroupDocs.Signature 功能或申请许可证"

release:
  title: "版本 {0} 已发布"
  notes: "看看有什么新鲜事"
  downloads: "下载"

code:
  title: "在 C# 中签署 PDF 文件"
  more: "更多示例"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // 选择PDF文档
    using (Signature signature = new Signature("sample.pdf"))
    {
        // 提供文字
        var options = new TextSignOptions("John Smith")
        {
            // 设置颜色
            ForeColor = Color.Red
        };
        // 签署文档并保存到文件
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature 概述"
  description: "用于在 .NET 应用程序中执行文档签名和相关操作的 API"
  features:
    # feature loop
    - title: "使用 C# 为业务文档添加签名"
      content: "文档签名：使用 GroupDocs.Signature for .NET，您可以向 PDF 和 Office 文档添加各种类型的签名，例如文本、图像、条形码和数字证书。此 API 允许您使用几乎任何数据类型（包括隐藏元数据）对文档进行签名。"

    # feature loop
    - title: "处理签署的文件"
      content: "附加处理：您可以使用 GroupDocs.Signature 对签名文档执行强大的操作。这包括搜索业务文档中的现有签名并使用特定标准验证它们。此外，您还可以通过此 .NET API 检索文档信息和预览页面。"

    # feature loop
    - title: "定制结果"
      content: "GroupDocs.Signature for .NET 提供了广泛的自定义选项。您可以将签名精确地放置在文档页面上的任何位置，并使用各种设置调整其外观。此外，该 API 支持以多种受支持的格式保存已处理的文档。"

############################# Platforms ############################
platforms:
  enable: true
  title: "平台独立性"
  description: "GroupDocs.Signature for .NET 支持以下操作系统、框架和包管理器"
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
    GroupDocs.Signature for .NET 支持使用以下[文件格式](https://docs.groupdocs.com/signature/net/supported-document-formats/) 进行操作。
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
  description: "快速准确地签署 PDF、Office 文档和图像"

  items:
    # feature loop
    - icon: "sign"
      title: "文件签署"
      content: "在业务文档的任何指定位置准确添加一种或多种支持类型的签名。"

    # feature loop
    - icon: "custom"
      title: "自定义签名"
      content: "利用颜色、字体、边框、旋转等功能来配置签名的外观。"

    # feature loop
    - icon: "password"
      title: "文档密码保护"
      content: "通过在签名后设置密码来保护某些文档类型。"

    # feature loop
    - icon: "protect"
      title: "防止变化"
      content: "附加数字证书签名后，防止重要业务文档发生更改。"

    # feature loop
    - icon: "convert"
      title: "将签名文件转换为其他格式"
      content: "将签名文件转换为所需格式，例如将 Word 文档另存为 PDF。"

    # feature loop
    - icon: "preview"
      title: "提取页面预览"
      content: "从签名文档中提取页面作为单独的图像以供将来处理。"

    # feature loop
    - icon: "search"
      title: "文档中的签名搜索"
      content: "检索有关特定文档中先前添加的签名的信息。"

    # feature loop
    - icon: "validate"
      title: "验证签署的文件"
      content: "使用验证功能验证文档的正确签名。"

    # feature loop
    - icon: "update"
      title: "更新或删除签名"
      content: "轻松地在页面上重新定位特定签名、修改其文本或删除它们，没有任何问题。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "代码示例"
  description: ".NET 操作的典型 GroupDocs.Signature 的一些用例"
  items:
    # code sample loop
    - title: "将 QR 码添加到 PDF"
      content: |
        将 [QR 码](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) 添加到 PDF 文档的特定页面可以增强业务流程。 以下是如何使用 GroupDocs.Signature 添加 QR 码的示例。
        {{< landing/code title="如何将二维码转为 PDF。">}}
        ```csharp {style=abap}
        // 加载要签名的文档
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // 使用预定义文本创建 QR 码选项
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // 配置二维码编码类型以及在页面中的位置
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // 签署文档并将其保存为结果文件
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "使用数字证书保护 DOCX 文档"
      content: |
        您可以使用存储为数字证书的个人或公司签名来[保护文档](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/)。 此类受保护的文档无法在不使签名无效的情况下进行修改。
        {{< landing/code title="以下是如何确保文档完整性。">}}
        ```csharp {style=abap}   
        // 加载要进行数字签名的文档
        using (Signature signature = new Signature("file_to_sign.docx"))
        {
            // 指定数字签名选项并提供证书文件的路径
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // 设置证书密码
                Password = "1234567890"
            };
            // 签署文档并将其保存到所需路径
            signature.Sign("digitally_signed.docx", options);
        }
        ```
        {{< /landing/code >}}

---
