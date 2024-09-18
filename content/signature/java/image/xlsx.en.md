



---
############################# Static ############################
layout: "format"
date:  2024-09-18T11:51:08
draft: false
lang: en
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Adding Image signatures to XLSX file with Java"
head_description: "Put image signature on XLSX file for Java using a few lines of code. Use GroupDocs.Signature for Java API to add images."

############################# Header ############################
title: "Sign XLSX files with image signatures" 
description: "Use GroupDocs.Signature for Java to insert images into various office document formats, including PDFs, Word, Excel, and image files. An image with a boss's signature can add an impressive touch!"
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download for free"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Discover GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) offers the ability to add image signatures to any page and position within business documents. Streamline your workflows by adding images to PDFs, Word documents, Excel spreadsheets, PowerPoint presentations, and popular image formats.

############################# Steps ############################
steps:
    enable: true
    title: "Steps for adding an image to any place of a XLSX via Java"
    content: |
      [GroupDocs.Signature](/signature/java/) enhances Java applications with the capability to add signatures to any page of XLSX documents precisely. Easily boost your product's functionality by integrating our library.
      
      1. Create an instance of Signature with the XLSX document.
      2. Use ImageSignOptions to specify the signature image.
      3. Place the image on any location of any page.
      4. Save the signed document to a new location.
   
    code:
      platform: "java"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/signature_all.pdf"
      result_title: "Sample signatures"
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
        // Instantiate Signature with the document path
        Signature signature = new Signature("input.xlsx");

        // Create ImageSignOptions using an image for the signature
        ImageSignOptions options = new ImageSignOptions("boss_signature.jpg");

        // Position the image in the top left corner of all pages
        options.setAllPages(true);
        options.setLeft(100);
        options.setTop(100);

        // Save the signed document
        SignResult result = signature.sign("output.xlsx", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Comprehensive document signing solution"
  description: "Our API supports a range of signing features, allowing you to add, modify, delete, search, and verify multiple signature types, including image signatures."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Image signing"
  features:
    # feature loop
    - title: "Insert images into office documents"
      content: "Effortlessly place image signatures in any position on any page of a document. Enrich your content with text, images, barcodes, metadata, and digital certificates."

    # feature loop
    - title: "Signature search and verification"
      content: "Easily verify the validity of signatures in signed documents. Retrieve a list of all signatures within a document and check detailed information about each one."

    # feature loop
    - title: "Modify signatures"
      content: "Update the content, appearance, size, or position of any signature previously added to a document. Our API makes modifying signatures simple and efficient."

    # feature loop
    - title: "Remove unnecessary signatures"
      content: "Our API supports full CRUD operations for most signature types. You can easily remove signatures from nearly all supported document types when necessary."
      
  code_samples:
    # code sample loop
    - title: "Enhance document content with image signatures"
      content: |
        Learn how to append images to business documents to provide additional information.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        // Select a document to be signed
        Signature signature = new Signature("input.xlsx");

        // Create image options with the path to the image
        ImageSignOptions options = new ImageSignOptions("organization_seal.jpg");

        // Set the size of the image signature
        options.setWidth(100);
        options.setHeight(100);

        // Place the image in the bottom right corner
        options.setVerticalAlignment(VerticalAlignment.Bottom);
        options.setHorizontalAlignment(HorizontalAlignment.Right);

        // Apply padding from the page corners if necessary
        Padding padding = new Padding();
        padding.setRight(120);
        padding.setBottom(120);
        options.setMargin(padding);

        // Add a custom border to the image if desired
        Border border = new Border();
        border.setColor(Color.GREEN);
        border.setDashStyle(DashStyle.DashLongDashDot);
        border.setWeight(5);
        border.setVisible(true);
        options.setBorder(border);

        // Rotate the signature for better alignment
        options.setRotationAngle(45);

        // Save the updated document to any location
        SignResult result = signature.sign("output.xlsx", options);
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
    title: "Take a look at our leading features"
    exclude: "image"
    description: "We are pleased to present a variety of signature tools and operations "
    items: 
          
        # operation loop 1
        - name: "Electronic signatures"
          operation: "esign"
          link: "/signature/java/esign/xlsx/"
          description: "Add various types of signatures to supported file formats"

        # operation loop 2
        - name: "Add text to documents"
          operation: "text"
          link: "/signature/java/text/xlsx/"
          description: "Enhance document content with customizable text signatures"

        # operation loop 3
        - name: "Image signatures"
          operation: "image"
          link: "/signature/java/image/xlsx/"
          description: "Place any image at any position within a document"

        # operation loop 4
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/signature/java/barcode/xlsx/"
          description: "Create and insert various barcodes into supported documents"

        # operation loop 5
        - name: "Generate QR codes"
          operation: "qrcode"
          link: "/signature/java/qrcode/xlsx/"
          description: "Generate and apply two-dimensional barcodes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/java/digital/xlsx/"
          description: "Secure business documents using digital certificates"

        # operation loop 7
        - name: "Stamp signatures"
          operation: "stamp"
          link: "/signature/java/stamp/xlsx/"
          description: "Use the Stamp Constructor to create custom round or square stamps"
          
        # operation loop 8
        - name: "Search signatures"
          operation: "search"
          link: "/signature/java/search/xlsx/"
          description: "Locate any previously added signatures within a document"
          
        # operation loop 9
        - name: "Signature verification"
          operation: "verify"
          link: "/signature/java/verify/xlsx/"
          description: "Verify the authenticity of signatures after they have been applied"
          
        # operation loop 10
        - name: "Modify signatures"
          operation: "modify"
          link: "/signature/java/modify/xlsx/"
          description: "Easily edit a variety of signatures within a document"
          
        # operation loop 11
        - name: "Delete signatures"
          operation: "delete"
          link: "/signature/java/delete/xlsx/"
          description: "Remove a wide range of previously applied signatures"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Add images to other file formats"
    exclude: "XLSX"
    description: "With the Java API, you can insert supported image formats into various documents. Easily resize, choose position, and add image signatures to your documents."
    items: 
          
        # format loop 1
        - name: "Sign PDF with image"
          format: "PDF"
          link: "/signature/java/image/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Sign DOCX with image"
          format: "DOCX"
          link: "/signature/java/image/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Sign JPEG with image"
          format: "JPEG"
          link: "/signature/java/image/jpeg/"
          description: "JPEG Image"
          
        # format loop 4
        - name: "Sign PPTX with image"
          format: "PPTX"
          link: "/signature/java/image/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "Sign XLSX with image"
          format: "XLSX"
          link: "/signature/java/image/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---