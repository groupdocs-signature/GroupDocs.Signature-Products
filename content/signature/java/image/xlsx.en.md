



---
############################# Static ############################
layout: "format"
date:  2024-08-07T20:02:05
draft: false
lang: en
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Add Metadata to XLSX Files in Java Applications"
head_description: "Java metadata processing API to add metadata information to XLSX files. Work with metadata standards XMP, EXIF, IPTC, ID3 etc."

############################# Header ############################
title: "Adding Metadata To XLSX In Java" 
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
    title: "Steps for Adding an Image to Any Page of a XLSX Document via Java"
    content: |
      [GroupDocs.Signature](/signature/java/) enhances Java applications with the capability to add signatures to any page of XLSX documents precisely. Easily boost your product's functionality by integrating our library.
      
      1. Create an instance of Signature with the XLSX document.
      2. Use ImageSignOptions to specify the signature image.
      3. Place the image on any location of any page.
      4. Save the signed document to a new location.
   
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
    - title: "Enhance Document Content with Image Signatures"
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


############################# More Formats #####################
more_formats:
    enable: true
    title: "Adding Metadata Properties To Other File Formats"
    exclude: "XLSX"
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