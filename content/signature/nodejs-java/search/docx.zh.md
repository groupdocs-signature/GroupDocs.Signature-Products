



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:13
draft: false
lang: zh
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "在 DOCX 文件中搜索电子签名，使用 JavaScript"
head_description: "利用 GroupDocs.Signature for Node.js via Java API 的强大功能，检测并搜索 PDF、Word 文档、Excel 电子表格、演示文稿和图像中的电子签名。"

############################# Header ############################
title: "在 DOCX 中搜索电子签名" 
description: "通过 GroupDocs.Signature for Node.js via Java 提供的先进工具，发现并检索 PDF、Word、Excel、演示文稿和图像文件中所有嵌入签名的详细信息。"
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费开始使用"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Java 概述"
    link: "/signature/nodejs-java/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) 提供了一个强大的框架，用于管理多种文件类型的数字签名。支持超过 60 种格式，例如 PDF、微软 Office 文档、图像和 ZIP 文件，该 API 使用户能够应用、定位、验证、更新或删除各种类型的签名，包括文本、图像、条形码、数字证书等。

############################# Steps ############################
steps:
    enable: true
    title: "使用 JavaScript 搜索 DOCX 中的签名指南"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) 提供了强大的工具，用于在 DOCX 文件中定位数字签名。Node.js via Java 开发人员可以轻松扩展应用程序功能。
      
      1. 指定要搜索签名的 DOCX 文件的路径。
      2. 使用 SearchOptions 筛选搜索结果。
      3. 执行 Search 方法以查找签名。
      4. 检查发现的签名列表。
   
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
        const signature = new signatureLib.Signature('input.docx');

        // 配置 TextSearchOptions 以包括每一页
        const options = new signatureLib.TextSearchOptions();
        options.setAllPages(true);

        // 执行搜索以定位文档中的所有文本签名
        const signatures = signature.search(signatureLib.TextSignature.class, options).toArray();
        console.log(`\nSource document contains the following text signature(s).`);

        // 聚合发现的签名以便进行全面分析
        for (const textSignature of signatures) {
            console.log(`Found Text signature at page ${textSignature.getPageNumber()} 
            with type [${textSignature.getSignatureImplementation()}] and text '${textSignature.getText()}'.`);
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "全面的签名管理解决方案"
  description: "GroupDocs.Signature for Node.js via Java 提供了一体化解决方案，以添加、修改、搜索和验证电子签名，适用于流行的文档格式。给您的工作流程带来先进的文档签署功能。"
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "签名检测功能"
  features:
    # feature loop
    - title: "对业务文件进行数字签名"
      content: "在文档的任何位置添加电子签名，例如文本、图像、条形码和数字证书。GroupDocs.Signature 支持在 PDF、Word、Excel、图像等文件中进行签名，确保灵活的文档管理。"

    # feature loop
    - title: "高效的签名管理"
      content: "签名后，轻松定位文档中嵌入的所有签名。该 API 允许全面搜索和检索签名，并具备更新或删除签名的能力。"

    # feature loop
    - title: "文档安全性和元数据管理"
      content: "通过嵌入或删除隐性元数据来确保文档的完整性。利用数字证书来封装和验证文档内容，以保护文件免受未授权的更改。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "识别图像签名"
      content: |
        此示例说明了如何在特定文档中检测图像签名。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // 将源文档作为参数提供给构造函数
          const signature = new signatureLib.Signature('input.docx');

          // 搜索任何文本类型的签名
          const signatures = signature.search(signatureLib.ImageSignature.class, signatureLib.SignatureType.Image).toArray();
          console.log(`\nSource document contains the following image signature(s).`);

          // 显示发现的签名及其完整属性
          for (const imageSignature of signatures) {
              console.log(`Found Image signature at page ${imageSignature.getPageNumber()} 
              and size ${imageSignature.getSize()}.`);
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
    title: "关键功能"
    exclude: "search"
    description: "我们的综合 API 提供了一系列旨在简化文档签名管理的操作，从签名到后处理和验证。"
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
    title: "跨多种文件类型定位签名"
    exclude: "DOCX"
    description: "使用 GroupDocs.Signature for Node.js via Java API，您可以高效地搜索和检索广泛支持的文件格式中的电子签名，从而便于将其无缝集成到文档工作流程中。"
    items: 
          
        # format loop 1
        - name: "搜索 PDF 中的签名"
          format: "PDF"
          link: "/signature/nodejs-java/search/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "查找 DOCX 中的签名"
          format: "DOCX"
          link: "/signature/nodejs-java/search/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "查找 PPTX 中的签名"
          format: "PPTX"
          link: "/signature/nodejs-java/search/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 4
        - name: "搜索 XLSX 中的签名"
          format: "XLSX"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---