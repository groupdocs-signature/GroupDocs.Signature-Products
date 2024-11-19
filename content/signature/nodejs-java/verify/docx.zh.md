



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:37
draft: false
lang: zh
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "通过 JavaScript 验证 DOCX 中的数字签名"
head_description: "使用 GroupDocs.Signature for Node.js via Java，您可以高效地验证 DOCX 文档中签名的真实性。无缝检查 PDF、Word、Excel、演示文稿、图像、ZIP 文件等中的签名。"

############################# Header ############################
title: "在 DOCX 中验证数字签名" 
description: "使用 GroupDocs.Signature for Node.js via Java 确保在多种文档格式（包括 PDF、Word、Excel、演示文稿、图像和 ZIP）中支持的所有电子签名的准确性和有效性。"
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "下载免费版本"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Java 的应用"
    link: "/signature/nodejs-java/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) 提供全面的文档签名管理功能，包括对 60 多种文件格式的签名能力。支持文本、图像、条形码、数字证书、元数据、印章等，GroupDocs.Signature for Node.js via Java 使您能够在 PDF、MS Office 文档、图像、ZIP 压缩包等格式中轻松搜索、验证、更新或删除签名。

############################# Steps ############################
steps:
    enable: true
    title: "如何使用 JavaScript 验证 DOCX 中的签名"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) 可以验证 DOCX 文档中特定签名的存在。Node.js via Java 开发人员可以通过集成我们的验证功能轻松提升其应用程序。
      
      1. 将 DOCX 文档加载到 Signature 实例中。
      2. 创建并配置 VerifyOptions 以实现所需的验证结果。
      3. 启动验证过程。
      4. 查看和评估验证结果。
   
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

        // 实例化包含文档的 Signature 对象
        const signature = new signatureLib.Signature('input.docx');

        // 建立 TextVerifyOptions 来验证包含指定文本的签名
        const options = new signatureLib.TextVerifyOptions();
        options.setText('signature');
        options.setMatchType(signatureLib.TextMatchType.Contains);

        // 执行文档签名的验证过程
        const result = signature.verify(options);

        // 解读和评估验证结果
        if (result.isValid()) {
            console.log('\nDocument was verified successfully!');
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "尖端文档签名技术"
  description: "GroupDocs.Signature 提供一体化解决方案，用于验证和管理各种办公格式中的签名。提供七种签名类型和完整的 CRUD 操作，便于无缝文档管理和内容安全。"
  image: "/img/signature/features_verify.webp" # 500x500 px
  image_description: "签名验证功能"
  features:
    # feature loop
    - title: "轻松签署企业文件"
      content: "以安全和定制的方式将数字签名（包括文本、图像、条形码、元数据、印章或数字证书）应用于您的文档。GroupDocs.Signature for Node.js via Java 确保企业文件签署的高效和专业。"

    # feature loop
    - title: "签名生命周期操作"
      content: "全面控制文档签名。列出文件中的所有签名，验证其真实性，根据需要更新或在必要时完全删除，确保文档处理的正确性。"

    # feature loop
    - title: "确保文档完整性"
      content: "利用数字证书保护您的文档免受未经授权的更改。使用元数据来确保和跟踪文档内容，确保其保持未经篡改和保密。"

    # feature loop
    - title: "定制化本地签名"
      content: "在 PDF 中添加个性化的本地签名，如贴纸或在 Word 文档中添加水印。这些可定制选项允许以专业和安全的方式处理文档，完全适合企业环境。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "条形码签名验证过程"
      content: |
        此示例阐明了如何验证嵌入文档中的条形码签名的方法。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // 提交包含条形码签名的文档
          const signature = new signatureLib.Signature('input.docx');

          // 配置参数以验证条形码与指定文本的匹配
          const options = new signatureLib.BarcodeVerifyOptions();
          options.setText('12345');
          options.setMatchType(signatureLib.TextMatchType.StartsWith);

          // 验证先前附加到文档上的签名
          const result = signature.verify(options);

          // 检查验证报告
          if (result.isValid()) {
              console.log('\nDocument was verified successfully!');
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
    title: "全面的功能和支持的签名"
    exclude: "verify"
    description: "探索 GroupDocs.Signature 的高级功能，具有多种签名管理工具和操作，以增强文档工作流程。"
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
    title: "各格式的全面签名验证"
    exclude: "DOCX"
    description: "GroupDocs.Signature for Node.js via Java 简化了多种文档格式的签名验证，提供强大的签名检查控制功能。自定义您的验证过程，确保文档经过适当签署。"
    items: 
          
        # format loop 1
        - name: "验证 PDF 签名"
          format: "PDF"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "验证 DOCX 签名"
          format: "DOCX"
          link: "/signature/nodejs-java/verify/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "验证 PPTX 签名"
          format: "PPTX"
          link: "/signature/nodejs-java/verify/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 4
        - name: "验证 XLSX 签名"
          format: "XLSX"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---