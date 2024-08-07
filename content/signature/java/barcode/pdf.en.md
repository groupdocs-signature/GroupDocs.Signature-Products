



---
############################# Static ############################
layout: "format"
date:  2024-08-07T18:32:07
draft: false
lang: en
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Add Metadata to PDF Files in Java Applications"
head_description: "Java metadata processing API to add metadata information to PDF files. Work with metadata standards XMP, EXIF, IPTC, ID3 etc."

############################# Header ############################
title: "Adding Metadata To PDF In Java" 
description: "Add custom metadata properties to a wide range of business documents, images, audio & video file formats using GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download Free Trial"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "About GroupDocs.Signature for Java API"
    link: "/signature/java/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) is an advanced metadata fields management and manipulation solution to easily view, update, remove, find, compare, exchange and export metadata information from images and document formats without using any external software. Add metadata details to Word documents, Excel spreadsheets, PowerPoint presentations, Outlook emails, OneNote, Visio, Project, PDF, AutoCAD, ZIp, Audio and Video file formats along with the support for working with many other metadata processing features.

############################# Steps ############################
steps:
    enable: true
    title: "Steps to Generate and Add a Barcode to PDF Documents"
    content: |
      [GroupDocs.Signature](/signature/java/) can generate barcodes in various popular formats and place them on PDF pages. With support for over 60 barcode types, Java applications can easily be enhanced with barcode signing capabilities by incorporating our library.
      
      1. Provide the PDF file or stream to be processed.
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
        Signature signature = new Signature("input.pdf");

        // Use BarcodeSignOptions to add a barcode to the document
        BarcodeSignOptions options = new BarcodeSignOptions("Business data");

        // Set up the barcode type and other properties
        options.setEncodeType(BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);

        // Save the signed file
        signature.sign("output.pdf", options);

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
    - title: "How to Customize a Barcode Signature"
      content: |
        This example demonstrates how to place a customized barcode on PDF document pages.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        // Provide the document to be signed
        Signature signature = new Signature("input.pdf");

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
        SignResult signResult = signature.sign("output.pdf", signOptions);
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
    title: "Adding Metadata Properties To Other File Formats"
    exclude: "PDF"
    description: "Multi format documents and images metadata addition API for Java. Retrieve metadata of some of the popular file formats as stated below."
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