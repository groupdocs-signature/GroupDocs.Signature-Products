



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:48
draft: false
lang: zh
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "通过 JavaScript 生成并添加印章到 PPTX"
head_description: "利用 GroupDocs.Signature 和 JavaScript 的强大功能，在您的 PPTX 文档的任何页面上生成并放置自定义印章。"

############################# Header ############################
title: "将自定义印章插入 PPTX 文件" 
description: "利用 GroupDocs.Signature for Node.js via Java 生成定制印章，并将其插入到文档中的任何位置。我们的平台提供广泛的选项，以根据您的特定业务需求个性化印章。"
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
    title: "GroupDocs.Signature for Node.js via Java 是什么？"
    link: "/signature/nodejs-java/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) 提供了一种强大且多功能的文档签名解决方案。它使用户能够在超过 60 种不同格式中添加印章和其他签名类型，如 PDF、Word、Excel、图像文件和 ZIP 文件。该平台允许您插入文本、图像、条形码、二维码、元数据、数字证书和印章签名。除签名外，您还可以搜索、验证、修改或删除文档中存在的任何签名。

############################# Steps ############################
steps:
    enable: true
    title: "使用 JavaScript 在 PPTX 中嵌入印章的指南"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) 提供了一个强大的工具，用于创建和嵌入印章，这可以显著增强 Node.js via Java 应用程序的功能。使用此功能可以为您的文档页面定制并应用印章。
      
      1. 输入需要贴印章的 PPTX 文档。
      2. 部署 StampSignOptions 以定义所有必要参数。
      3. 根据需要插入多个印章行。
      4. 应用印章并保存最终文档。
   
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

        // 将文档路径与 Signature 实例关联
        const signature = new signatureLib.Signature('input.pptx');

        // 创建包含所需签名内容的 StampSignOptions
        const options = new signatureLib.StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // 添加一个或多个印章行
        const outerLine = new signatureLib.StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(signatureLib.Color.WHITE);
        outerLine.setBackgroundColor(signatureLib.Color.BLUE);
        options.getOuterLines().add(outerLine);

        // 保存应用印章的文档
        const result = signature.sign('output.pptx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "通过签名增强文档安全"
  description: "使用 GroupDocs.Signature for Node.js via Java，您可以在所有流行文档格式中添加、编辑、验证或删除印章和其他签名类型。该 API 简化了管理签名的过程，以增强文档的完整性和定制化。"
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "GroupDocs.Signature 的功能"
  features:
    # feature loop
    - title: "自定义文档签名"
      content: "在文档的任何部分应用文本、图像、条形码、二维码和印章等签名。此工具还允许加入隐藏的元数据和数字证书，以进一步保护您的内容不被未经授权的修改。"

    # feature loop
    - title: "签名搜索和验证"
      content: "文档签名后，使用我们的验证系统确保签名的完整性。此外，我们的平台使您能够搜索并检索所有应用于文档的签名的详细信息。"

    # feature loop
    - title: "根据需要修改签名"
      content: "对先前应用的签名进行调整和更新。无论是更改内容、颜色、大小还是签名的位置，GroupDocs.Signature for Node.js via Java 都提供全面的定制选项。"

    # feature loop
    - title: "删除不需要的签名"
      content: "轻松删除文档中任何不必要的签名。我们的 API 支持删除各种签名类型，包括印章和数字证书，使您能够完全灵活地管理文档。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "将自定义印章集成到文档中"
      content: |
        了解如何设计和应用包含必要文本的自定义印章到您的文档。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // 提供要贴印章的文档
          const signature = new signatureLib.Signature('input.pptx');

          // 设置具有所需配置的印章选项
          const options = new signatureLib.StampSignOptions();

          // 指定印章在页面上的尺寸和位置
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
          options.setAllPages(true);

          // 包括带有自定义文本的外圆线
          const outerLine1 = new signatureLib.StampLine();
          outerLine1.setText('* The best  choice *');
          outerLine1.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
          const signatureFont1 = new signatureLib.SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName('Arial');
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(signatureLib.Color.WHITE);
          outerLine1.setBackgroundColor(signatureLib.Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // 根据需要添加内方形线
          const innerLine1 = new signatureLib.StampLine();
          innerLine1.setText('Company #1');
          innerLine1.setTextColor(signatureLib.Color.RED);
          const signFont1 = new signatureLib.SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);
          
          // 保存带印章的文档
          const result = signature.sign('output.pptx', options);
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
            link: "/examples/signature/formats/signature_stamp.pptx"
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
    title: "探索关键功能"
    exclude: "stamp"
    description: "我们的解决方案提供多种工具，用于创建、管理和删除不同类型的签名，使用户可以完全控制其文档工作流程。"
    items: 
          
        # operation loop 1
        - name: "电子签名"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pptx/"
          description: "向支持的文件格式添加各种类型的签名"

        # operation loop 2
        - name: "向文档添加文本"
          operation: "text"
          link: "/signature/nodejs-java/text/pptx/"
          description: "通过可自定义的文本签名增强文档内容"

        # operation loop 3
        - name: "图像签名"
          operation: "image"
          link: "/signature/nodejs-java/image/pptx/"
          description: "在文档内的任意位置放置任何图像"

        # operation loop 4
        - name: "生成条形码"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pptx/"
          description: "创建并插入各种条形码到支持的文档中"

        # operation loop 5
        - name: "生成二维码"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "生成用于文档签名的二维码"
          
        # operation loop 6
        - name: "数字证书"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "安全地进行商业操作并使用数字证书签署文档"

        # operation loop 7
        - name: "盖章签名"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pptx/"
          description: "使用盖章构造器创建自定义圆形或方形印章"
          
        # operation loop 8
        - name: "搜索签名"
          operation: "search"
          link: "/signature/nodejs-java/search/pptx/"
          description: "在文档中定位任何之前添加的签名"
          
        # operation loop 9
        - name: "签名验证"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pptx/"
          description: "验证签名在应用后是否真实有效"
          
        # operation loop 10
        - name: "修改签名"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pptx/"
          description: "轻松编辑文档中的多种签名"
          
        # operation loop 11
        - name: "删除签名"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pptx/"
          description: "移除多种之前应用的签名"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "在多种文件类型中应用印章签名"
    exclude: "PPTX"
    description: "GroupDocs.Signature API 支持在 60 多种文件格式中使用印章签名，使用户可以在任何页面或区域放置自定义印章，从而提高文档的可访问性和安全性。"
    items: 
          
        # format loop 1
        - name: "盖章 PDF"
          format: "PDF"
          link: "/signature/nodejs-java/stamp/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "盖章 DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "盖章 JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/stamp/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "盖章 PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/stamp/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "盖章 XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---