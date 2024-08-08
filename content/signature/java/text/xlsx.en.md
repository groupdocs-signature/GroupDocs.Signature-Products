



---
############################# Static ############################
layout: "format"
date:  2024-08-08T16:38:31
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
    title: "Steps for Adding Text Signatures to XLSX Files Using Java"
    content: |
      [GroupDocs.Signature](/signature/java/) can be integrated into Java applications to add text signatures to XLSX documents. Developers can quickly enhance their products' functionality by using our solutions.
      
      1. Use the XLSX document as a parameter for the Signature class constructor.
      2. Instantiate TextSignOptions with the appropriate text.
      3. Configure the visual options for the signature.
      4. Add the text signature to any page(s) of the document.
   
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
        // Pass the document path to the Signature constructor
        Signature signature = new Signature("input.xlsx");

        // Instantiate TextSignOptions with the signature text
        TextSignOptions options = new TextSignOptions("Approved on 03/12/2021");
        
        // Set up text color and font attributes
        options.setForeColor(Color.RED);
        SignatureFont signatureFont = new SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName("Comic Sans MS");
        options.setFont(signatureFont);

        // Append the text signature to the document
        SignResult result = signature.sign("output.xlsx", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Document Metadata Management"
  description: "Our comprehensive API streamlines managing document metadata. Access, edit, and manipulate various document properties for improved organization and searchability."
  image: "/img/signature/features_text.webp" # 500x500 px
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
    - title: "Mark Documents with Text Signatures"
      content: |
        Learn how to append textual information to business documents to improve business processes.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        // Select a document to be signed
        Signature signature = new Signature("input.xlsx");

        // Create text options with the desired text
        TextSignOptions options = new TextSignOptions("Rescheduled to 03/04/2025");

        // Specify the signature's size and position on the page
        options.setLeft(100);
        options.setTop(100);
        options.setWidth(100);
        options.setHeight(30);

        // Signatures support padding from the page corners
        Padding padding = new Padding();
        padding.setBottom(20);
        padding.setRight(20);
        options.setMargin(padding);

        // Text color and font style can be customized
        options.setForeColor(Color.RED);
        SignatureFont signatureFont = new SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName("Comic Sans MS");
        options.setFont(signatureFont);

        // Text signatures can include a border
        Border border = new Border();
        border.setColor(Color.GREEN);
        border.setDashStyle(DashStyle.DashLongDashDot);
        border.setTransparency(0.5);
        border.setVisible(true);
        border.setWeight(2);
        options.setBorder(border);

        // Background customization is also available
        Background background = new Background();
        background.setColor(Color.LIGHT_GRAY);
        background.setTransparency(0.5);
        background.setBrush(new LinearGradientBrush(Color.GREEN, Color.DARK_GRAY, 0));
        options.setBackground(background);

        // Signatures can be rotated on the page
        options.setRotationAngle(45);

        // Text can be saved as an image for compatibility
        options.setSignatureImplementation(TextSignatureImplementation.Image);

        // Save the document with the added text
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