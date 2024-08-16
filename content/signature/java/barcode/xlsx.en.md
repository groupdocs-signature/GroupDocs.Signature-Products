



---
############################# Static ############################
layout: "format"
date:  2024-08-16T17:36:45
draft: false
lang: en
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Add Generated Barcodes to XLSX Files Using Java Applications"
head_description: "Utilize Java applications with GroupDocs.Signature to generate and insert barcodes on any page of XLSX documents."

############################# Header ############################
title: "Embed Barcodes in XLSX Pages Using Java" 
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
    title: "Steps to Generate and Add a Barcode to XLSX Documents"
    content: |
      [GroupDocs.Signature](/signature/java/) can generate barcodes in various popular formats and place them on XLSX pages. With support for over 60 barcode types, Java applications can easily be enhanced with barcode signing capabilities by incorporating our library.
      
      1. Provide the XLSX file or stream to be processed.
      2. Pass the barcode text to the BarcodeSignOptions instance.
      3. Customize barcode options such as position, size, etc.
      4. Save the file with the newly added barcode.
   
    code:
      platform: "java"
      copy_title: "Copy"
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
        // Create a new Signature instance with the document path
        Signature signature = new Signature("input.xlsx");

        // Use BarcodeSignOptions to add a barcode to the document
        BarcodeSignOptions options = new BarcodeSignOptions("Business data");

        // Set up the barcode type and other properties
        options.setEncodeType(BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);

        // Save the signed file
        signature.sign("output.xlsx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Enhance or Protect Document Content with Signatures"
  description: "The GroupDocs.Signature for Java library is designed for signing and further processing popular file formats. Quickly and easily add, modify, verify, or delete various types of signatures."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Features of GroupDocs.Signature"
  features:
    # feature loop
    - title: "Document Signing"
      content: "Sign any page of supported documents with text, images, barcodes, QR codes, or stamps. Add hidden metadata like EXIF in images or protect document content from unauthorized changes using digital certificates."

    # feature loop
    - title: "Signature Search and Verification"
      content: "There’s much more you can do with a signed document. We offer verification of signatures to ensure everything is in order. Additionally, you can retrieve a list of all document signatures through a search."

    # feature loop
    - title: "Modify Signatures"
      content: "Most previously added signatures can be modified. Easily correct text, adjust position, or change color."

    # feature loop
    - title: "Delete Signatures"
      content: "Our solution supports full CRUD operations for signatures. Many types of signatures can be deleted from a document when necessary."
      
  code_samples:
    # code sample loop
    - title: "How to Customize a Barcode Signature"
      content: |
        This example demonstrates how to place a customized barcode on XLSX document pages.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        // Provide the document to be signed
        Signature signature = new Signature("input.xlsx");

        // Create signature options with the desired text
        BarcodeSignOptions signOptions = new BarcodeSignOptions("Accepted for review on February 15, 2020");

        // Set the relative barcode position on the page
        signOptions.setVerticalAlignment(VerticalAlignment.Bottom);
        signOptions.setHorizontalAlignment(HorizontalAlignment.Right);

        // Set the barcode padding from the page edge
        Padding padding = new Padding();
        padding.setLeft(20);
        padding.setTop(20);
        signOptions.setMargin(padding);

        // Set the color of the bars
        signOptions.setForeColor(Color.RED);

        // Define the message font style
        SignatureFont font = new SignatureFont();
        font.setSize(12);
        font.setFamilyName("Comic Sans MS");
        signOptions.setFont(font);

        // Specify the message position
        signOptions.setCodeTextAlignment(CodeTextAlignment.Above);

        // Sign and save the document
        SignResult signResult = signature.sign("output.xlsx", signOptions);
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


############################# More Formats #####################
more_formats:
    enable: true
    title: "Sign Documents in Other Formats"
    exclude: "XLSX"
    description: "Over 60 formats can be signed using our Java API. Apply various signatures to any page or position within the document."
    items: 
          
        # format loop 1
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/signature/java//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Watermark JPEG"
          format: "JPEG"
          link: "/signature/java//jpeg/"
          description: "JPEG Image"
          
        # format loop 3
        - name: "Watermark PDF"
          format: "PDF"
          link: "/signature/java//pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 4
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/signature/java//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/signature/java//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---