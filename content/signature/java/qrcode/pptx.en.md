



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:19
draft: false
lang: en
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Create QR code for PPTX with Java"
head_description: "The GroupDocs.Signature API enables the generation of QR codes for PPTX files. Create QR codes from your content and place them on any page."

############################# Header ############################
title: "Create QR codes for PPTX" 
description: "Easily create 2D barcodes with text and numeric data and place them on any page of various documents using GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Free trial"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Learn more about GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) offers a wide range of features to generate and embed various types of signatures in all major document formats. It supports PDFs, Word documents, Excel spreadsheets, PowerPoint presentations, and images. Enhance your documents with Text, Image, Barcode, QR Code, Metadata, Digital, and Stamp signatures.

############################# Steps ############################
steps:
    enable: true
    title: "Steps to generate and place a QR code at any location in a PPTX"
    content: |
      [GroupDocs.Signature](/signature/java/) can generate QR codes in many popular formats and place them on PPTX pages. Over 10 QR code types are supported and can be quickly integrated into Java applications. Use our product to sign documents with generated QR codes.
      
      1. Get the PPTX file or stream to be signed with a QR code.
      2. Provide the text for QrCodeSignOptions.
      3. Customize visual options such as color, position, size, etc.
      4. Save the file with the QR code.
   
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
        // Pass the document to a new Signature instance
        Signature signature = new Signature("input.pptx");

        // Use QrCodeSignOptions to add a QR code to the document
        QrCodeSignOptions options = new QrCodeSignOptions("Text Content");

        // Specify the signature type and position on the page
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(50);
        options.setTop(150);

        // Save the file with the added QR code
        signature.sign("output.pptx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Add signatures to your documents"
  description: "The GroupDocs.Signature for Java API supports signing all popular file formats. Generate, modify, search, verify, and delete different types of signatures."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Key Features of GroupDocs.Signature"
  features:
    # feature loop
    - title: "Sign documents"
      content: "GroupDocs.Signature supports signing with Text, Image, Barcode, QR Code, and Stamp signatures. Place them on any page of any supported document format. Manage document metadata with metadata signatures, and protect the content from unauthorized changes using digital certificates."

    # feature loop
    - title: "Search and verification"
      content: "Ensure that all signatures in a document are valid with the verification procedure. Retrieve a complete list of signatures in a document using the built-in search feature."

    # feature loop
    - title: "Modify signatures"
      content: "Easily modify signature properties after signing. Adjust content, position, color, size, and other attributes as needed."

    # feature loop
    - title: "Remove signatures"
      content: "Delete unwanted signatures with ease. Various signature types, including digital certificates, can be programmatically removed from documents."
      
  code_samples_ext:
    # code sample ext loop
    - title: "How to customize a generated QR code"
      content: |
        Use this example to learn how to place a new QR code on a PPTX page.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Get the document that needs to be signed and pass it to Signature
          Signature signature = new Signature("input.pptx");

          // Use QR code options to provide text with the required information
          QrCodeSignOptions signOptions = new QrCodeSignOptions("Archived on July 11, 2019");

          // Set the relative position of the QR code on the page
          signOptions.setVerticalAlignment(VerticalAlignment.Top);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Right);

          // Set the signature padding
          Padding padding = new Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Specify the color of the QR code
          signOptions.setForeColor(Color.RED);

          // Define the font options for the message
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Customize the QR code background color and brush
          Background background = new Background();
          background.setColor(Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new LinearGradientBrush(Color.GREEN, Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Add the QR code to the document
          SignResult signResult = signature.sign("output.pptx", signOptions);
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
            link: "/examples/signature/formats/signature_qrcode.pptx"
        links:
          #  loop
          - title: "More examples"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################# Actions ############################

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
    title: "Check out our key offerings"
    exclude: "qrcode"
    description: "We offer a diverse selection of signature features and advanced operations"
    items: 
          
        # operation loop 1
        - name: "Electronic signatures"
          operation: "esign"
          link: "/signature/java/esign/pptx/"
          description: "Add various types of signatures to supported file formats"

        # operation loop 2
        - name: "Add text to documents"
          operation: "text"
          link: "/signature/java/text/pptx/"
          description: "Enhance document content with customizable text signatures"

        # operation loop 3
        - name: "Image signatures"
          operation: "image"
          link: "/signature/java/image/pptx/"
          description: "Place any image at any position within a document"

        # operation loop 4
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/signature/java/barcode/pptx/"
          description: "Create and insert various barcodes into supported documents"

        # operation loop 5
        - name: "Generate QR codes"
          operation: "qrcode"
          link: "/signature/java/qrcode/pptx/"
          description: "Generate and QR Codes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/java/digital/pptx/"
          description: "Secure business and sign documents with digital certificates"

        # operation loop 7
        - name: "Stamp signatures"
          operation: "stamp"
          link: "/signature/java/stamp/pptx/"
          description: "Use the Stamp Constructor to create custom round or square stamps"
          
        # operation loop 8
        - name: "Search signatures"
          operation: "search"
          link: "/signature/java/search/pptx/"
          description: "Locate any previously added signatures within a document"
          
        # operation loop 9
        - name: "Signature verification"
          operation: "verify"
          link: "/signature/java/verify/pptx/"
          description: "Verify the authenticity of signatures after they have been applied"
          
        # operation loop 10
        - name: "Modify signatures"
          operation: "modify"
          link: "/signature/java/modify/pptx/"
          description: "Easily edit a variety of signatures within a document"
          
        # operation loop 11
        - name: "Delete signatures"
          operation: "delete"
          link: "/signature/java/delete/pptx/"
          description: "Remove a wide range of previously applied signatures"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Generate QR codes for additional file formats"
    exclude: "PPTX"
    description: "Enhance all popular file formats with generated QR codes using the Java API. Add 2D barcode data for easy scanning and processing."
    items: 
          
        # format loop 1
        - name: "QR-Code for PDF"
          format: "PDF"
          link: "/signature/java/qrcode/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "QR-Code for DOCX"
          format: "DOCX"
          link: "/signature/java/qrcode/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "QR-Code for JPEG"
          format: "JPEG"
          link: "/signature/java/qrcode/jpeg/"
          description: "JPEG Image"
          
        # format loop 4
        - name: "QR-Code for PPTX"
          format: "PPTX"
          link: "/signature/java/qrcode/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "QR-Code for XLSX"
          format: "XLSX"
          link: "/signature/java/qrcode/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---