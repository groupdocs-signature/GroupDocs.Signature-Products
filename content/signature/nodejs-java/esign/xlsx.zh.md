



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:11
draft: false
lang: zh
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "在 JavaScript 中使用电子签名签署 XLSX"
head_description: "利用 JavaScript API 的能力，数字签名和保护 XLSX 文件，包括 PDF、Word 文档、Excel 表格、演示文稿和图像格式。"

############################# Header ############################
title: "电子签署 XLSX 文件" 
description: "使用 GroupDocs.Signature for Node.js via Java 在您的文档中插入多种数字签名，确保 PDF、Word、Excel、演示文稿和图像格式文件的数据完整性和合规性。"
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "立即免费下载"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Java API 概述"
    link: "/signature/nodejs-java/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) 提供了一套强大的工具，用于添加电子签名。通过其直观的 API，您可以无缝签署、搜索、验证、修改和删除各种文件类型中的签名，无需外部软件。它支持对 PDF、Word 文档、Excel 表格、PowerPoint 幻灯片和多种图像格式的顺畅签署。

############################# Steps ############################
steps:
    enable: true
    title: "使用 JavaScript 签署 XLSX 的步骤"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) 简化了将自定义签名添加到 XLSX 文件的过程。Node.js via Java 开发者可以无缝地将签名功能集成到他们的应用程序中。
      
      1. 将 XLSX 文档加载到 Signature 实例中。
      2. 配置 SignOptions 以定义签名属性。
      3. 根据需要调整大小、颜色和内容等属性。
      4. 将已签署的文档保存到指定位置。
   
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

        // 将文档导入 Signature 实例
        const signature = new signatureLib.Signature('input.xlsx');

        // 实例化一个 QrCodeSignOptions 对象
        const options = new signatureLib.QrCodeSignOptions('QR code text');
        
        // 指定所有必需的选项
        options.setLeft(100);
        options.setTop(100);
        options.setForeColor(new Color(255, 0, 0));

        // 将签署后的文档保存到本地磁盘
        signature.sign('output.xlsx', options);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "高级数字签名功能"
  description: "我们的高级 API 通过简化各种文档的电子签名自动化、验证、修改和管理，加速商业运营。"
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "数字签名功能"
  features:
    # feature loop
    - title: "办公文件的数字签名"
      content: "轻松地将数字签名添加到文档中的任何页面或位置。使用数字证书、元数据、条形码或视觉元素等选项自定义签名，以增强安全性和文档完整性。"

    # feature loop
    - title: "全面的签名控制"
      content: "一旦文档被签署，您可以轻松管理其签名。获取所有签名的完整列表，允许您根据需要进行更新或删除。"

    # feature loop
    - title: "增强文档安全性"
      content: "使用数字证书保护文档免受篡改。可以嵌入或提取元数据，以增强可追溯性和审计，确保文档合规性和真实性。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "如何将图像签名应用于文档"
      content: |
        本指南详细说明在文档中的指定页面上加盖图像签名的过程。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
        
          // 提供源文档作为输入参数
          const signature = new signatureLib.Signature('input.xlsx');

          // 在签名配置选项中指定图像文件路径
          const options = new signatureLib.ImageSignOptions('image.jpg');

          // 配置尺寸并指定签名的目标页
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
          options.setHeight(150);
          options.setWidth(200);
          options.setMargin(new signatureLib.Padding(50));
          options.setAllPages(true);

          // 将签名应用实施到文档上
          signature.sign('output.xlsx', options);

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
            link: "/examples/signature/formats/signature_esign.xlsx"
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
    title: "查看我们的广泛能力"
    exclude: "esign"
    description: "我们提供多种签名类型和丰富的操作功能"
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
    title: "数字签署多种文件类型"
    exclude: "XLSX"
    description: "Node.js via Java API 允许您对超过 60 种文件格式应用数字签名，为您提供了在保护关键商业文件时的广泛灵活性。"
    items: 
          
        # format loop 1
        - name: "电子签名 PDF"
          format: "PDF"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "电子签名 DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/esign/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "电子签名 JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "JPEG 图像"
          
        # format loop 4
        - name: "电子签名 PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/esign/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 5
        - name: "电子签名 XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---