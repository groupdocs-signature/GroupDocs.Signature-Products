



---
############################# Static ############################
layout: "format"
date:  2024-10-03T12:32:59
draft: false
lang: en
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Add text signatures to XLSX via JavaScript"
head_description: "Utilize the JavaScript API to seamlessly integrate text signatures into XLSX documents. Our API supports a broad spectrum of formats, including PDF, Word, Excel, Presentations, Images, and ZIP files."

############################# Header ############################
title: "Add text signatures to XLSX" 
description: "Incorporate personalized text signatures into your business files with GroupDocs.Signature for Node.js via Java. Take control of your document workflows by enhancing them with secure and customizable signature options."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Start free trial"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Introducing GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) is an innovative solution designed to facilitate the addition of text signatures to documents. Customize and place signatures on any page, improving efficiency in document handling. Streamline your organization's workflows by integrating personalized text markings that enhance both functionality and professionalism.

############################# Steps ############################
steps:
    enable: true
    title: "Guide to creating text signatures for XLSX using JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) enables the addition of text signatures to XLSX documents within Node.js via Java applications. Quickly enhance your product's capabilities with our robust solutions.
      
      1. Provide the XLSX document as an argument to the Signature class.
      2. Instantiate TextSignOptions with the required text.
      3. Set the visual properties of the text signature.
      4. Add the text signature to the desired page(s) of the document.
   
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

        // Initialize the Signature class with the document path
        const signature = new signatureLib.Signature('input.xlsx');

        // Create TextSignOptions with the required signature text
        const options = new signatureLib.TextSignOptions('John Smith');

        // Configure the text color and font properties
        options.setForeColor(new signatureLib.Color(255, 0, 0));
        const signatureFont = new signatureLib.SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName('Comic Sans MS');
        options.setFont(signatureFont);
        
        // Add the text signature to the document
        const result = signature.sign('output.xlsx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Enhanced text signature control"
  description: "With GroupDocs.Signature for Node.js via Java, you can greatly improve the management of text-based signatures in key document formats. The tool allows you to configure the style, placement, and content of signatures with ease, enabling businesses to tailor their document processes."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "Core features of GroupDocs.Signature"
  features:
    # feature loop
    - title: "Dynamic document signatures"
      content: "Insert various types of signatures—such as text, images, barcodes, QR codes, or stamps—on any page of supported documents. Embed metadata to carry hidden information or apply digital certificates for advanced security measures."

    # feature loop
    - title: "Signature search and validation"
      content: "Verify the authenticity of signatures embedded within your documents. Perform efficient searches to locate all signature instances, ensuring thorough document tracking and management."

    # feature loop
    - title: "Edit or remove signatures"
      content: "Modify or delete previously added signatures as needed. You can adjust the appearance, position, or content of any signature to meet evolving requirements, ensuring flexibility in document handling."

    # feature loop
    - title: "Native signature customization"
      content: "For certain file types, tailor signature placement with built-in document features, such as adding watermarks to Word files or customized stamps to PDFs, enhancing the uniqueness of your documents."
      
  code_samples:
    # code sample loop
    - title: "Implement text signatures in documents"
      content: |
        Learn how to embed text signatures into business documents to optimize processes.
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // Choose the document to be signed
        const signature = new signatureLib.Signature('input.xlsx');

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


############################# More Operations #####################
more_operations:
    enable: true
    title: "Comprehensive signature management features"
    exclude: "text"
    description: "Our platform offers full CRUD operations and advanced features for the management of seven distinct signature types, allowing you to manage your document signatures with precision and ease."
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
    title: "Apply text signatures across various formats"
    exclude: "XLSX"
    description: "Leverage the capabilities of Node.js via Java API to integrate text-based signatures into a wide range of Office formats. Control the flow of information at every stage of your document lifecycle by adding highly customizable text marks."
    items: 
          
        # format loop 1
        - name: "PDF text signatures"
          format: "PDF"
          link: "/signature/nodejs-java/text/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "DOCX text signatures"
          format: "DOCX"
          link: "/signature/nodejs-java/text/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "JPEG text signatures"
          format: "JPEG"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "JPEG Image"
          
        # format loop 4
        - name: "PPTX text signatures"
          format: "PPTX"
          link: "/signature/nodejs-java/text/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "XLSX text signatures"
          format: "XLSX"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---