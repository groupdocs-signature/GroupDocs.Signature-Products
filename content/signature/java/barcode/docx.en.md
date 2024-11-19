



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:24
draft: false
lang: en
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Easily add barcodes to DOCX files with Java"
head_description: "Create and insert barcode signatures into DOCX documents in Java with ease. GroupDocs.Signature enables versatile signature integration for multiple formats."

############################# Header ############################
title: "Generate barcode for DOCX" 
description: "Add barcodes of popular formats to any position in your business documents with GroupDocs.Signature for Java. Our solution provides extensive options to customize barcode signatures."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download for Free"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "About GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) is an advanced signing solution that supports a wide range of signature types. You can sign documents with text, images, barcodes, digital certificates, stamps, and more across 60+ file formats, including PDF, MS Office, images, ZIP files, and other popular business formats. Additionally, signatures in signed documents can be searched, verified, modified, or deleted at any time.

############################# Steps ############################
steps:
    enable: true
    title: "Steps to generate and add a barcode to DOCX file"
    content: |
      [GroupDocs.Signature](/signature/java/) can generate barcodes in various popular formats and place them on DOCX pages. With support for over 60 barcode types, Java applications can easily be enhanced with barcode signing capabilities by incorporating our library.
      
      1. Provide the DOCX file or stream to be processed.
      2. Pass the barcode text to the BarcodeSignOptions instance.
      3. Customize barcode options such as position, size, etc.
      4. Save the file with the newly added barcode.
   
    code:
      platform: "java"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Sample signatures"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-signature</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/signature/java/"
          
      content: |
        ```java {style=abap}
        // Create a new Signature instance with the document path
        Signature signature = new Signature("input.docx");

        // Use BarcodeSignOptions to add a barcode to the document
        BarcodeSignOptions options = new BarcodeSignOptions("Business data");

        // Set up the barcode type and other properties
        options.setEncodeType(BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);

        // Save the signed file
        signature.sign("output.docx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Enhance or protect document content with signatures"
  description: "The GroupDocs.Signature for Java library is designed for signing and further processing popular file formats. Quickly and easily add, modify, verify, or delete various types of signatures."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Features of GroupDocs.Signature"
  features:
    # feature loop
    - title: "Document signing"
      content: "Sign any page of supported documents with text, images, barcodes, QR codes, or stamps. Add hidden metadata like EXIF in images or protect document content from unauthorized changes using digital certificates."

    # feature loop
    - title: "Signature search and verification"
      content: "There’s much more you can do with a signed document. We offer verification of signatures to ensure everything is in order. Additionally, you can retrieve a list of all document signatures through a search."

    # feature loop
    - title: "Modify signatures"
      content: "Most previously added signatures can be modified. Easily correct text, adjust position, or change color."

    # feature loop
    - title: "Delete signatures"
      content: "Our solution supports full CRUD operations for signatures. Many types of signatures can be deleted from a document when necessary."
      
  code_samples_ext:
    # code sample ext loop
    - title: "How to create a barcode signature"
      content: |
        This example demonstrates how to place a customized barcode on DOCX document pages.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Provide the document to be signed
          Signature signature = new Signature("input.docx");

          // Create signature options with the desired text
          BarcodeSignOptions signOptions = new BarcodeSignOptions("Accepted");
          signOptions.setEncodeType(BarcodeTypes.Code39FullASCII);

          // Set the relative barcode position on the page
          signOptions.setVerticalAlignment(VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Left);

          // Set the barcode padding from the page edge
          Padding padding = new Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // Set the color of the bars
          signOptions.setForeColor(Color.RED);

          // Define the message font style
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Arial");
          signOptions.setFont(font);

          // Specify the message position
          signOptions.setCodeTextAlignment(CodeTextAlignment.Above);

          // Sign and save the document
          SignResult signResult = signature.sign("output.docx", signOptions);

          ```
        platform: "java"
        copy_title: "Copy"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-signature</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "click to copy"
          copy_done: "copied"
        top_links:
          #  loop
          - title: "Download result"
            icon: "download"
            link: "/examples/signature/formats/signature_barcode.docx"
        links:
          #  loop
          - title: "More examples"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Ready to get started?"
  description: "Try GroupDocs.Signature features for free or request a license"
  items:
    #  loop
    - title: "Maven download"
      link: "https://releases.groupdocs.com/signature/java/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/signature/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Discover our core capabilities"
    exclude: "barcode"
    description: "We proudly present an extensive variety of supported signatures and functions"
    items: 
          
        # operation loop 1
        - name: "Electronic signatures"
          operation: "esign"
          link: "/signature/java/esign/docx/"
          description: "Add various types of signatures to supported file formats"

        # operation loop 2
        - name: "Add text to documents"
          operation: "text"
          link: "/signature/java/text/docx/"
          description: "Enhance document content with customizable text signatures"

        # operation loop 3
        - name: "Image signatures"
          operation: "image"
          link: "/signature/java/image/docx/"
          description: "Place any image at any position within a document"

        # operation loop 4
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/signature/java/barcode/docx/"
          description: "Create and insert various barcodes into supported documents"

        # operation loop 5
        - name: "Generate QR codes"
          operation: "qrcode"
          link: "/signature/java/qrcode/docx/"
          description: "Generate and QR Codes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/java/digital/docx/"
          description: "Secure business and sign documents with digital certificates"

        # operation loop 7
        - name: "Stamp signatures"
          operation: "stamp"
          link: "/signature/java/stamp/docx/"
          description: "Use the Stamp Constructor to create custom round or square stamps"
          
        # operation loop 8
        - name: "Search signatures"
          operation: "search"
          link: "/signature/java/search/docx/"
          description: "Locate any previously added signatures within a document"
          
        # operation loop 9
        - name: "Signature verification"
          operation: "verify"
          link: "/signature/java/verify/docx/"
          description: "Verify the authenticity of signatures after they have been applied"
          
        # operation loop 10
        - name: "Modify signatures"
          operation: "modify"
          link: "/signature/java/modify/docx/"
          description: "Easily edit a variety of signatures within a document"
          
        # operation loop 11
        - name: "Delete signatures"
          operation: "delete"
          link: "/signature/java/delete/docx/"
          description: "Remove a wide range of previously applied signatures"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Sign documents in other formats"
    exclude: "DOCX"
    description: "Over 60 formats can be signed using our Java API. Apply various signatures to any page or position within the document."
    items: 
          
        # format loop 1
        - name: "Add barcode to PDF"
          format: "PDF"
          link: "/signature/java/barcode/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Add barcode to DOCX"
          format: "DOCX"
          link: "/signature/java/barcode/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Add barcode to JPEG"
          format: "JPEG"
          link: "/signature/java/barcode/jpeg/"
          description: "JPEG Image"
          
        # format loop 4
        - name: "Add barcode to PPTX"
          format: "PPTX"
          link: "/signature/java/barcode/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "Add barcode to XLSX"
          format: "XLSX"
          link: "/signature/java/barcode/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---