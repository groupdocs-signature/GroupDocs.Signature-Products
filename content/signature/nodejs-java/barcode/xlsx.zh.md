



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:26
draft: false
lang: zh
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "使用 JavaScript 应用程序为 XLSX 生成条形码"
head_description: "仅需几行代码即可快速生成并嵌入条形码签名到 XLSX 文档中。GroupDocs.Signature 支持多种文件格式的签名。"

############################# Header ############################
title: "轻松生成并添加条形码到 XLSX" 
description: "使用 GroupDocs.Signature for Node.js via Java 将条形码整合到您的业务文档中，准确定位到所需位置。我们的解决方案提供广泛的自定义选项，以满足您的条形码签名需求。"
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "立即下载 - 完全免费！"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "关于 GroupDocs.Signature for Node.js via Java 的介绍"
    link: "/signature/nodejs-java/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) 是一款强大的文档签名工具，支持各种类型的签名，包括文本、图像、条形码、数字证书和印章。它兼容超过 60 种文件格式，如 PDF、MS Office 文件、图像和 ZIP 压缩包，能够进行全面的文档管理。文档中的签名可以根据需要进行搜索、验证、修改或删除。

############################# Steps ############################
steps:
    enable: true
    title: "如何在 XLSX 文件中生成并嵌入条形码"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) 可以在 XLSX 页面上生成并放置条形码，支持超过 60 种条形码类型，Node.js via Java 应用程序可以通过集成我们的库轻松增强条形码签名功能。
      
      1. 提供需处理的 XLSX 文件或流。
      2. 将条形码文本传递给 BarcodeSignOptions 实例。
      3. 调整条形码设置，如位置、大小等。
      4. 保存带有新添加条形码的文档。
   
    code:
      platform: "nodejs-java"
      copy_title: "复制"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "示例签名"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "点击以复制"
        copy_done: "已复制"
      links:
        #  loop
        - title: "更多示例"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "文档"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // 使用文档路径实例化 Signature 对象
        const signature = new signatureLib.Signature('input.xlsx');

        // 使用 BarcodeSignOptions 将条形码集成到文档中
        const options = new signatureLib.BarcodeSignOptions('Business data');

        // 配置条形码类型及其他参数
        options.setEncodeType(signatureLib.BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);
  
        // 保存已签名的文档
        signature.sign('output.xlsx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "使用高级签名选项增强和保护您的文档"
  description: "GroupDocs.Signature for Node.js via Java 库旨在简化流行文档格式的签名和后续管理。快速并高效地添加、修改、验证或移除各种签名。"
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "GroupDocs.Signature 的关键功能"
  features:
    # feature loop
    - title: "动态文档签名"
      content: "使用各种签名类型（包括文本、图像、条形码、二维码和印章）对文档的任意页面进行签名。此外，您可以嵌入隐藏的元数据（例如图像中的 EXIF 数据），或使用数字证书保护文档以防止未授权的编辑。"

    # feature loop
    - title: "强大的签名验证和搜索"
      content: "我们的解决方案提供全面的工具用于管理签名文档。验证签名的真实性以确保文档的完整性，利用搜索功能列出嵌入在文档中的所有签名。"

    # feature loop
    - title: "轻松编辑签名"
      content: "大多数先前添加的签名可以轻松修改。更新文本、重新定位或更改签名的外观以满足您的需求。"

    # feature loop
    - title: "简化签名移除"
      content: "凭借对 CRUD 操作的全面支持，我们的工具能够高效移除文档中的签名，确保仅保留最相关的签名。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "如何应用条形码签名"
      content: |
        此示例演示如何在 XLSX 文档页面嵌入自定义条形码。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // 提供待签名的文档
          const signature = new signatureLib.Signature('input.xlsx');

          // 使用 BarcodeSignOptions 将条形码集成到文档中
          const signOptions = new signatureLib.BarcodeSignOptions('Accepted');
          signOptions.setEncodeType(signatureLib.BarcodeTypes.Code39FullASCII);

          // 配置条形码类型及其他参数
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Left);

          // 定义条形码与页面边缘的间距
          const padding = new signatureLib.Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // 选择条形码颜色
          signOptions.setForeColor(signatureLib.Color.RED);

          // 指定消息的字体样式
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName('Arial');
          signOptions.setFont(font);

          // 指示消息的位置
          signOptions.setCodeTextAlignment(signatureLib.CodeTextAlignment.Above);

          // 签名并保存文档
          signature.sign('output.xlsx', signOptions);

          ```
        platform: "nodejs-java"
        copy_title: "复制"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
          copy_tip: "点击以复制"
          copy_done: "已复制"
        top_links:
          #  loop
          - title: "下载结果"
            icon: "download"
            link: "/examples/signature/formats/signature_barcode.xlsx"
        links:
          #  loop
          - title: "更多示例"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
          #  loop
          - title: "文档"
            link: "https://docs.groupdocs.com/signature/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "准备开始了吗？"
  description: "免费试用 GroupDocs.Signature 的功能或请求许可证"
  items:
    #  loop
    - title: "NPM 下载"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "许可证"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "深入了解我们的主要功能"
    exclude: "barcode"
    description: "体验我们提供的各种签名类型和工具"
    items: 
          
        # operation loop 1
        - name: "电子签名"
          operation: "esign"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "向支持的文件格式添加各种类型的签名"

        # operation loop 2
        - name: "向文档添加文本"
          operation: "text"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "通过可自定义的文本签名增强文档内容"

        # operation loop 3
        - name: "图像签名"
          operation: "image"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "在文档内的任意位置放置任何图像"

        # operation loop 4
        - name: "生成条形码"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "创建并插入各种条形码到支持的文档中"

        # operation loop 5
        - name: "生成二维码"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "生成用于文档签名的二维码"
          
        # operation loop 6
        - name: "数字证书"
          operation: "digital"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "安全地进行商业操作并使用数字证书签署文档"

        # operation loop 7
        - name: "盖章签名"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "使用盖章构造器创建自定义圆形或方形印章"
          
        # operation loop 8
        - name: "搜索签名"
          operation: "search"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "在文档中定位任何之前添加的签名"
          
        # operation loop 9
        - name: "签名验证"
          operation: "verify"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "验证签名在应用后是否真实有效"
          
        # operation loop 10
        - name: "修改签名"
          operation: "modify"
          link: "/signature/nodejs-java/modify/xlsx/"
          description: "轻松编辑文档中的多种签名"
          
        # operation loop 11
        - name: "删除签名"
          operation: "delete"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "移除多种之前应用的签名"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "支持多种文档格式的签名"
    exclude: "XLSX"
    description: "Node.js via Java API 可让您对超过 60 种不同格式进行签名。无论是在特定页面添加签名，还是进行精准定位，我们的工具均能轻松应用各种签名类型。"
    items: 
          
        # format loop 1
        - name: "向 PDF 添加条形码"
          format: "PDF"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "向 DOCX 添加条形码"
          format: "DOCX"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "向 JPEG 添加条形码"
          format: "JPEG"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "向 PPTX 添加条形码"
          format: "PPTX"
          link: "/signature/nodejs-java/barcode/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "向 XLSX 添加条形码"
          format: "XLSX"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---