



---
############################# Static ############################
layout: "format"
date:  2024-08-07T18:32:11
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
    title: "Guidelines for Removing Text Signatures from PDF using JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) enables Node.js via Java developers to efficiently remove text signatures in PDF files by following a series of simple steps.
      
      1. Provide the PDF file path to an instance of the Signature class.
      2. Utilize the Search method to identify all text signatures in the document.
      3. Remove one or more of the identified text signatures.
      4. Review the results of the document processing.
   
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

        // Pass the document with the signatures to the Signature instance
        const signature = new signatureLib.Signature('input.pdf');

        // Erase all QR-code signatures
        const options = new signatureLib.TextSearchOptions();
        const signatures = signature.search(signatureLib.TextSignature.class, options);

        // Remove the first detected text signature
        if(signatures.size() > 0)
        {
            const textSignature = signatures[0];
            const result = signature.delete('output.pdf', textSignature);

            // Handle the result of the deletion
            if(result)
            {
                console.log(`\nSignature was deleted successfully`);
            }
        }

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
    - title: "Remove All QR-Code Signatures"
      content: |
        Learn the procedure to eliminate all QR-code signatures embedded in a document.
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // Provide a document that includes QR-code signatures
        const signature = new signatureLib.Signature('input.pdf');

        // Erase all QR-code signatures
        const result = await signature.delete('output.pdf', signatureLib.SignatureType.QrCode);
        if (result.getSucceeded().size() > 0) {

            // Review the outcome of the deletion
            console.log('Following QR-Code signatures were deleted:');
            let number = 1;
            result.getSucceeded().toArray().forEach((o) => {
                const temp = o;
                console.log(`Signature #${number++}: Type: ${temp.getSignatureType()}, 
                Id: ${temp.getSignatureId()}, Text: ${temp.getText()}`);
            });
        }
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