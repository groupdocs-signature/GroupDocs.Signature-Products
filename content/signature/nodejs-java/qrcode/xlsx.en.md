



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:21
draft: false
lang: en
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Generate QR codes in XLSX docs with JavaScript"
head_description: "Utilize the GroupDocs.Signature API to create and integrate 2D barcodes within XLSX files. Effortlessly place QR codes on any document page."

############################# Header ############################
title: "Make QR codes for XLSX" 
description: "Create and embed 2D barcodes with customizable content, including text and numeric data, across various document types like PDFs, Word, Excel, and Images with GroupDocs.Signature for Node.js via Java."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Try It Free"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Explore GroupDocs.Signature for Node.js via Java capabilities"
    link: "/signature/nodejs-java/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) offers advanced document enhancement tools, enabling the generation and embedding of multiple signature types, including QR codes, into popular file formats. Sign and secure PDFs, Word documents, Excel spreadsheets, PowerPoint presentations, and images with Text, Image, Barcode, QR Code, Metadata, Digital, and Stamp signatures.

############################# Steps ############################
steps:
    enable: true
    title: "Guide to generating and embedding a QR code in any place within a XLSX"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) enables the creation of QR codes in various widely-used formats and their integration into XLSX pages. Supporting over 10 distinct QR code types, our solution can be seamlessly incorporated into Node.js via Java applications, enriching them with QR code signing capabilities.
      
      1. Provide the XLSX file or stream for QR code signing.
      2. Input the desired text into the QrCodeSignOptions instance.
      3. Adjust visual settings such as color, positioning, size, etc.
      4. Save the document containing the QR code.
   
    code:
      platform: "nodejs-java"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Sample signatures"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // Create a Signature instance and pass the document path
        const signature = new signatureLib.Signature('input.xlsx');

        // Leverage QrCodeSignOptions to insert a QR code into the document
        // Create QR code sign options
        const options = new signatureLib.QrCodeSignOptions('Text Content');

        // Define the signature type and placement on the page
        options.setEncodeType(signatureLib.QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);
  
        // Store the document with the newly added QR code
        signature.sign('output.xlsx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Comprehensive signature and QR code integration"
  description: "With GroupDocs.Signature for Node.js via Java API, you can manage a full spectrum of signatures. Generate, customize, verify, search, and remove signatures effortlessly across different document types, offering unmatched flexibility for your workflows."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Signature and QR code features"
  features:
    # feature loop
    - title: "Multi-format document signing"
      content: "Add multiple types of signatures, including Text, Image, Barcode, QR Code, and Stamp signatures, to any supported document format. Place them on any page, and manage document metadata. Ensure document security through digital certificates to prevent unauthorized changes."

    # feature loop
    - title: "Efficient signature validation"
      content: "Validate all signatures within a document to ensure they meet required standards. Easily retrieve and review signatures through the built-in search functionality."

    # feature loop
    - title: "Flexible signature editing"
      content: "Update or modify existing signatures, adjusting aspects such as content, location, size, and color, to suit your document’s needs after initial signing."

    # feature loop
    - title: "Signature removal made easy"
      content: "Remove any unwanted or obsolete signatures, including digital certificates, with ease. Full control over signature management ensures a clean and well-organized document."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Customizing a generated QR code"
      content: |
        This example details the process of adding a customized QR code to a XLSX page.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Obtain the document to be signed and pass it to Signature
          const signature = new signatureLib.Signature('input.xlsx');

          // Set up QR code options with the required text
          const signOptions = new signatureLib.QrCodeSignOptions('Archived on July 11, 2019');

          // Determine the QR code's position on the page
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // Specify the signature padding
          const padding = new signatureLib.Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Choose the QR code color
          signOptions.setForeColor(signatureLib.Color.RED);

          // Define the font options for the accompanying message
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Customize the background color and brush for the QR code
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new signatureLib.LinearGradientBrush(signatureLib.Color.GREEN, signatureLib.Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Embed the QR code into the document
          signature.sign('output.xlsx', signOptions);
          ```
        platform: "nodejs-java"
        copy_title: "Copy"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
          copy_tip: "click to copy"
          copy_done: "copied"
        top_links:
          #  loop
          - title: "Download result"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.xlsx"
        links:
          #  loop
          - title: "More examples"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/signature/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Ready to get started?"
  description: "Try GroupDocs.Signature features for free or request a license"
  items:
    #  loop
    - title: "NPM download"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Understand our main capabilities"
    exclude: "qrcode"
    description: "We deliver a broad selection of signature formats and operations tailored to your needs"
    items: 
          
        # operation loop 1
        - name: "Electronic signatures"
          operation: "esign"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "Add various types of signatures to supported file formats"

        # operation loop 2
        - name: "Add text to documents"
          operation: "text"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "Enhance document content with customizable text signatures"

        # operation loop 3
        - name: "Image signatures"
          operation: "image"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "Place any image at any position within a document"

        # operation loop 4
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "Create and insert various barcodes into supported documents"

        # operation loop 5
        - name: "Generate QR codes"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Generate and QR Codes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "Secure business and sign documents with digital certificates"

        # operation loop 7
        - name: "Stamp signatures"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "Use the Stamp Constructor to create custom round or square stamps"
          
        # operation loop 8
        - name: "Search signatures"
          operation: "search"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "Locate any previously added signatures within a document"
          
        # operation loop 9
        - name: "Signature verification"
          operation: "verify"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "Verify the authenticity of signatures after they have been applied"
          
        # operation loop 10
        - name: "Modify signatures"
          operation: "modify"
          link: "/signature/nodejs-java/modify/xlsx/"
          description: "Easily edit a variety of signatures within a document"
          
        # operation loop 11
        - name: "Delete signatures"
          operation: "delete"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "Remove a wide range of previously applied signatures"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Integrate QR codes with various file formats"
    exclude: "XLSX"
    description: "Leverage the Node.js via Java API to generate QR codes and embed them into a variety of widely-used file formats. Encapsulate important data in these barcodes for seamless integration and future retrieval."
    items: 
          
        # format loop 1
        - name: "QR-Code for PDF"
          format: "PDF"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "QR-Code for DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "QR-Code for JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "JPEG Image"
          
        # format loop 4
        - name: "QR-Code for PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "QR-Code for XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---