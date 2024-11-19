



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:25
draft: false
lang: en
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Generate barcode for XLSX using JavaScript Applications"
head_description: "Quickly generate and embed a barcode signature in a XLSX document with JavaScript using just a few lines of code. GroupDocs.Signature supports signing across multiple file formats."

############################# Header ############################
title: "Generate and add Barcodes in XLSX effortlessly" 
description: "Employ GroupDocs.Signature for Node.js via Java to incorporate barcodes into your business documents, placing them precisely where needed. Our solution offers extensive customization options to tailor barcode signatures to your requirements."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download Now – It's Free!"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "An introduction to GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) is a powerful document signing tool, supporting a diverse range of signature types including text, images, barcodes, digital certificates, and stamps. With compatibility across more than 60 file formats, such as PDFs, MS Office files, images, and ZIP archives, it allows for comprehensive document management. Signatures within documents can be searched, verified, altered, or removed as required.

############################# Steps ############################
steps:
    enable: true
    title: "How to generate and embed barcodes in XLSX file"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) enables the generation and placement of barcodes in a variety of popular formats on XLSX pages. With support for over 60 types of barcodes, Node.js via Java applications can be easily enhanced with barcode signing features by integrating our library.
      
      1. Provide the XLSX file or stream for processing.
      2. Pass the barcode text to a BarcodeSignOptions instance.
      3. Adjust barcode settings such as position, size, etc.
      4. Save the document with the newly added barcode.
   
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

        // Instantiate a Signature object with the document path
        const signature = new signatureLib.Signature('input.xlsx');

        // Utilize BarcodeSignOptions to integrate a barcode into the document
        const options = new signatureLib.BarcodeSignOptions('Business data');

        // Configure the barcode type and additional parameters
        options.setEncodeType(signatureLib.BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);
  
        // Save the signed document
        signature.sign('output.xlsx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Augment and secure your documents with advanced signature options"
  description: "The GroupDocs.Signature for Node.js via Java library is designed to streamline the signing and subsequent management of popular document formats. Quickly and easily add, modify, verify, or remove a wide range of signatures."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Key Functionalities of GroupDocs.Signature"
  features:
    # feature loop
    - title: "Dynamic document signing"
      content: "Sign any page of your documents using a variety of signature types, including text, images, barcodes, QR codes, and stamps. Additionally, you can embed hidden metadata, such as EXIF data in images, or secure the document against unauthorized edits using digital certificates."

    # feature loop
    - title: "Robust signature verification and search"
      content: "Our solution provides extensive tools for managing signed documents. Verify the authenticity of signatures to ensure document integrity, and utilize the search feature to list all signatures embedded within a document."

    # feature loop
    - title: "Easily edit signatures"
      content: "Most signatures added previously can be effortlessly modified. Update the text, reposition, or change the appearance of the signature to match your needs."

    # feature loop
    - title: "Streamlined signature removal"
      content: "With comprehensive support for CRUD operations, our tool allows for the efficient removal of signatures from your documents, ensuring that only the most relevant signatures remain."
      
  code_samples_ext:
    # code sample ext loop
    - title: "How to apply a barcode signature"
      content: |
        This example illustrates how to embed a customized barcode on XLSX document pages.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Provide the document to be signed
          const signature = new signatureLib.Signature('input.xlsx');

          // Utilize BarcodeSignOptions to integrate a barcode into the document
          const signOptions = new signatureLib.BarcodeSignOptions('Accepted');
          signOptions.setEncodeType(signatureLib.BarcodeTypes.Code39FullASCII);

          // Configure the barcode type and additional parameters
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Left);

          // Define the barcode padding from the page edge
          const padding = new signatureLib.Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // Choose the bar color
          signOptions.setForeColor(signatureLib.Color.RED);

          // Specify the font style for the message
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName('Arial');
          signOptions.setFont(font);

          // Indicate the position of the message
          signOptions.setCodeTextAlignment(signatureLib.CodeTextAlignment.Above);

          // Sign and save the document
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
            link: "/examples/signature/formats/signature_barcode.xlsx"
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
    title: "Dive into our primary features"
    exclude: "barcode"
    description: "Experience a broad array of signature types and tools we provide"
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
    title: "Sign across multiple document formats"
    exclude: "XLSX"
    description: "The Node.js via Java API empowers you to sign over 60 different formats. Whether adding signatures to specific pages or positioning them precisely, our tool makes it easy to apply various signature types."
    items: 
          
        # format loop 1
        - name: "Add barcode to PDF"
          format: "PDF"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Add barcode to DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Add barcode to JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "JPEG Image"
          
        # format loop 4
        - name: "Add barcode to PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/barcode/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "Add barcode to XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---