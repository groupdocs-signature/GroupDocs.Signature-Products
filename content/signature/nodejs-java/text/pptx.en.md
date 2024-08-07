



---
############################# Static ############################
layout: "format"
date:  2024-08-07T18:32:06
draft: false
lang: en
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Add Metadata to PPTX Files in JavaScript Applications"
head_description: "JavaScript metadata processing API to add metadata information to PPTX files. Work with metadata standards XMP, EXIF, IPTC, ID3 etc."

############################# Header ############################
title: "Adding Metadata To PPTX In JavaScript" 
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
    title: "Procedure to Add Text Signatures to PPTX Documents Using JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) enables the addition of text signatures to PPTX documents within Node.js via Java applications. Quickly enhance your product's capabilities with our robust solutions.
      
      1. Provide the PPTX document as an argument to the Signature class.
      2. Instantiate TextSignOptions with the required text.
      3. Set the visual properties of the text signature.
      4. Add the text signature to the desired page(s) of the document.
   
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

        // Initialize the Signature class with the document path
        const signature = new signatureLib.Signature('input.pptx');

        // Create TextSignOptions with the required signature text
        const options = new signatureLib.TextSignOptions('John Smith');

        // Configure the text color and font properties
        options.setForeColor(new signatureLib.Color(255, 0, 0));
        const signatureFont = new signatureLib.SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName('Comic Sans MS');
        options.setFont(signatureFont);
        
        // Add the text signature to the document
        const result = signature.sign('output.pptx', options);
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
    - title: "Implement Text Signatures in Documents"
      content: |
        Learn how to embed text signatures into business documents to optimize processes.
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // Choose the document to be signed
        const signature = new signatureLib.Signature('input.pptx');

        // Define text options with the specified content
        const options = new signatureLib.TextSignOptions('Rescheduled to 03/04/2025');

        // Set the size and position of the signature on the page
        options.setLeft(100);
        options.setTop(100);
        options.setWidth(100);
        options.setHeight(30);

        // Apply padding for the signature from the page edges
        const padding = new signatureLib.Padding();
        padding.setBottom(20);
        padding.setRight(20);
        options.setMargin(padding);

        // Customize the text color and font style
        options.setForeColor(signatureLib.Color.RED);
        const signatureFont = new signatureLib.SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName('Comic Sans MS');
        options.setFont(signatureFont);

        // Add a border to the text signature if desired
        const border = new signatureLib.Border();
        border.setColor(signatureLib.Color.GREEN);
        border.setDashStyle(signatureLib.DashStyle.DashLongDashDot);
        border.setTransparency(0.5);
        border.setVisible(true);
        border.setWeight(2);
        options.setBorder(border);

        // Configure the background of the signature
        const background = new signatureLib.Background();
        background.setColor(signatureLib.Color.LIGHT_GRAY);
        background.setTransparency(0.5);
        const brush = new signatureLib.LinearGradientBrush
            (signatureLib.Color.GREEN, signatureLib.Color.DARK_GRAY, 0);
        background.setBrush(brush);
        options.setBackground(background);

        // Rotate the signature as needed on the page
        options.setRotationAngle(45);

        // Optionally, save the text as an image for compatibility
        options.setSignatureImplementation(signatureLib.TextSignatureImplementation.Image);
        
        // Customize the text color and font style
        const result = signature.sign('output.pptx', options);
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
    exclude: "PPTX"
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