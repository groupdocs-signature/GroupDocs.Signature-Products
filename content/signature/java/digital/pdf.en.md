



---
############################# Static ############################
layout: "format"
date:  2024-09-06T10:45:36
draft: false
lang: en
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Secure PDF against Changes Using Java Applications"
head_description: "Use Java applications with GroupDocs.Signature to protect PDF documents with digital certificates."

############################# Header ############################
title: "Protect PDF with Digital Certificates via Java" 
description: "Safeguard the content of your business documents by sealing them with digital certificates using the features of GroupDocs.Signature for Java. We provide multiple ways to mark and secure your documents."
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
       [GroupDocs.Signature for Java](/signature/java/) is a comprehensive signing solution that supports various types of document processing. You can add text, images, digital certificates, and stamps to files in 60+ formats, including PDF, MS Office, images, ZIP files, and other popular business formats. Additionally, signed documents can be searched, verified, modified, or deleted automatically in a convenient way.

############################# Steps ############################
steps:
    enable: true
    title: "Steps for Protecting PDF Files with Digital Certificates in Java"
    content: |
      [GroupDocs.Signature](/signature/java/) allows Java developers to prevent changes in PDF documents using digital signatures. Empower your business applications with the ability to secure important data.
      
      1. Pass the PDF document to the Signature class constructor.
      2. Use a digital certificate and its password to protect the document.
      3. Optionally, add a visual representation of the digital signature on the document pages.
      4. Sign the document to prevent any future changes.
   
    code:
      platform: "java"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/signature_all.pdf"
      result_title: "Download signatures"
      install:
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
        // Use Signature with the document for digital signing
        Signature signature = new Signature("input.pdf");

        // Provide a digital certificate and password
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // Set up visual representation if needed
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);

        // Protect the document with a digital certificate
        SignResult result = signature.sign("output.pdf", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Enhance or Protect Document Content with Signatures"
  description: "The GroupDocs.Signature for Java library is capable of signing all popular file formats. Add, modify, verify, or delete various types of signatures automatically to streamline your business processes."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Features of GroupDocs.Signature"
  features:
    # feature loop
    - title: "Add Signatures to Documents"
      content: "Text, Image, Barcode, QR-Code, or Stamp signatures can be precisely added to any page of any supported document. Hidden metadata like EXIF can be added or edited in images and most file types. Protect document content from unauthorized changes using digital signatures."

    # feature loop
    - title: "Signature Search and Verification"
      content: "Documents can be processed in various ways after signing. Verify signed documents to ensure they have been processed properly. If you need more control, retrieve a list of all signatures through search."

    # feature loop
    - title: "Edit Signatures"
      content: "Most types of signatures support further modification. You are free to correct text, change position, color, size, and more."

    # feature loop
    - title: "Remove Unnecessary Signatures"
      content: "Our solution supports full CRUD operations for signatures. Many types of signatures, including digital certificates, can be deleted from a document when necessary."
      
  code_samples:
    # code sample loop
    - title: "Protect Documents with Digital Signatures"
      content: |
        Learn how to secure a document from changes using digital signatures.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        // Provide a document for signing
        Signature signature = new Signature("input.pdf");

        // Use a valid digital certificate with a password
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // Specify additional text data
        options.setReason("Security issue");
        options.setContact("John Smith");
        options.setLocation("Office D.W.");

        // Use an image and other options for visual representation
        options.setImageFilePath("image.png");

        options.setAllPages(true);
        options.setVerticalAlignment(VerticalAlignment.Bottom);
        options.setHorizontalAlignment(HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        Padding padding = new Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);

        // Save the protected document to a different location
        SignResult result = signature.sign("output.pdf", options);
        ```
        {{< /landing/code >}}


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
    title: "Examine Our Comprehensive Feature Set"
    exclude: "digital"
    description: "We take pride in the extensive functionality and signature support our platform offers"
    items: 
          
        # operation loop 1
        - name: "Electronic Signatures"
          operation: "esign"
          link: "/signature/java/esign/pdf/"
          description: "Add various types of signatures to supported file formats."

        # operation loop 2
        - name: "Add Text to Documents"
          operation: "text"
          link: "/signature/java/text/pdf/"
          description: "Enhance document content with customizable text signatures."

        # operation loop 3
        - name: "Image Signatures"
          operation: "image"
          link: "/signature/java/image/pdf/"
          description: "Place any image at any position within a document."

        # operation loop 4
        - name: "Generate Barcodes"
          operation: "barcode"
          link: "/signature/java/barcode/pdf/"
          description: "Create and insert various barcodes into supported documents."

        # operation loop 5
        - name: "Generate QR Codes"
          operation: "qrcode"
          link: "/signature/java/qrcode/pdf/"
          description: "Generate and apply two-dimensional barcodes, including QR codes, for document signing."
          
        # operation loop 6
        - name: "Digital Certificates"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "Secure business documents using digital certificates."

        # operation loop 7
        - name: "Stamp Signatures"
          operation: "stamp"
          link: "/signature/java/stamp/pdf/"
          description: "Use the Stamp Constructor to create custom round or square stamps."
          
        # operation loop 8
        - name: "Search Signatures"
          operation: "search"
          link: "/signature/java/search/pdf/"
          description: "Locate any previously added signatures within a document."
          
        # operation loop 9
        - name: "Signature Verification"
          operation: "verify"
          link: "/signature/java/verify/pdf/"
          description: "Verify the authenticity of signatures after they have been applied."
          
        # operation loop 10
        - name: "Modify Signatures"
          operation: "modify"
          link: "/signature/java/modify/pdf/"
          description: "Easily edit a variety of signatures within a document."
          
        # operation loop 11
        - name: "Delete Signatures"
          operation: "delete"
          link: "/signature/java/delete/pdf/"
          description: "Remove a wide range of previously applied signatures."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Sign Documents in Other Formats"
    exclude: "PDF"
    description: "The Java API allows you to process more than 60 formats. Create and add various signatures to any page, seal content with digital certificates, and manage and edit existing signatures within the document."
    items: 
          
        # format loop 1
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/signature/java/digital/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Watermark JPEG"
          format: "JPEG"
          link: "/signature/java/digital/jpeg/"
          description: "JPEG Image"
          
        # format loop 3
        - name: "Watermark PDF"
          format: "PDF"
          link: "/signature/java/digital/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 4
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/signature/java/digital/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/signature/java/digital/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---