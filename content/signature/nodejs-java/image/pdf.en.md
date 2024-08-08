



---
############################# Static ############################
layout: "format"
date:  2024-08-08T16:38:31
draft: false
lang: en
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Add Metadata to PDF Files in JavaScript Applications"
head_description: "JavaScript metadata processing API to add metadata information to PDF files. Work with metadata standards XMP, EXIF, IPTC, ID3 etc."

############################# Header ############################
title: "Adding Metadata To PDF In JavaScript" 
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
    title: "Procedure for Embedding Images in PDF Pages Using JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) empowers Node.js via Java applications to seamlessly integrate image signatures into PDF documents. Enhance your application's capabilities with our comprehensive library.
      
      1. Instantiate Signature with the PDF document
      2. Utilize ImageSignOptions to specify the signature image
      3. Position the image precisely on any page
      4. Save the signed document to the desired location
   
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

        // Initialize Signature with the path to the document
        const signature = new signatureLib.Signature('input.pdf');

        // Configure ImageSignOptions to include the desired image signature
        const options = new signatureLib.ImageSignOptions('boss_signature.jpg');

        // Place the image at the top-left corner across all pages
        options.setAllPages(true);
        options.setLeft(100);
        options.setTop(100);
        
        // Save the document with the applied image signature
        const result = signature.sign('output.pdf', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Document Metadata Management"
  description: "Our comprehensive API streamlines managing document metadata. Access, edit, and manipulate various document properties for improved organization and searchability."
  image: "/img/signature/features_image.webp" # 500x500 px
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
    - title: "Enhance Documents with Image Signatures"
      content: |
        Learn how to incorporate images into business documents to add supplementary information.
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // Select the document to be signed
        const signature = new signatureLib.Signature('input.pdf');

        // Configure image options with the image path
        const options = new signatureLib.ImageSignOptions('organization_seal.jpg');

        // Adjust the size of the image signature
        options.setWidth(100);
        options.setHeight(100);

        // Place the image at the bottom-right corner
        options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
        options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

        // Apply padding from the page corners if needed
        const padding = new signatureLib.Padding();
        padding.setRight(120);
        padding.setBottom(120);
        options.setMargin(padding);

        // Optionally, add a custom border to the image
        const border = new signatureLib.Border();
        border.setColor(signatureLib.Color.GREEN);
        border.setDashStyle(signatureLib.DashStyle.DashLongDashDot);
        border.setWeight(5);
        border.setVisible(true);
        options.setBorder(border);

        // Rotate the image signature for optimal appearance
        options.setRotationAngle(45);

        // Save the updated document to the desired location
        const result = signature.sign('output.pdf', options);
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
    exclude: "PDF"
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