



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:18
draft: false
lang: zh
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "使用JavaScript应用程序更新PPTX文档签名"
head_description: "利用JavaScript API修订和管理PPTX格式中的数字签名，包括PDF、Word、Excel、PowerPoint和图像文件。"

############################# Header ############################
title: "轻松调整PPTX中的签名" 
description: "通过GroupDocs.Signature for Node.js via Java，您可以修改嵌入在业务文档中的各种电子签名，包括PDF、Word文件、Excel表格、演示文稿和图像格式。"
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费获取"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Java概览"
    link: "/signature/nodejs-java/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/)不仅支持添加签名，还允许您根据需要调整它们。无论您是处理PDF、Word文档、Excel电子表格还是演示文稿，GroupDocs.Signature for Node.js via Java提供无缝的签名管理控制，使未来的修改变得简单易懂。

############################# Steps ############################
steps:
    enable: true
    title: "使用JavaScript修改PPTX中的文本签名指南"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/)使Node.js via Java开发人员能够更新先前嵌入在PPTX文件中的文本签名内容。增强Node.js via Java应用程序的强大编辑功能。
      
      1. 将PPTX文档导入到Signature实例中。
      2. 检索文档中所有签名的列表。
      3. 更新所需签名的内容。
      4. 检查修改结果。
   
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

        // 初始化一个Signature对象并指定文档路径
        const signature = new signatureLib.Signature('input.pptx');

        // 执行搜索以定位文档中的文本签名
        const options = new signatureLib.TextSearchOptions();
        const signatures = signature.search(signatureLib.TextSignature.class, options).toArray();

        if (signatures.length > 0) {
            // 编辑第一个识别到的签名的文本
            const textSignature = signatures[0];
            textSignature.setText('New Text');
            const result = signature.update('output.pptx', textSignature);

            // 验证所做的签名更改
            if (result) {
              console.log(`\nSignature was updated successfully`);
            }
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "文档签名管理"
  description: "GroupDocs.Signature for Node.js via Java提供了一套强大的工具，可以跨多种文档格式添加、修改、验证、搜索和删除签名，从而提升您的工作流程和文档安全性。"
  image: "/img/signature/features_modify.webp" # 500x500 px
  image_description: "签名编辑"
  features:
    # feature loop
    - title: "灵活的文档签署"
      content: "在您的文件中的任意位置使用各种选项（文本、图像、条形码和印章）进行文件签名。您还可以调整嵌入的元数据（如图像中的EXIF数据），并使用数字证书保护敏感信息。"

    # feature loop
    - title: "验证和搜索签名"
      content: "通过轻松验证签名确保文档的完整性。使用内置搜索功能查找和管理文件中的所有签名，确保没有遗漏。"

    # feature loop
    - title: "更新现有签名"
      content: "当签名需要调整时，无论是外观、位置还是内容，我们的API都使过程顺畅无忧，让您快速微调任何签名。"

    # feature loop
    - title: "删除多余签名"
      content: "无论您是需要删除过期签名还是清理文档，GroupDocs.Signature for Node.js via Java都提供对签名删除的充分控制，以确保您的文件保持最新和准确。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "编辑条形码签名"
      content: |
        该示例演示如何以编程方式编辑文档中的条形码签名。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // 加载包含条形码签名的文档
          const signature = new signatureLib.Signature('input.pptx');

          // 识别文档中的所有条形码签名
          const options = new signatureLib.BarcodeSearchOptions();
          const signatures = signature.search(signatureLib.BarcodeSignature.class, options).toArray();

          if (signatures.length > 0) {

              // 更改第一个条形码签名的位置并保存文档
              const barcodeSignature = signatures[0];
              barcodeSignature.setLeft(100);
              barcodeSignature.setTop(100);
              const result = signature.update('output.pptx', barcodeSignature);

              // 确认条形码成功修改
              if (result) {
                console.log(`\nBarcode was updated successfully.`);
              }
          }
          ```
        platform: "nodejs-java"
        copy_title: "复制"
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
    title: "探索我们的签名和功能选项"
    exclude: "modify"
    description: "我们提供丰富的签名功能以及多种操作工具"
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
    title: "跨多种文件格式编辑签名"
    exclude: "PPTX"
    description: "使用Node.js via Java API，已签署的文档可以随时重新访问，允许您提取和修改流行业务格式的签名属性，确保完全的灵活性和控制。"
    items: 
          
        # format loop 1
        - name: "修改 PDF 签名"
          format: "PDF"
          link: "/signature/nodejs-java/modify/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "编辑 DOCX 签名"
          format: "DOCX"
          link: "/signature/nodejs-java/modify/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "编辑 PPTX 签名"
          format: "PPTX"
          link: "/signature/nodejs-java/modify/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 4
        - name: "修改 XLSX 签名"
          format: "XLSX"
          link: "/signature/nodejs-java/modify/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---