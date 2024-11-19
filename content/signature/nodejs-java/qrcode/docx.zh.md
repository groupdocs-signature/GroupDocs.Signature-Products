



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:22
draft: false
lang: zh
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "在DOCX文档中使用JavaScript生成二维码"
head_description: "利用GroupDocs.Signature API在DOCX文件中创建和集成 2D 条形码。轻松地将二维码放置在任何文档页面上。"

############################# Header ############################
title: "为DOCX生成二维码" 
description: "使用GroupDocs.Signature for Node.js via Java创建并嵌入带有可定制内容（如文本和数字数据）的 2D 条形码，适用于PDF、Word、Excel、图像等多种文档类型。"
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费试用"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "探索GroupDocs.Signature for Node.js via Java的功能"
    link: "/signature/nodejs-java/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/)提供先进的文档增强工具，使您能够在流行的文件格式中生成和嵌入多种签名类型，包括二维码。签署并保护PDF、Word文档、Excel 表格、PowerPoint 演示文稿和图像，使用文本、图像、条形码、二维码、元数据、数字和印章签名。

############################# Steps ############################
steps:
    enable: true
    title: "在DOCX中生成和嵌入二维码的指南"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/)使得在各种广泛使用的格式中创建二维码并将其集成到DOCX页面成为可能。我们的解决方案支持超过10种不同的二维码类型，可以无缝地集成到Node.js via Java应用程序中，增强其二维码签署能力。
      
      1. 提供用于二维码签名的DOCX文件或流。
      2. 将所需文本输入到QrCodeSignOptions实例中。
      3. 调整颜色、位置、大小等视觉设置。
      4. 保存包含二维码的文档。
   
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

        // 创建一个Signature实例并传入文档路径
        const signature = new signatureLib.Signature('input.docx');

        // 利用QrCodeSignOptions将二维码插入文档中
        // Create QR code sign options
        const options = new signatureLib.QrCodeSignOptions('Text Content');

        // 定义签名类型及其在页面上的位置
        options.setEncodeType(signatureLib.QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);
  
        // 保存包含新添加二维码的文档
        signature.sign('output.docx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "全面的签名和二维码集成"
  description: "使用GroupDocs.Signature for Node.js via Java API，您可以管理各种签名。轻松生成、定制、验证、搜索和移除不同文档类型中的签名，为您的工作流程提供无与伦比的灵活性。"
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "签名和二维码功能"
  features:
    # feature loop
    - title: "多格式文档签署"
      content: "向任何支持的文档格式添加多种类型的签名，包括文本、图像、条形码、二维码和印章签名。可将它们放置在任何页面上，并管理文档元数据。通过数字证书确保文档安全，防止未授权的更改。"

    # feature loop
    - title: "高效的签名验证"
      content: "验证文档中的所有签名，以确保其符合所需标准。通过内置搜索功能轻松检索和审核签名。"

    # feature loop
    - title: "灵活的签名编辑"
      content: "更新或修改现有签名，调整内容、位置、大小和颜色，以满足文档在初始签署后的需求。"

    # feature loop
    - title: "轻松删除签名"
      content: "轻松移除任何不需要或过时的签名，包括数字证书。对签名管理的完全控制确保文档干净、有序。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "自定义生成的二维码"
      content: |
        此示例详细说明了如何在DOCX页面上添加自定义二维码的过程。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // 获取要签名的文档并传递给Signature
          const signature = new signatureLib.Signature('input.docx');

          // 使用所需文本设置二维码选项
          const signOptions = new signatureLib.QrCodeSignOptions('Archived on July 11, 2019');

          // 确定二维码在页面上的位置
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // 指定签名的内边距
          const padding = new signatureLib.Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // 选择二维码颜色
          signOptions.setForeColor(signatureLib.Color.RED);

          // 定义配套消息的字体选项
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // 自定义二维码的背景颜色和画笔
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new signatureLib.LinearGradientBrush(signatureLib.Color.GREEN, signatureLib.Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // 将二维码嵌入文档中
          signature.sign('output.docx', signOptions);
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
            link: "/examples/signature/formats/signature_qrcode.docx"
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
    title: "了解我们的主要功能"
    exclude: "qrcode"
    description: "我们提供广泛的签名格式和操作，以满足您的需求"
    items: 
          
        # operation loop 1
        - name: "电子签名"
          operation: "esign"
          link: "/signature/nodejs-java/esign/docx/"
          description: "向支持的文件格式添加各种类型的签名"

        # operation loop 2
        - name: "向文档添加文本"
          operation: "text"
          link: "/signature/nodejs-java/text/docx/"
          description: "通过可自定义的文本签名增强文档内容"

        # operation loop 3
        - name: "图像签名"
          operation: "image"
          link: "/signature/nodejs-java/image/docx/"
          description: "在文档内的任意位置放置任何图像"

        # operation loop 4
        - name: "生成条形码"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "创建并插入各种条形码到支持的文档中"

        # operation loop 5
        - name: "生成二维码"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "生成用于文档签名的二维码"
          
        # operation loop 6
        - name: "数字证书"
          operation: "digital"
          link: "/signature/nodejs-java/digital/docx/"
          description: "安全地进行商业操作并使用数字证书签署文档"

        # operation loop 7
        - name: "盖章签名"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "使用盖章构造器创建自定义圆形或方形印章"
          
        # operation loop 8
        - name: "搜索签名"
          operation: "search"
          link: "/signature/nodejs-java/search/docx/"
          description: "在文档中定位任何之前添加的签名"
          
        # operation loop 9
        - name: "签名验证"
          operation: "verify"
          link: "/signature/nodejs-java/verify/docx/"
          description: "验证签名在应用后是否真实有效"
          
        # operation loop 10
        - name: "修改签名"
          operation: "modify"
          link: "/signature/nodejs-java/modify/docx/"
          description: "轻松编辑文档中的多种签名"
          
        # operation loop 11
        - name: "删除签名"
          operation: "delete"
          link: "/signature/nodejs-java/delete/docx/"
          description: "移除多种之前应用的签名"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "将二维码与多种文件格式集成"
    exclude: "DOCX"
    description: "利用Node.js via Java API生成二维码并将其嵌入多种广泛使用的文件格式中。在这些条形码中封装重要数据，以实现无缝集成和未来检索。"
    items: 
          
        # format loop 1
        - name: "PDF 的二维码"
          format: "PDF"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "DOCX 的二维码"
          format: "DOCX"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "JPEG 的二维码"
          format: "JPEG"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "PPTX 的二维码"
          format: "PPTX"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "XLSX 的二维码"
          format: "XLSX"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---