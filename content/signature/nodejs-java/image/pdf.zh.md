



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:52
draft: false
lang: zh
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "使用 JavaScript 向 PDF 文件添加图像签名"
head_description: "在 Node.js 中使用几行代码在 PDF 文件上放置图像签名。使用 GroupDocs.Signature for Node.js via Java API 添加图像。"

############################# Header ############################
title: "使用图像签名签署 PDF 文件" 
description: "利用 GroupDocs.Signature for Node.js via Java 的功能将图像无缝嵌入 PDF、Word、Excel 等多种办公文档格式中。添加执行签名图像可以显著提升文档的专业性和可信度，创造出精致而生动的展示效果。"
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费下载"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "介绍 GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) 使用户能够在文档的任何位置嵌入图像签名。此工具使企业能够通过将图像添加到 PDF、Word、Excel、PowerPoint 和流行图像格式中来简化工作流程，提高文档管理效率。

############################# Steps ############################
steps:
    enable: true
    title: "使用 JavaScript 在 PDF 中添加图像的指南"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) 使 Node.js via Java 应用程序能够无缝地将图像签名集成到 PDF 文档中。利用我们的全面库增强您的应用程序功能。
      
      1. 用 PDF 文档实例化 Signature
      2. 使用 ImageSignOptions 指定签名图像
      3. 在任意页面上准确放置图像
      4. 将签名文档保存到所需位置
   
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

        // 使用文档的路径初始化 Signature
        const signature = new signatureLib.Signature('input.pdf');

        // 配置 ImageSignOptions 以包括所需的图像签名
        const options = new signatureLib.ImageSignOptions('company_logo.jpg');

        // 在所有页面的左上角放置图像
        options.setAllPages(true);
        options.setLeft(100);
        options.setTop(200);
        
        // 保存带有应用图像签名的文档
        const result = signature.sign('output.pdf', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "高级文档签署功能"
  description: "我们的API提供了一套简化电子签署的功能。您可以添加、修改、删除、搜索和验证多种类型的签名，包括图像签名。"
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "图像签名"
  features:
    # feature loop
    - title: "将图像嵌入办公文档"
      content: "可以轻松地在文档中的任何地方放置图像签名，无论是 PDF、Word 还是 Excel 文件。通过添加图像、条形码、元数据或数字证书来增强文档的功能性。"

    # feature loop
    - title: "搜索和验证签名"
      content: "通过验证签名确保您的签名文件的真实性。使用搜索功能检索和查看嵌入文档中的所有签名。"

    # feature loop
    - title: "修改现有签名"
      content: "我们的API使用户能够根据需要更新和调整签名。根据文档处理的灵活性，修改任何先前添加的签名的大小、位置或其他属性。"

    # feature loop
    - title: "删除不必要的签名"
      content: "通过删除不再需要的签名来有效管理文档。我们的API支持几乎所有签名类型的完整CRUD操作。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "通过图像签名增强文档"
      content: |
        了解如何将图像纳入商业文档以添加补充信息。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // 选择要签署的文档
          const signature = new signatureLib.Signature('input.pdf');

          // 用图像路径配置图像选项
          const options = new signatureLib.ImageSignOptions('manager_signature.jpg');

          // 调整图像签名的大小
          options.setWidth(100);
          options.setHeight(100);

          // 将图像放置在右下角
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // 如有需要，从页面角落添加填充
          const padding = new signatureLib.Padding();
          padding.setRight(120);
          padding.setBottom(120);
          options.setMargin(padding);

          // 可选地，为图像添加自定义边框
          const border = new signatureLib.Border();
          border.setColor(signatureLib.Color.RED);
          border.setDashStyle(signatureLib.DashStyle.DashDotDot);
          border.setWeight(5);
          border.setVisible(true);
          options.setBorder(border);

          // 旋转图像签名以获得最佳效果
          options.setRotationAngle(45);

          // 将更新后的文档保存到所需位置
          const result = signature.sign('output.pdf', options);
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
            link: "/examples/signature/formats/signature_image.pdf"
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
    title: "发现我们提供的功能"
    exclude: "image"
    description: "我们自豪地展示广泛的签名方法和操作。"
    items: 
          
        # operation loop 1
        - name: "电子签名"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "向支持的文件格式添加各种类型的签名"

        # operation loop 2
        - name: "向文档添加文本"
          operation: "text"
          link: "/signature/nodejs-java/text/pdf/"
          description: "通过可自定义的文本签名增强文档内容"

        # operation loop 3
        - name: "图像签名"
          operation: "image"
          link: "/signature/nodejs-java/image/pdf/"
          description: "在文档内的任意位置放置任何图像"

        # operation loop 4
        - name: "生成条形码"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "创建并插入各种条形码到支持的文档中"

        # operation loop 5
        - name: "生成二维码"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "生成用于文档签名的二维码"
          
        # operation loop 6
        - name: "数字证书"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "安全地进行商业操作并使用数字证书签署文档"

        # operation loop 7
        - name: "盖章签名"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pdf/"
          description: "使用盖章构造器创建自定义圆形或方形印章"
          
        # operation loop 8
        - name: "搜索签名"
          operation: "search"
          link: "/signature/nodejs-java/search/pdf/"
          description: "在文档中定位任何之前添加的签名"
          
        # operation loop 9
        - name: "签名验证"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "验证签名在应用后是否真实有效"
          
        # operation loop 10
        - name: "修改签名"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pdf/"
          description: "轻松编辑文档中的多种签名"
          
        # operation loop 11
        - name: "删除签名"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "移除多种之前应用的签名"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "向各种文件类型添加图像"
    exclude: "PDF"
    description: "Node.js via Java API 允许您将图像嵌入到广泛的文档格式中。自定义大小、位置和页面定位以增强文档签署过程。"
    items: 
          
        # format loop 1
        - name: "使用图像签名 PDF"
          format: "PDF"
          link: "/signature/nodejs-java/image/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "使用图像签名 DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/image/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "使用图像签名 JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "使用图像签名 PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/image/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "使用图像签名 XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---