



---
############################# Static ############################
layout: "format"
date:  2024-08-08T16:38:30
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
    title: "Steps for Adding Stamp Signatures to PDF Documents via Java"
    content: |
      [GroupDocs.Signature](/signature/java/) provides a stamp constructor that can be highly beneficial for Java applications. Utilize it to create well-customized stamps for your document pages.
      
      1. Provide the PDF document to be stamped.
      2. Use StampSignOptions to configure all necessary parameters.
      3. Add as many lines as needed.
      4. Apply the stamp and save the document.
   
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
        // Use the document path with the Signature object
        Signature signature = new Signature("input.pdf");

        // Instantiate StampSignOptions with the desired signature text
        StampSignOptions options = new StampSignOptions();

        // Add one or more stamp lines
        StampLine outerLine = new StampLine();
        outerLine.setText(" * The Best Company * ");
        outerLine.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(Color.WHITE);
        outerLine.setBackgroundColor(Color.BLUE);
        options.getOuterLines().add(outerLine);

        // Save the stamped document
        SignResult result = signature.sign("output.pdf", options);
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "Document Metadata Management"
  description: "Our comprehensive API streamlines managing document metadata. Access, edit, and manipulate various document properties for improved organization and searchability."
  image: "/img/signature/features_stamp.webp" # 500x500 px
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
    - title: "Add Custom Stamps to Documents using Special Signatures"
      content: |
        Learn how to generate and add custom stamps with important textual information to your documents.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        // Provide the document to be stamped
        Signature signature = new Signature("input.pdf");

        // Instantiate the stamp options object
        StampSignOptions signOptions = new StampSignOptions();

        // Set the size and position on the page
        signOptions.setHeight(300);
        signOptions.setWidth(300);
        signOptions.setVerticalAlignment(VerticalAlignment.Bottom);
        signOptions.setHorizontalAlignment(HorizontalAlignment.Right);
        signOptions.setAllPages(true);

        // Add one or more outer round lines with text
        StampLine outerLine1 = new StampLine();
        outerLine1.setText("* The best choice *");
        outerLine1.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
        SignatureFont signatureFont1 = new SignatureFont();
        signatureFont1.setSize(12);
        signatureFont1.setFamilyName("Arial");
        outerLine1.setFont(signatureFont1);
        outerLine1.setHeight(30);
        outerLine1.setTextBottomIntent(6);
        outerLine1.setTextColor(Color.WHITE);
        outerLine1.setBackgroundColor(Color.BLUE);
        signOptions.getOuterLines().add(outerLine1);

        // Add one or more inner square lines
        StampLine innerLine1 = new StampLine();
        innerLine1.setText("Company #1");
        innerLine1.setTextColor(Color.RED);
        SignatureFont signFont1 = new SignatureFont();
        signFont1.setSize(20);
        signFont1.setBold(true);
        innerLine1.setFont(signFont1);
        innerLine1.setHeight(40);
        signOptions.getInnerLines().add(innerLine1);

        // Save the stamped document
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