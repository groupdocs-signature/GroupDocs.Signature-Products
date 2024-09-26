---
############################# Static ############################
layout: "family"
date:  2024-09-26T13:44:48
draft: false

product: "Signature"
product_tag: "signature"

lang: zh

############################# Head ############################
head_title: "C# .NET、Java、Node.js 数字签名应用程序"
head_description: "将 .NET、Java 或 Node.js 应用程序中的电子签名与 GroupDocs.Signature 集成。签署流行的商业文档格式。"

############################# Header ############################
title: "文档电子签名解决方案"
description:  |
  使用我们为程序员和最终用户提供的灵活 API 和基于应用程序的解决方案，在任何平台上签署数字文档和图像。

  使用高级方法搜索和修改以前添加的签名。

  使用数字证书保护文档免受更改并控制隐藏的元数据。

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "选择您的平台"
  title: "平台独立性"
  description: "GroupDocs.Signature 库支持以下操作系统和框架："
  details_link_title: "了解更多"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Signature .NET 
      color: "blue"
      tag: "net"
      link: "/signature/net/"
      features_link: "https://docs.groupdocs.com/signature/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.6.2 or higher <br> .NET Core 3.0 or higher <br> .NET 6.0 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS <br> Microsoft Azure
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Signature Java
      color: "red"
      tag: "java"
      link: "/signature/java/"
      features_link: "https://docs.groupdocs.com/signature/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 8 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Signature Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/signature/nodejs-java/"
      features_link: "https://docs.groupdocs.com/signature/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> 任何其他文本编辑器
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

    # items loop
    - title: "Python"
      description: GroupDocs.Signature Python
      color: "yellow"
      tag: "python-net"
      link: "/signature/python-net/"
      features_link: "https://docs.groupdocs.com/signature/python-net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Python 3.9+ and .Net 6+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IDLE <br> PyCharm <br> Visual Studio Code
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Signature 主要功能"
  description: "我们的解决方案旨在向流行的文档和文件格式添加各种类型的签名。轻松丰富您的业务流程。"

  items:
    # items loop
    - icon: "additional"
      title: "通过签名丰富您的数据"
      content: "将文本、图像、水印等附加到您的业务文档中。"

    # items loop
    - icon: "protect"
      title: "保护文档内容"
      content: "通过使用数字证书密封来禁止文档更改。"

    # items loop
    - icon: "search"
      title: "添加隐藏数据和条形码"
      content: "使用元数据存储不可见信息或在页面上放置自定义条形码。"

    # items loop
    - icon: "manipulate"
      title: "操纵签名"
      content: "搜索、更新或删除之前添加的所有签名。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "使用签名保护您的文件"
  description: "GroupDocs.Signature 代码示例"
  items:
    # code sample loop
    - title: "生成并添加二维码"
      content: |
       GroupDocs.Signature 允许我们生成 QR 码并将其添加到具有受支持格式的文档中。提供必须签名的文档的路径，并设置所需的 QR 码文本和视觉选项。您可以将生成的二维码图像放置在任何文档页面的任何区域。
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // 指定要签署的文件
            using (Signature signature = new Signature("source.docx"))
            {
                // 创建 QR 码标志选项
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // 设置 QR 码选项
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150,
                };

                // 签名并保存处理后的文件
                SignResult result = signature.Sign("result.docx", options);
            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // 指定要签署的文件
            Signature signature = new Signature("source.docx");

            // 创建 QR 码标志选项
            QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith");

            // 设置 QR 码选项
            options.setEncodeType(QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // 签名并保存处理后的文件
            signature.sign("result.docx", options);
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            const signatureLib = require('@groupdocs/groupdocs.signature')

            // 指定要签署的文件
            const signature = new signatureLib.Signature('source.docx');

            // 创建 QR 码标志选项
            const options = new signatureLib.QrCodeSignOptions('JohnSmith');

            // 设置 QR 码选项
            options.setEncodeType(signatureLib.QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // 签名并保存处理后的文件
            signature.sign('result.docx', options);
            ```
        - language: "Python"
          color: "yellow"
          content: |
            ```python {style=abap}  
            import groupdocs.signature as sg

            def run():

                # 指定要签署的文件
                with sg.Signature('source.docx') as signature:

                    # 创建 QR 码标志选项
                    options = sg.QrCodeSignOptions('JohnSmith')

                    # 设置 QR 码选项
                    options.setEncodeType(sg.QrCodeTypes.QR)
                    options.setLeft(50)
                    options.setTop(100)

                    # 签名并保存处理后的文件
                    signature.sign('result.docx', options)
            ```

############################# Supported Formats ###############################
formats:
  enable: true
  title: "支持 60 多种文件格式"
  description: "GroupDocs.Signature 支持几乎所有流行的文件格式"

############################# Metrics ###############################
metrics:
  enable: true
  title: "我们的图书馆统计数据"
  description: "检查关键产品指标，揭示对我们的成就、影响和增长的见解"

  items:
    # items loop
    - number: "50+"
      title: "支持的格式"
      content: "签署 60 多种最流行的商业文件格式。"

    # items loop
    - number: "500k"
      title: "NuGet 下载"
      content: ".NET 的 GroupDocs.Signature 是一个流行的库，在 NuGet 上的下载量超过 550,000 次。"

    # items loop
    - number: "15k"
      title: "Maven 下载"
      content: "Java 开发人员已在 Maven 上下载 GroupDocs.Signature 超过 15K 次。"

    # items loop
    - number: "140+"
      title: "快乐的顾客"
      content: "全球的个人开发者和顶级公司使用我们的产品来构建创新的解决方案。"


############################# Customers ###############################
customers:
  enable: true
  title: "我们满意的客户"
  description: "GroupDocs 库被世界各地的全球知名和杰出品牌所采用"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "准备好开始了吗？"
  description: "在您的平台上免费试用 GroupDocs.Signature 功能"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/signature/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/signature/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/signature/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "经常问的问题"
  description: "探索我们的常见问题"

  items:
    # items loop
    - question: "GroupDocs.Signature 是否需要任何外部库来进行文档签名？"
      answer: "不，GroupDocs.Signature 独立工作。没有 Adob​​e Acrobat、Microsoft Office 等第三方依赖项。"

    # items loop
    - question: "购买前是否可以测试 GroupDocs.Signature 功能？"
      answer: "绝对地！ GroupDocs.Signature 提供免费试用。安装它并探索它的功能。请注意，试用版会向您的文档添加“试用徽章”，并且仅处理前 3 页。要获得完整体验，请获取免费的 30 天临时许可证来访问所有功能。请参阅[临时许可证](https://purchase.groupdocs.com/temporary-license/) 下的详细信息。"

    # items loop
    - question: "提供哪些许可证类型？"
      answer: "正在寻找 GroupDocs.Signature 许可证？我们提供根据您的需求量身定制的各种选项。根据团队规模、部署位置（单个办公室或远程工作场所）以及最终客户分发是否需要与客户共享 SDK/API 进行选择。或者，您也可以选择按月计费的使用许可证，只需按使用量付费。在 [价钱](https://purchase.groupdocs.com/pricing/signature/net/) 下找到最适合您的价格。"

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Signature 低代码 API"
  description: "通过我们基于云的 REST API 使用您的应用程序签署文件。"
  
  items:
    # items loop
    - title: "GroupDocs.Signature Cloud for cURL"
      content: "使用 cURL RESTful API 在 PDF、Word、Excel、PowerPoint、JPEG 和许多其他文件格式上添加签名。"
      icon: "groupdocs_signature-for-curl"
      link: "https://products.groupdocs.cloud/signature/curl"

    # items loop
    - title: "GroupDocs.Signature Cloud for .NET"
      content: "通过 Cloud SDK 签署文档来丰富您的 .NET 应用程序。以您自己的方式保护业务文档。"
      icon: "groupdocs_signature-for-net"
      link: "https://products.groupdocs.cloud/signature/net"

    # items loop
    - title: "GroupDocs.Signature Cloud for Java"
      content: "GroupDocs.Signature SDK 授予您的 Java 应用程序签署任何文件的各种可能性。"
      icon: "groupdocs_signature-for-java"
      link: "https://products.groupdocs.cloud/signature/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Signature 网络应用"
  description: "GroupDocs.Signature 提供了一个免费的网络应用程序，您可以在其中签署文档。可以通过您喜爱的浏览器免费对 60 多种流行的文件格式进行签名。"

  items:
    # items loop
    - title: "GroupDocs.Signature Total"
      content: "可通过任何设备在文档上签名的在线工具。"
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/signature/total"

    # items loop
    - title: "GroupDocs.Signature DOCX"
      content: "在线签署 MS Word DOCX。"
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/signature/docx"

    # items loop
    - title: "GroupDocs.Signature PDF"
      content: "在线保护 PDF 文档。"
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/signature/pdf"


      


---