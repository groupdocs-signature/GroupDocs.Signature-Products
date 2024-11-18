



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:59
draft: false
lang: zh
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "使用JavaScript为PPTX文件添加数字电子签名"
head_description: "仅需几行代码即可使用JavaScript在PPTX文件上添加数字签名。使用GroupDocs.Signature for Node.js via Java对多种文件格式进行签名。"

############################# Header ############################
title: "通过数字证书保护PPTX" 
description: "利用GroupDocs.Signature for Node.js via Java的高级功能，在您的业务文档中嵌入数字证书，以确保其安全性。我们提供灵活的选项来保护和验证您的文档。"
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
    title: "GroupDocs.Signature for Node.js via Java介绍"
    link: "/signature/nodejs-java/"
    link_title: "了解更多"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) 是一款全面的签署解决方案，旨在满足各种文档处理需求。它允许您在超过60种不同的文件格式（包括PDF、MS Office、图像和ZIP文件）中嵌入文本、图像、数字证书和印章。此外，已签署的文档可以方便地进行搜索、验证、编辑或在必要时删除。

############################# Steps ############################
steps:
    enable: true
    title: "在JavaScript中使用数字证书保护PPTX的指南"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/)使Node.js via Java开发人员能够通过使用数字签名保护PPTX文档免于修改。通过全面的数据安全功能增强您的业务应用程序。
      
      1. 将PPTX文档传递给Signature类构造函数。
      2. 应用数字证书及其相应的密码以保护文档。
      3. 可选择在文档页面上添加数字签名的可视表示。
      4. 对文档签名以防止未来的任何更改。
   
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

        // 利用Signature为文档应用数字签名
        const signature = new signatureLib.Signature('input.pptx');

        // 提供所需的数字证书和密码
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // 如有必要，配置视觉签名设置
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);
        
        // 使用数字证书对文档进行加密
        const result = signature.sign('output.pptx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "通过签名优化或保护文档内容"
  description: "GroupDocs.Signature for Node.js via Java旨在签署所有主要文件格式，使您能够轻松地添加、调整、验证或删除各种类型的签名。"
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "GroupDocs.Signature的主要功能"
  features:
    # feature loop
    - title: "为文档添加签名"
      content: "轻松在任何受支持文档的任意页面上放置文本、图像、条形码、二维码或印章签名。您还可以插入或编辑隐藏的元数据，例如图像中的EXIF。通过数字证书保护文档内容，防止未授权的更改。"

    # feature loop
    - title: "定位并验证签名"
      content: "签名后，您的文档可以进行多次验证。确认已签署内容的完整性，或进行详细搜索以列出所有现有签名。"

    # feature loop
    - title: "修订现有签名"
      content: "大多数签名类型允许在创建后进行编辑。您可以轻松修改文本、重新定位元素、调整颜色、调整大小并进行其他必要的更改。"

    # feature loop
    - title: "消除不必要的签名"
      content: "我们的解决方案支持签名的完整CRUD操作。如有需要，您可以从文档中删除多种签名类型，包括数字证书。"
      
  code_samples:
    # code sample loop
    - title: "使用数字签名保护文档"
      content: |
        了解如何使用数字签名锁定文档以防止更改。
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // 提供需要签名的文档
        const signature = new signatureLib.Signature('input.pptx');

        // 使用适当的数字证书及其密码
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // 添加额外的文本信息
        options.setReason('Security issue');
        options.setContact('John Smith');
        options.setLocation('Office D.W.');

        // 添加例如图像等视觉元素来表示签名
        options.setImageFilePath('image.png');
        options.setAllPages(true);
        options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
        options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        const padding = new signatureLib.Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);
        
        // 将数字安全文档保存到指定位置
        const result = signature.sign('output.pptx', options);
        ```
        {{< /landing/code >}}


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
    exclude: "digital"
    description: "我们自豪地支持全面的签名选项和功能"
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
    title: "在多种格式中对文档进行签名"
    exclude: "PPTX"
    description: "Node.js via Java API支持超过60种格式，使您能够在任何页面上应用多种签名，通过数字证书强制内容安全，并有效地管理文档中的签名。"
    items: 
          
        # format loop 1
        - name: "保护 PDF"
          format: "PDF"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 2
        - name: "保护 DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/digital/docx/"
          description: "Microsoft Word 开放 XML 文档"
          
        # format loop 3
        - name: "保护 PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "PowerPoint 开放 XML 演示文稿"
          
        # format loop 4
        - name: "保护 XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "Microsoft Excel 开放 XML 电子表格"


          

---