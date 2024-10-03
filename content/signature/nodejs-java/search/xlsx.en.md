



---
############################# Static ############################
layout: "format"
date:  2024-10-03T12:33:02
draft: false
lang: en
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Search for e-signatures in XLSX files with JavaScript"
head_description: "Harness the power of the GroupDocs.Signature for Node.js via Java API to detect and search for electronic signatures across PDFs, Word documents, Excel spreadsheets, Presentations, and Images."

############################# Header ############################
title: "Search for e-signatures in XLSX" 
description: "Discover and retrieve detailed information about all embedded signatures in PDFs, Word, Excel, Presentations, and Image files using the advanced tools provided by GroupDocs.Signature for Node.js via Java."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Get started for free"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Overview of GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) offers a robust framework for managing digital signatures across a wide spectrum of file types. Supporting over 60 formats such as PDF, Microsoft Office documents, Images, and ZIP files, the API enables users to apply, locate, verify, update, or remove a variety of signature types, including text, images, barcodes, digital certificates, and more.

############################# Steps ############################
steps:
    enable: true
    title: "Guide to searching for signatures in XLSX using JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) provides a powerful tool for locating digital signatures within XLSX files. Node.js via Java developers can easily extend their application functionality with our solution.
      
      1. Specify the path of the XLSX file for signature search.
      2. Use SearchOptions to filter the search results.
      3. Execute the Search method to find the signatures.
      4. Review the list of discovered signatures.
   
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

        // Instantiate a Signature object using the document path
        const signature = new signatureLib.Signature('input.xlsx');

        // Configure TextSearchOptions to include every page
        const options = new signatureLib.TextSearchOptions();
        options.setAllPages(true);

        // Perform a search to locate all text signatures within the document
        const signatures = signature.search(signatureLib.TextSignature.class, options).toArray();
        console.log(`\nSource document contains the following text signature(s).`);

        // Aggregate the discovered signatures for comprehensive analysis
        for (const textSignature of signatures) {
            console.log(`Found Text signature at page ${textSignature.getPageNumber()} 
            with type [${textSignature.getSignatureImplementation()}] and text '${textSignature.getText()}'.`);
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Complete signature management solution"
  description: "GroupDocs.Signature for Node.js via Java provides an all-in-one solution for adding, modifying, searching, and verifying electronic signatures across popular document formats. Empower your workflows with advanced document signing features."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "Signature detection features"
  features:
    # feature loop
    - title: "Digitally sign business files"
      content: "Add electronic signatures such as text, image, barcode, and digital certificates to any location within your documents. GroupDocs.Signature supports signing in PDFs, Word, Excel, Images, and more, ensuring flexible document management."

    # feature loop
    - title: "Efficient signature management"
      content: "After signing, easily locate all signatures embedded within a document. The API allows for comprehensive searching and retrieval of signatures, as well as the ability to update or remove them."

    # feature loop
    - title: "Document security and metadata management"
      content: "Secure the integrity of your documents by embedding or removing hidden metadata. Protect your files from unauthorized changes by utilizing digital certificates to seal and authenticate document content."
      
  code_samples:
    # code sample loop
    - title: "Identifying image signatures"
      content: |
        This example elucidates how to detect an image signature within a specific document.
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // Supply the source document as a parameter to the constructor
        const signature = new signatureLib.Signature('input.xlsx');

        // Search for any signatures that are of the text type
        const signatures = signature.search(signatureLib.ImageSignature.class, signatureLib.SignatureType.Image).toArray();
        console.log(`\nSource document contains the following image signature(s).`);

        // Display the findings with comprehensive properties of the detected signatures
        for (const imageSignature of signatures) {
            console.log(`Found Image signature at page ${imageSignature.getPageNumber()} 
            and size ${imageSignature.getSize()}.`);
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


############################# More Operations #####################
more_operations:
    enable: true
    title: "Key functionalities"
    exclude: "search"
    description: "Our comprehensive API delivers a range of operations designed to streamline the management of document signatures, from signing to post-processing and verification."
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
          description: "Generate and apply two-dimensional barcodes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "Secure business documents using digital certificates"

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
    title: "Locate signatures across multiple file types"
    exclude: "XLSX"
    description: "With GroupDocs.Signature for Node.js via Java API, you can efficiently search and retrieve electronic signatures from a wide range of supported file formats, facilitating seamless integration into your document workflows."
    items: 
          
        # format loop 1
        - name: "Search signatures in PDF"
          format: "PDF"
          link: "/signature/nodejs-java/search/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Search signatures in DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/search/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Search signatures in PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/search/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Search signatures in XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---