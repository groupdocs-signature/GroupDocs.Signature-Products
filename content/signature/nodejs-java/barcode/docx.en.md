



---
############################# Static ############################
layout: "format"
date:  2024-08-07T18:32:08
draft: false
lang: en
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Add Metadata to DOCX Files in JavaScript Applications"
head_description: "JavaScript metadata processing API to add metadata information to DOCX files. Work with metadata standards XMP, EXIF, IPTC, ID3 etc."

############################# Header ############################
title: "Adding Metadata To DOCX In JavaScript" 
description: "Add custom metadata properties to a wide range of business documents, images, audio & video file formats using GroupDocs.Signature for Node.js via Java."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download Free Trial"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "About GroupDocs.Signature for Node.js via Java API"
    link: "/signature/nodejs-java/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) is an advanced metadata fields management and manipulation solution to easily view, update, remove, find, compare, exchange and export metadata information from images and document formats without using any external software. Add metadata details to Word documents, Excel spreadsheets, PowerPoint presentations, Outlook emails, OneNote, Visio, Project, PDF, AutoCAD, ZIp, Audio and Video file formats along with the support for working with many other metadata processing features.

############################# Steps ############################
steps:
    enable: true
    title: "Instructions for Generating and Embedding Barcodes in DOCX Documents"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) enables the generation and placement of barcodes in a variety of popular formats on DOCX pages. With support for over 60 types of barcodes, Node.js via Java applications can be easily enhanced with barcode signing features by integrating our library.
      
      1. Provide the DOCX file or stream for processing.
      2. Pass the barcode text to a BarcodeSignOptions instance.
      3. Adjust barcode settings such as position, size, etc.
      4. Save the document with the newly added barcode.
   
    code:
      platform: "nodejs-java"
      copy_title: "Copy"
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
        const signature = new signatureLib.Signature('input.docx');

        // Utilize BarcodeSignOptions to integrate a barcode into the document
        const options = new signatureLib.BarcodeSignOptions('Business data');

        // Configure the barcode type and additional parameters
        options.setEncodeType(signatureLib.BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);
  
        // Save the signed document
        signature.sign('output.docx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Document Metadata Management"
  description: "Our comprehensive API streamlines managing document metadata. Access, edit, and manipulate various document properties for improved organization and searchability."
  image: "/img/signature/features_delete.webp" # 500x500 px
  image_description: "Metadata Functionality"
  features:
    # feature loop
    - title: "Metadata Access"
      content: "Effortlessly retrieve and process a document's metadata. Gain insights into properties like author, creation date, and many others."

    # feature loop
    - title: "Metadata Editing"
      content: "Modify document metadata directly. Update properties for better organization, searchability, and information accuracy."

    # feature loop
    - title: "Advanced Metadata Management"
      content: "Perform complex operations on document metadata. Efficiently handle tasks like adding custom properties, deleting irrelevant data, and ensuring data consistency."
      
  code_samples:
    # code sample loop
    - title: "How to Customize a Barcode Signature"
      content: |
        This example illustrates how to embed a customized barcode on DOCX document pages.
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // Provide the document to be signed
        const signature = new signatureLib.Signature('input.docx');

        // Utilize BarcodeSignOptions to integrate a barcode into the document
        const signOptions = new signatureLib.BarcodeSignOptions('Accepted for review on February 15, 2020');

        // Configure the barcode type and additional parameters
        signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
        signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

        // Define the barcode padding from the page edge
        const padding = new signatureLib.Padding();
        padding.setLeft(20);
        padding.setTop(20);
        signOptions.setMargin(padding);

        // Choose the bar color
        signOptions.setForeColor(signatureLib.Color.RED);

        // Specify the font style for the message
        const font = new signatureLib.SignatureFont();
        font.setSize(12);
        font.setFamilyName('Comic Sans MS');
        signOptions.setFont(font);

        // Indicate the position of the message
        signOptions.setCodeTextAlignment(signatureLib.CodeTextAlignment.Above);

        // Sign and save the document
        signature.sign('output.docx', signOptions);
        ```
        {{< /landing/code >}}


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


############################# More Formats #####################
more_formats:
    enable: true
    title: "Adding Metadata Properties To Other File Formats"
    exclude: "DOCX"
    description: "Multi format documents and images metadata addition API for Node.js via Java. Retrieve metadata of some of the popular file formats as stated below."
    items: 
          
        # format loop 1
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Watermark JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java//jpeg/"
          description: "JPEG Image"
          
        # format loop 3
        - name: "Watermark PDF"
          format: "PDF"
          link: "/signature/nodejs-java//pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 4
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---