



---
############################# Static ############################
layout: "format"
date:  2024-09-06T10:45:40
draft: false
lang: en
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Efficiently Erase Signatures from DOCX Files Using JavaScript"
head_description: "Elevate your JavaScript applications by integrating GroupDocs.Signature for Node.js via Java, a powerful tool designed to seamlessly remove embedded signatures from DOCX files."

############################# Header ############################
title: "Effortlessly Erase Signatures from DOCX with JavaScript" 
description: "Our comprehensive solution extends beyond simple document signing, offering robust features within GroupDocs.Signature for Node.js via Java to locate and delete a wide array of signatures."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Get Your Free Download"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Discover GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) represents a sophisticated solution for intricate metadata management and manipulation. It provides the ability to view, update, remove, search, compare, exchange, and export metadata across diverse image and document formats, all without relying on external software. Integrate metadata into Word documents, Excel spreadsheets, PowerPoint presentations, Outlook emails, OneNote notebooks, Visio diagrams, Project files, PDFs, AutoCAD drawings, ZIP archives, as well as audio and video formats, among others.

############################# Steps ############################
steps:
    enable: true
    title: "Guidelines for Removing Text Signatures from DOCX using JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) enables Node.js via Java developers to efficiently remove text signatures in DOCX files by following a series of simple steps.
      
      1. Provide the DOCX file path to an instance of the Signature class.
      2. Utilize the Search method to identify all text signatures in the document.
      3. Remove one or more of the identified text signatures.
      4. Review the results of the document processing.
   
    code:
      platform: "nodejs-java"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/signature_all.pdf"
      result_title: "Download signatures"
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
        const signature = new signatureLib.Signature('input.docx');

        // Erase all QR-code signatures
        const options = new signatureLib.TextSearchOptions();
        const signatures = signature.search(signatureLib.TextSignature.class, options);

        // Remove the first detected text signature
        if(signatures.size() > 0)
        {
            const textSignature = signatures[0];
            const result = signature.delete('output.docx', textSignature);

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
  title: "Enhance Document Security with Signature Tools"
  description: "GroupDocs.Signature for Node.js via Java is specifically crafted to streamline the signing and management of business file formats, allowing you to add, edit, verify, or remove signatures with precision."
  image: "/img/signature/features_delete.webp" # 500x500 px
  image_description: "Explore the Comprehensive Capabilities of GroupDocs.Signature"
  features:
    # feature loop
    - title: "Comprehensive Document Signing"
      content: "Add text, image, barcode, QR code, or stamp signatures to any page of supported documents effortlessly. Utilize hidden metadata like EXIF in images, or secure document integrity with digital certificates to prevent unauthorized modifications."

    # feature loop
    - title: "Signature Search and Validation"
      content: "Our tools enable thorough verification of document signatures, ensuring their authenticity. Perform comprehensive searches to retrieve all signatures within your documents, enhancing document control."

    # feature loop
    - title: "Edit Existing Signatures"
      content: "Easily modify previously added signatures by adjusting text, altering position, or changing colors to meet your specific requirements."

    # feature loop
    - title: "Remove Unwanted Signatures"
      content: "With full CRUD capabilities, our solution enables the efficient deletion of a wide range of signature types from your documents, ensuring flexibility and control."
      
  code_samples:
    # code sample loop
    - title: "Remove All QR-Code Signatures"
      content: |
        Learn the procedure to eliminate all QR-code signatures embedded in a document.
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // Provide a document that includes QR-code signatures
        const signature = new signatureLib.Signature('input.docx');

        // Erase all QR-code signatures
        const result = await signature.delete('output.docx', signatureLib.SignatureType.QrCode);
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


############################# More Operations #####################
more_operations:
    enable: true
    title: "Explore the Features We Provide"
    exclude: "delete"
    description: "Discover the full range of signature solutions and operations available in our system"
    items: 
          
        # operation loop 1
        - name: "Electronic Signatures"
          operation: "esign"
          link: "/signature/nodejs-java/esign/docx/"
          description: "Add various types of signatures to supported file formats."

        # operation loop 2
        - name: "Add Text to Documents"
          operation: "text"
          link: "/signature/nodejs-java/text/docx/"
          description: "Enhance document content with customizable text signatures."

        # operation loop 3
        - name: "Image Signatures"
          operation: "image"
          link: "/signature/nodejs-java/image/docx/"
          description: "Place any image at any position within a document."

        # operation loop 4
        - name: "Generate Barcodes"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "Create and insert various barcodes into supported documents."

        # operation loop 5
        - name: "Generate QR Codes"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "Generate and apply two-dimensional barcodes, including QR codes, for document signing."
          
        # operation loop 6
        - name: "Digital Certificates"
          operation: "digital"
          link: "/signature/nodejs-java/digital/docx/"
          description: "Secure business documents using digital certificates."

        # operation loop 7
        - name: "Stamp Signatures"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "Use the Stamp Constructor to create custom round or square stamps."
          
        # operation loop 8
        - name: "Search Signatures"
          operation: "search"
          link: "/signature/nodejs-java/search/docx/"
          description: "Locate any previously added signatures within a document."
          
        # operation loop 9
        - name: "Signature Verification"
          operation: "verify"
          link: "/signature/nodejs-java/verify/docx/"
          description: "Verify the authenticity of signatures after they have been applied."
          
        # operation loop 10
        - name: "Modify Signatures"
          operation: "modify"
          link: "/signature/nodejs-java/modify/docx/"
          description: "Easily edit a variety of signatures within a document."
          
        # operation loop 11
        - name: "Delete Signatures"
          operation: "delete"
          link: "/signature/nodejs-java/delete/docx/"
          description: "Remove a wide range of previously applied signatures."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Eliminate Signatures from Various File Formats"
    exclude: "DOCX"
    description: "Our GroupDocs.Signature for Node.js via Java solution is proficient in removing signatures across a diverse range of over 60 file formats, ensuring broad compatibility and functionality."
    items: 
          
        # format loop 1
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/delete/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Watermark JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/delete/jpeg/"
          description: "JPEG Image"
          
        # format loop 3
        - name: "Watermark PDF"
          format: "PDF"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 4
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/delete/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---