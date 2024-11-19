



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:42
draft: false
lang: zh
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "通过 JavaScript 删除 PDF 中的签名"
head_description: "使用 GroupDocs.Signature for Node.js via Java 可以轻松地从签名的 PDF 文档中删除数字签名、条形码签名、文本签名、图像签名和元数据签名。"

############################# Header ############################
title: "轻松移除 PDF 中的签名" 
description: "我们的综合解决方案超越了简单的文档签署，GroupDocs.Signature for Node.js via Java 提供强大的功能，以定位并删除各种类型的签名。"
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "获取您的免费下载"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "了解 GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) 是一个先进的企业级数字签名库，旨在支持多种类型的签名，包括文本、图像、条形码、数字证书和印章。该工具兼容超过60种文档格式—例如 PDF、MS Office 文件、图像、ZIP 归档及其他关键商业格式—在电子文档工作流程中提供无与伦比的灵活性。该平台不仅能无缝嵌入签名，还提供强大的搜索、验证、更新和删除签名的功能，确保在企业环境中全面管理数字签署流程。

############################# Steps ############################
steps:
    enable: true
    title: "使用 JavaScript 从 PDF 中移除数字签名的指南"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) 使 Node.js via Java 开发人员能够通过一系列简单步骤高效地移除 PDF 文件中的电子签名。
      
      1. 将 PDF 文件路径提供给 Signature 类的实例。
      2. 使用 Search 方法识别文档中的所有签名。
      3. 删除一个或多个已识别的签名。
      4. 检查文档处理的结果。
   
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

        // 将带有签名的文档传递给 Signature 实例
        const signature = new signatureLib.Signature('input.pdf');

        // 删除所有条形码签名
        const options = new signatureLib.DigitalSearchOptions();
        const signatures = signature.search(signatureLib.DigitalSignature.class, options);

        // 删除第一个检测到的数字签名
        if(signatures.size() > 0)
        {
            const digitalSignature = signatures[0];
            const result = signature.delete('output.pdf', digitalSignature);

            // 处理删除结果
            if(result)
            {
                console.log(`\n PDF digital signature deleted successfully`);
            }
        }

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "通过签名工具增强文档安全性"
  description: "GroupDocs.Signature for Node.js via Java 专为简化商业文件格式的签署和管理而精心打造，允许您精准地添加、编辑、验证或删除签名。"
  image: "/img/signature/features_delete.webp" # 500x500 px
  image_description: "探索 GroupDocs.Signature 的全面功能"
  features:
    # feature loop
    - title: "文档签署"
      content: "在任何支持的文档页面上添加文本、图像、条形码、二维码或印章签名。利用图像中的隐藏元数据，如 EXIF，或使用数字证书保护文档完整性，以避免未授权的修改。"

    # feature loop
    - title: "签名搜索和验证"
      content: "我们的工具支持对文档签名的全面验证，确保其真实性。执行全面搜索以检索文档中的所有签名，增强文档控制。"

    # feature loop
    - title: "编辑现有签名"
      content: "根据特定要求，通过调整文本、改变位置或更改颜色，灵活地修改先前添加的签名。"

    # feature loop
    - title: "删除不需要的签名"
      content: "凭借全面的 CRUD 能力，我们的解决方案能够高效地删除文档中的各种签名，确保灵活性和控制。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "删除所有条形码签名"
      content: |
        了解如何消除文档中嵌入的所有条形码签名。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // 提供一个包含条形码签名的文档
          const signature = new signatureLib.Signature('input.pdf');

          // 删除所有条形码签名
          const result = await signature.delete('output.pdf', signatureLib.SignatureType.Barcode);
          if (result.getSucceeded().size() > 0) {

              // 查看删除结果
              console.log('Following PDF barcode signatures were deleted:');
              let number = 1;
              result.getSucceeded().toArray().forEach((o) => {
                    const temp = o;
                    console.log(`Signature #${number++}: Type: ${temp.getSignatureType()}, 
                    Id: ${temp.getSignatureId()}, Text: ${temp.getText()}`);
              });
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
    title: "探索我们提供的功能"
    exclude: "delete"
    description: "发现我们系统中可用的完整签名解决方案和操作"
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
    title: "从各种文件格式中删除签名"
    exclude: "PDF"
    description: "我们的 GroupDocs.Signature for Node.js via Java 解决方案擅长删除超过60种文件格式中的签名，确保其广泛的兼容性和功能性。"
    items: 
          
        # format loop 1
        - name: "删除 PDF 签名"
          format: "PDF"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "移除 DOCX 签名"
          format: "DOCX"
          link: "/signature/nodejs-java/delete/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "删除 PPTX 签名"
          format: "PPTX"
          link: "/signature/nodejs-java/delete/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 4
        - name: "删除 XLSX 签名"
          format: "XLSX"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---