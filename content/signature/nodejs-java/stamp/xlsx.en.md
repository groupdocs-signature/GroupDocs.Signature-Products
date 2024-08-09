



---
############################# Static ############################
layout: "format"
date:  2024-08-08T16:38:30
draft: false
lang: en
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Add Metadata to XLSX Files in JavaScript Applications"
head_description: "JavaScript metadata processing API to add metadata information to XLSX files. Work with metadata standards XMP, EXIF, IPTC, ID3 etc."

############################# Header ############################
title: "Adding Metadata To XLSX In JavaScript" 
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
    title: "Guidelines for Embedding Stamp Signatures in XLSX Documents Using JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) provides a powerful tool for creating and embedding stamps, which can significantly enhance Node.js via Java applications. Use this feature to craft and apply custom stamps to your document pages.
      
      1. Input the XLSX document that requires stamping.
      2. Deploy StampSignOptions to define all essential parameters.
      3. Insert as many stamp lines as needed.
      4. Apply the stamp and save the finalized document.
   
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

        // Associate the document path with the Signature instance
        const signature = new signatureLib.Signature('input.xlsx');

        // Create StampSignOptions with the necessary signature content
        const options = new signatureLib.StampSignOptions();

        // Incorporate one or more stamp lines
        const outerLine = new signatureLib.StampLine();
        outerLine.setText(" * The Best Company * ");
        outerLine.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(signatureLib.Color.WHITE);
        outerLine.setBackgroundColor(signatureLib.Color.BLUE);
        options.getOuterLines().add(outerLine);

        // Save the document with the applied stamp
        const result = signature.sign('output.xlsx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Document Metadata Management"
  description: "Our comprehensive API streamlines managing document metadata. Access, edit, and manipulate various document properties for improved organization and searchability."
  image: "/img/signature/features_stamp.webp" # 500x500 px
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
    - title: "Integrate Custom Stamps into Documents with Advanced Signature Tools"
      content: |
        Learn how to design and apply customized stamps containing essential text to your documents.
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // Provide the document for stamping
        const signature = new signatureLib.Signature('input.xlsx');

        // Set up stamp options with the desired configurations
        const signOptions = new signatureLib.StampSignOptions();

        // Specify the dimensions and position of the stamp on the page
        signOptions.setHeight(300);
        signOptions.setWidth(300);
        signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
        signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
        signOptions.setAllPages(true);

        // Include outer circular lines with custom text
        const outerLine1 = new signatureLib.StampLine();
        outerLine1.setText('* The best choice *');
        outerLine1.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
        const signatureFont1 = new signatureLib.SignatureFont();
        signatureFont1.setSize(12);
        signatureFont1.setFamilyName('Arial');
        outerLine1.setFont(signatureFont1);
        outerLine1.setHeight(30);
        outerLine1.setTextBottomIntent(6);
        outerLine1.setTextColor(signatureLib.Color.WHITE);
        outerLine1.setBackgroundColor(signatureLib.Color.BLUE);
        signOptions.getOuterLines().add(outerLine1);

        // Add inner square lines as needed
        const innerLine1 = new signatureLib.StampLine();
        innerLine1.setText('Company #1');
        innerLine1.setTextColor(signatureLib.Color.RED);
        const signFont1 = new signatureLib.SignatureFont();
        signFont1.setSize(20);
        signFont1.setBold(true);
        innerLine1.setFont(signFont1);
        innerLine1.setHeight(40);
        signOptions.getInnerLines().add(innerLine1);
        
        // Save the stamped document
        const result = signature.sign('output.xlsx', options);
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
    exclude: "XLSX"
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