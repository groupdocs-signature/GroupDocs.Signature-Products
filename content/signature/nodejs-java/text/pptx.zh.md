



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:14
draft: false
lang: zh
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "通过JavaScript向PPTX添加文本签名"
head_description: "利用JavaScript API无缝地将文本签名集成到PPTX文档中。我们的API支持广泛的格式，包括PDF、Word、Excel、演示文稿、图像和ZIP文件。"

############################# Header ############################
title: "向PPTX添加文本签名" 
description: "使用GroupDocs.Signature for Node.js via Java将个性化文本签名纳入您的业务文件中。通过增强安全和可自定义的签名选项，掌控您的文档工作流程。"
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "开始免费试用"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "介绍GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/)是一个创新解决方案，旨在便捷地将文本签名添加到文档中。自定义并在任意页面上放置签名，提高文档处理效率。通过整合个性化的文本标记，简化您组织的工作流程，提升功能性和专业性。

############################# Steps ############################
steps:
    enable: true
    title: "使用JavaScript为PPTX创建文本签名的指南"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/)使您能够在Node.js via Java应用程序中向PPTX文档添加文本签名。快速提升您产品的能力，借助我们的强大解决方案。
      
      1. 将PPTX文档作为参数传递给Signature类。
      2. 使用所需文本实例化TextSignOptions。
      3. 设置文本签名的视觉属性。
      4. 将文本签名添加到文档的所需页面。
   
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

        // 使用文档路径初始化Signature类
        const signature = new signatureLib.Signature('input.pptx');

        // 创建包含所需签名文本的TextSignOptions
        const options = new signatureLib.TextSignOptions('Approved');

        // 配置文本颜色和字体属性
        options.setForeColor(new signatureLib.Color(255, 0, 0));
        const signatureFont = new signatureLib.SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName('Comic Sans MS');
        options.setFont(signatureFont);
        
        // 将文本签名添加到文档中
        const result = signature.sign('output.pptx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "增强的文本签名控制"
  description: "使用GroupDocs.Signature for Node.js via Java，您可以大幅改善主要文档格式中基于文本的签名管理。该工具使您能够配置签名的样式、位置和内容，帮助企业定制其文档流程。"
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "GroupDocs.Signature的核心功能"
  features:
    # feature loop
    - title: "动态文档签名"
      content: "在支持的文档的任何页面插入各种类型的签名——如文本、图片、条形码、二维码或印章。嵌入元数据以携带隐藏信息，或应用数字证书以提高安全性。"

    # feature loop
    - title: "签名搜索与验证"
      content: "验证嵌入在文档中的签名的真实性。执行高效搜索以定位所有签名实例，确保全面的文档跟踪和管理。"

    # feature loop
    - title: "编辑或删除签名"
      content: "根据需要修改或删除先前添加的签名。您可以调整任意签名的外观、位置或内容，以满足演变需求，确保文档处理的灵活性。"

    # feature loop
    - title: "本地签名自定义"
      content: "对于某些文件类型，根据内置文档特性定制签名位置，如在Word文件中添加水印或在PDF中添加自定义印章，增强文档的独特性。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "在文档中实现文本签名"
      content: |
        了解如何将文本签名嵌入到业务文档中以优化流程。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // 选择要签名的文档
          const signature = new signatureLib.Signature('input.pptx');

          // 定义包含指定内容的文本选项
          const options = new signatureLib.TextSignOptions('Rescheduled to 03/04/2025');

          // 设置签名在页面上的大小和位置
          options.setLeft(100);
          options.setTop(180);
          options.setWidth(230);
          options.setHeight(30);

          // 为签名与页面边缘间添加填充
          const padding = new signatureLib.Padding();
          padding.setBottom(20);
          padding.setRight(20);
          options.setMargin(padding);

          // 自定义文本颜色和字体样式
          options.setForeColor(signatureLib.Color.RED);
          const signatureFont = new signatureLib.SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName('Comic Sans MS');
          options.setFont(signatureFont);

          // 如有需要，为文本签名添加边框
          const border = new signatureLib.Border();
          border.setColor(signatureLib.Color.RED);
          border.setDashStyle(signatureLib.DashStyle.Dash);
          border.setTransparency(0.5);
          border.setVisible(true);
          border.setWeight(2);
          options.setBorder(border);

          // 配置签名的背景
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.YELLOW);
          background.setTransparency(0.8);
          options.setBackground(background);

          // 可选择，如果需要，将文本保存为图像以便兼容
          options.setSignatureImplementation(signatureLib.TextSignatureImplementation.Image);
          
          // 保存带有添加的文本签名的文档
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
            link: "/examples/signature/formats/signature_text.pptx"
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
    title: "全面的签名管理功能"
    exclude: "text"
    description: "我们的平台提供完整的CRUD操作和高级功能，管理七种不同类型的签名，使您能够精准和便捷地管理您的文档签名。"
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
    title: "在各种格式中应用文本签名"
    exclude: "PPTX"
    description: "利用Node.js via Java API的功能，将基于文本的签名集成到广泛的Office格式中。在文档生命周期的每个阶段，通过添加高度可自定义的文本标记来控制信息流。"
    items: 
          
        # format loop 1
        - name: "PDF 文本签名"
          format: "PDF"
          link: "/signature/nodejs-java/text/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "DOCX 文本签名"
          format: "DOCX"
          link: "/signature/nodejs-java/text/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "JPEG 文本签名"
          format: "JPEG"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "PPTX 文本签名"
          format: "PPTX"
          link: "/signature/nodejs-java/text/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "XLSX 文本签名"
          format: "XLSX"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---