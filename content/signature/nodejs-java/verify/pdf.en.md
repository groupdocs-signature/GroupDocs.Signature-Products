



---
############################# Static ############################
layout: "format"
date:  2024-10-08T11:43:33
draft: false
lang: en
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Verify digital signatures in PDF via JavaScript"
head_description: "With GroupDocs.Signature for Node.js via Java, you can efficiently verify the authenticity of signatures within PDF documents. Seamlessly check signatures in PDFs, Word, Excel, Presentations, Images, ZIP files, and more."

############################# Header ############################
title: "Verify digital signatures in PDF" 
description: "Ensure the accuracy and validity of all supported e-signatures in a wide array of document formats, including PDF, Word, Excel, Presentations, Images, and ZIP, using GroupDocs.Signature for Node.js via Java."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download the free version"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Applications of GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) offers comprehensive document signature management, including the ability to sign over 60 file formats. With support for text, image, barcode, digital certificates, metadata, stamps, and more, GroupDocs.Signature for Node.js via Java empowers you to search, verify, update, or remove signatures effortlessly in formats such as PDFs, MS Office documents, Images, ZIP archives, and more.

############################# Steps ############################
steps:
    enable: true
    title: "How to verify signatures in PDF using JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) can authenticate the presence of specific signatures in a PDF document. Node.js via Java developers can effortlessly enhance their applications by incorporating our verification features.
      
      1. Load the PDF document into the Signature instance.
      2. Create and configure VerifyOptions to achieve the desired verification results.
      3. Initiate the verification process.
      4. Review and assess the verification outcomes.
   
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

        // Instantiate a Signature object with the document
        const signature = new signatureLib.Signature('input.pdf');

        // Establish TextVerifyOptions to validate signatures that include specified text
        const options = new signatureLib.TextVerifyOptions();
        options.setText('signature');
        options.setMatchType(signatureLib.TextMatchType.Contains);

        // Execute the verification process for document signatures
        const result = signature.verify(options);

        // Interpret and assess the outcomes of the verification
        if (result.isValid()) {
            console.log('\nDocument was verified successfully!');
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Cutting-edge document signing technology"
  description: "GroupDocs.Signature provides an all-in-one solution for verifying and managing signatures in various office formats. Offering seven signature types and full CRUD operations, it allows for seamless document management and content security."
  image: "/img/signature/features_verify.webp" # 500x500 px
  image_description: "Signature verification features"
  features:
    # feature loop
    - title: "Sign corporate documents with ease"
      content: "Apply digital signatures—whether text-based, image, barcode, metadata, stamps, or digital certificates—to your documents in a secure and customized manner. GroupDocs.Signature for Node.js via Java ensures streamlined and professional corporate document signing."

    # feature loop
    - title: "Signature lifecycle operations"
      content: "Gain full control over document signatures. List all signatures in a file, verify their authenticity, update them as required, or remove them entirely when necessary, ensuring proper document processing."

    # feature loop
    - title: "Ensure document integrity"
      content: "Leverage digital certificates to protect your documents from unauthorized changes. Use metadata to secure and track document content, ensuring it remains untampered and confidential."

    # feature loop
    - title: "Customized native signatures"
      content: "Add tailored native signatures like stickers in PDFs or watermarks in Word documents. These customizable options allow for professional and secure document handling, perfectly suited to corporate environments."
      
  code_samples:
    # code sample loop
    - title: "Barcode signatures verification process"
      content: |
        This example elucidates the methodology for authenticating barcode signatures embedded within a document.
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // Submit the document featuring barcode signatures
        const signature = new signatureLib.Signature('input.pdf');

        // Configure the parameters to validate barcodes against designated text
        const options = new signatureLib.BarcodeVerifyOptions();
        options.setText('12345');
        options.setMatchType(signatureLib.TextMatchType.StartsWith);

        // Authenticate the signatures previously affixed to the document
        const result = signature.verify(options);

        // Check validation report
        if (result.isValid()) {
            console.log('\nDocument was verified successfully!');
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
    title: "Comprehensive features and supported signatures"
    exclude: "verify"
    description: "Explore the advanced capabilities of GroupDocs.Signature, featuring a diverse range of signature management tools and operations for enhanced document workflows."
    items: 
          
        # operation loop 1
        - name: "Electronic signatures"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "Add various types of signatures to supported file formats"

        # operation loop 2
        - name: "Add text to documents"
          operation: "text"
          link: "/signature/nodejs-java/text/pdf/"
          description: "Enhance document content with customizable text signatures"

        # operation loop 3
        - name: "Image signatures"
          operation: "image"
          link: "/signature/nodejs-java/image/pdf/"
          description: "Place any image at any position within a document"

        # operation loop 4
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "Create and insert various barcodes into supported documents"

        # operation loop 5
        - name: "Generate QR codes"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Generate and apply two-dimensional barcodes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Secure business documents using digital certificates"

        # operation loop 7
        - name: "Stamp signatures"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pdf/"
          description: "Use the Stamp Constructor to create custom round or square stamps"
          
        # operation loop 8
        - name: "Search signatures"
          operation: "search"
          link: "/signature/nodejs-java/search/pdf/"
          description: "Locate any previously added signatures within a document"
          
        # operation loop 9
        - name: "Signature verification"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "Verify the authenticity of signatures after they have been applied"
          
        # operation loop 10
        - name: "Modify signatures"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pdf/"
          description: "Easily edit a variety of signatures within a document"
          
        # operation loop 11
        - name: "Delete signatures"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "Remove a wide range of previously applied signatures"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Comprehensive signature validation for various formats"
    exclude: "PDF"
    description: "GroupDocs.Signature for Node.js via Java simplifies signature verification across multiple document formats, offering robust controls for signature checks. Customize your verification process and ensure documents are signed appropriately."
    items: 
          
        # format loop 1
        - name: "Verify PDF signatures"
          format: "PDF"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Verify DOCX signatures"
          format: "DOCX"
          link: "/signature/nodejs-java/verify/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Verify PPTX signatures"
          format: "PPTX"
          link: "/signature/nodejs-java/verify/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Verify XLSX signatures"
          format: "XLSX"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---