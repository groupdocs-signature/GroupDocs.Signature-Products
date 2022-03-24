---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java 数字签名 API，将电子签名添加到 PDF Word Excel 图像"
head_description: "Java 数字签名 API。电子签名库，用于对 PDF、Microsoft Word、Excel 电子表格、PowerPoint 演示文稿和图像文档格式进行数字签名."

############################# Header ############################
title: "用于管理数字签名的 Java API"
description: "在用于签署图像和数字文档文件格式的 Java 应用程序中管理图像、二维码、条形码、元数据、文本和图章类型的电子签名。"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "/border/groupdocs-signature-java.svg"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "概述"

            # button loop
            - link: "#features"
              text: "特征"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "价钱"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# 概述 ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature for Java API 可帮助您开发具有电子签名功能的 Java 应用程序，以签署支持格式的数字文档，而无需安装任何外部软件。它支持对各种类型的电子签名进行操作和管理，例如图像、条形码、二维码、印章、文本、光学和元数据。您的所有电子商务文档（如微软办公软件 Word、PowerPoint 演示文稿、Excel 电子表格、图像和 PDF 文件）都可以通过自定义签名属性进行数字签名，例如根据您的要求，阴影、尺寸、对齐等。数字签名库简单轻量，由一个 DLL 文件组成，可以轻松集成到新的或现有的 Java 应用程序中。 

      通过 GroupDocs.Signature for Java API，您可以从系统中加载所有已注册的证书，或者使用简单和高级的搜索来查找现有签名。使用受密码保护的文档的选项，指定常见的签名属性（文本大小、不透明度、旋转、验证、字体属性、颜色选项、页码、宽度、顶部、左侧等）以及实现不同电子签名类型的支持使其成为可靠的数字文档的电子签名管理解决方案。

      GroupDocs.Signature for Java 与所有 Java 版本兼容，并支持能够运行 Java 运行时的流行操作系统（Windows、Linux、MacOS）
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          以下是 Java 的 GroupDocs.Signature 的概述：

        right:
          enable: true
          icon: "fab fa-html5"
          title: "签名类型"
          content: |
            * 文字签名
            * 图像签名
            * 数字签名
            * 二维码签名
            * 条码签名
            * 盖章签名
            * 表单域签名
      
      ## TAB TWO ##
      tab_two:
        description: |
          Java 电子签名 API 支持 [文档文件格式](https://docs.groupdocs.com/signature/java/supported-document-formats/)，如下所示。

        left:
          enable: true
          table:
            # table loop
            - title: "微软办公软件"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM

        right:
          enable: true
          table:
            # table loop
            - title: "Images & 其他格式"
              content: |
                * **图像**：JPG、BMP、PNG、TIFF、GIF、DCM、WEBP
                * **OpenDocument**：ODT、OTT、OTS、ODS、ODP、OTP、ODG
                * **Jpeg2000**：JP2、JPF、JPX、J2K、J2C、JPM
                * **元文件**：EMF、WMF、CMX
                * **便携式**：PDF
                * **可缩放矢量图形**：CDR、SVG
                * **Adobe Photoshop**：PSD
                * **其他**：DJV

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature for Java 支持以下操作系统、框架和包管理器:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "操作系统"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "支持的框架"
              content: |
                * Java 7 (1.7) 及更高版本

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "开发环境"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "构建自动化工具"
              content: |
                * Maven

############################# 特征 ############################
features:
    enable: true
    title: "GroupDocs.Signature for Java 特征"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "从支持的文档格式创建、读取、修改、隐藏和删除电子签名"

      # feature loop
      - icon: "fas fa-eye"
        content: "从流、相对路径或绝对路径访问要签名的文档"

      # feature loop
      - icon: "fas fa-bolt"
        content: "将签名签名应用于文档、电子表格、演示文稿、图像和 PDF 文件"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "添加文字签名作为注释、贴纸、图像到 PDF 文件还配置样式和颜色"

      # feature loop
      - icon: "fas fa-code"
        content: "签署 PDF 文档、图像文件并以不同的文件格式获取输出"

      # feature loop
      - icon: "fas fa-cloud"
        content: "使用文字签名作为水印对图像进行数字签名并添加透明度、旋转到电子签名"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "搜索证书并使用数字证书签署 Microsoft Word、Excel 和 PDF 文档"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "使用本机文本水印为文字处理文档格式签名"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "使用 QR 码、条形码签署 Word、幻灯片、单元格、PDF 和图像文件"

      # feature loop
      - icon: "fas fa-border-all"
        content: "配置和应用盖章签名以保护支持的文件格式"

      # feature loop
      - icon: "fas fa-wrench"
        content: "设置和分配图像签名到文档、电子表格、演示文稿、图像和 PDF 文件"

      # feature loop
      - icon: "fas fa-columns"
        content: "配置签名属性，例如外观、边距、对齐等."

      # feature loop
      - icon: "fas fa-file-word"
        content: "将数字签名应用于受密码保护的文档"

      # feature loop
      - icon: "fas fa-envelope"
        content: "使用签名处理程序执行 PDF 文档的文本验证"

      # feature loop
      - icon: "fas fa-print"
        content: "使用 .CER 和 .PFX 证书容器对 Word、Excel、PDF 文档进行数字验证"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "为 PDF 文字签名指定不同的度量单位类型（例如毫米、像素等）"

      # feature loop
      - icon: "fas fa-lock"
        content: "通过文件或 URL 获取文档信息 - 将表单字段签名添加到 PDF 文档"

      # feature loop
      - icon: "fas fa-file-code"
        content: "将自定义数据对象、嵌入式 VCard、电子邮件、EPC、MeCard 或事件对象添加到 QR 码"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "将不同的画笔样式应用于签名，例如渐变、径向、实体和纹理画笔"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "签署位于 FTP 或 Azure 云存储的文档"

      # feature loop
      - icon: "fas fa-heading"
        content: "为文档、幻灯片、图像和 PDF 文件设置形状内的文本对齐方式"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "搜索、验证和数字签名 PowerPoint 演示文档"

      # feature loop
      - icon: "fas fa-cube"
        content: "使用单元格文档中的像素放置签名和用于盖章签名的文本定位"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "用圆角实现矩形盖章签名"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "用图像数据内容扩展条形码和二维码签名"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "在使用签名和搜索选项时添加加密元数据签名"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "将自定义对象嵌入 Word、Excel 和演示文稿中的元数据签名"

    more_feature:
      # more_feature_loop
      - title: "轻松配置和应用电子签名"
        content: |
          GroupDocs.Signature for Java API 可以配置和添加电子签名到支持的文档格式。以下是一个代码示例，展示了将文本签名应用于 PDF 文件是多么简单：
          
          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // 设置签名位置
          options.setLeft(100);
          options.setTop(100);
          
          // 设置签名矩形
          options.setWidth(100);
          options.setHeight(30);

          // 设置文本颜色和字体
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // 签署文件归档
          signature.sign("sample_signed.pdf", options);
          ```
      # more_feature_loop
      - title: "电子签名支持的条形码编码类型"
        content: |
          使用 GroupDocs.Signature for Java API，您可以将条形码和 QR 码签名应用于支持的文件格式。 GroupDocs.Signature for Java 支持大量条形码编码类型以满足大多数需求。支持的条码编码类型包括 Code 11、Code 128、Code 16K/32、Databar 码、GS1 Codeblock、ISBN、ISMN、ISSN、ITF16、Pdf147、EAN8、EAN13、EAN14、UPCA、UPCE、ITF14、Code39 Standard 和Code39 扩展。

          同样，Java API 的 GroupDocs.Signature 允许您使用 QR 码类型，例如 QR、Aztec 和 Data Matrix。支持的 QR 码编码类型包括 Aztec、DataMatrix、GS1 DataMatrix 和 GS1 QR。

      # more_feature_loop
      - title: "搜索签名和证书"
        content: |
          通过 GroupDocs.Signature for Java API，您可以在任何文档、演示文稿、电子表格、图像以及 PDF 文件中搜索二维码和条形码签名，并获取搜索结果。您还可以从二维签名码签名的文档中搜索自定义数据对象，以及从二维签名签名的文档中搜索标准 VCard 和电子邮件对象。还支持验证二维码签名的加密文本以及在 PDF 文档中搜索元数据签名。对 Words & Cells 文档的数字签名应用额外的搜索条件。 

          搜索选项也可用于 word 文档、幻灯片和电子表格的元数据签名，而表单域搜索可用于 PDF 文档。

      # more_feature_loop
      - title: "配置电子签名属性"
        content: |
          为了增强最终用户的 UX，GroupDocs.Signature for Java API 提供了许多可以很容易配置的属性。您可以设置字体和颜色选项（背景颜色、前景色、粗体、斜体、下划线、字体系列、字体大小等）、背景和边框选项（背景颜色、背景透明度、边框颜色、边框虚线样式、边框粗细、边框透明度等），签名边距（左侧，顶部，宽度，高度，填充等），以及设置图像签名区域和签名对齐（水平对齐，垂直对齐等）。

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature 为其他流行的开发环境提供文档查看 API"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for .NET"
          image: "/border/groupdocs-signature-net.svg"
          product: "GroupDocs.Signature"
          platform: ".NET"
          link: "/signature/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---