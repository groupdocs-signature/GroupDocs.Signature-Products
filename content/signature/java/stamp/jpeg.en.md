



---
############################# Static ############################
layout: "format"
date:  2024-10-03T08:55:47
draft: false
lang: en
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Add stamps to JPEG using Java"
head_description: "Leverage GroupDocs.Signature and Java to create custom stamps and place them on any page within JPEG documents."

############################# Header ############################
title: "Add custom stamps to JPEG" 
description: "Design and apply round or square stamps to any section of your documents using GroupDocs.Signature for Java. Our solution offers extensive customization options to meet all your business needs."
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
    title: "About GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) is a robust tool that allows you to add various stamp signatures to documents. It supports over 60 different file formats, including PDFs, Word, Excel, images, and ZIP files. You can apply text, image, barcode, metadata, digital certificate, and stamp signatures. In addition to adding signatures, you can search for, verify, modify, and remove them.

############################# Steps ############################
steps:
    enable: true
    title: "Steps for adding stamps to JPEG via Java"
    content: |
      [GroupDocs.Signature](/signature/java/) provides a stamp constructor that can be highly beneficial for Java applications. Utilize it to create well-customized stamps for your document pages.
      
      1. Provide the JPEG document to be stamped.
      2. Use StampSignOptions to configure all necessary parameters.
      3. Add as many lines as needed.
      4. Apply the stamp and save the document.
   
    code:
      platform: "java"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/signature_all.pdf"
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
        // Use the document path with the Signature object
        Signature signature = new Signature("input.jpeg");

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
        SignResult result = signature.sign("output.jpeg", options);
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "Protect your document content with signatures"
  description: "The GroupDocs.Signature for Java library is designed for signing and managing signatures across popular file formats. Effortlessly add, modify, verify, or remove stamps and other types of signatures."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Stamp Signatures with GroupDocs.Signature"
  features:
    # feature loop
    - title: "Sign your documents"
      content: "Apply customizable signatures to any part of your document. Choose from various signature types, including text, images, barcodes, QR codes, and stamps. Additionally, hidden metadata can be added or modified to enhance document security."

    # feature loop
    - title: "Search and validate signatures"
      content: "Once a document is signed, use our verification tools to ensure that the signature content is valid. Search for and retrieve a list of all signatures for further processing."

    # feature loop
    - title: "Update signatures as needed"
      content: "Easily modify a wide range of signatures applied to a document. Update properties such as size, color, position, content, and more."

    # feature loop
    - title: "Remove signatures"
      content: "Need to remove signatures from a document? Our API fully supports signature deletion, making it easy to manage your documents effectively."
      
  code_samples:
    # code sample loop
    - title: "Add custom stamps to documents using special signatures"
      content: |
        Learn how to generate and add custom stamps with important textual information to your documents.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        // Provide the document to be stamped
        Signature signature = new Signature("input.jpeg");

        // Instantiate the stamp options object
        StampSignOptions options = new StampSignOptions();

        // Set the size and position on the page
        options.setHeight(300);
        options.setWidth(300);
        options.setVerticalAlignment(VerticalAlignment.Bottom);
        options.setHorizontalAlignment(HorizontalAlignment.Right);
        options.setAllPages(true);

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
        options.getOuterLines().add(outerLine1);

        // Add one or more inner square lines
        StampLine innerLine1 = new StampLine();
        innerLine1.setText("Company #1");
        innerLine1.setTextColor(Color.RED);
        SignatureFont signFont1 = new SignatureFont();
        signFont1.setSize(20);
        signFont1.setBold(true);
        innerLine1.setFont(signFont1);
        innerLine1.setHeight(40);
        options.getInnerLines().add(innerLine1);

        // Save the stamped document
        SignResult result = signature.sign("output.jpeg", options);
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
    title: "Explore our core features"
    exclude: "stamp"
    description: "Utilize a wide range of options for adding, managing, and deleting signatures."
    items: 
          
        # operation loop 1
        - name: "Electronic signatures"
          operation: "esign"
          link: "/signature/java/esign/jpeg/"
          description: "Add various types of signatures to supported file formats"

        # operation loop 2
        - name: "Add text to documents"
          operation: "text"
          link: "/signature/java/text/jpeg/"
          description: "Enhance document content with customizable text signatures"

        # operation loop 3
        - name: "Image signatures"
          operation: "image"
          link: "/signature/java/image/jpeg/"
          description: "Place any image at any position within a document"

        # operation loop 4
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/signature/java/barcode/jpeg/"
          description: "Create and insert various barcodes into supported documents"

        # operation loop 5
        - name: "Generate QR codes"
          operation: "qrcode"
          link: "/signature/java/qrcode/jpeg/"
          description: "Generate and apply two-dimensional barcodes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "Secure business documents using digital certificates"

        # operation loop 7
        - name: "Stamp signatures"
          operation: "stamp"
          link: "/signature/java/stamp/jpeg/"
          description: "Use the Stamp Constructor to create custom round or square stamps"
          
        # operation loop 8
        - name: "Search signatures"
          operation: "search"
          link: "/signature/java/search/pdf/"
          description: "Locate any previously added signatures within a document"
          
        # operation loop 9
        - name: "Signature verification"
          operation: "verify"
          link: "/signature/java/verify/pdf/"
          description: "Verify the authenticity of signatures after they have been applied"
          
        # operation loop 10
        - name: "Modify signatures"
          operation: "modify"
          link: "/signature/java/modify/pdf/"
          description: "Easily edit a variety of signatures within a document"
          
        # operation loop 11
        - name: "Delete signatures"
          operation: "delete"
          link: "/signature/java/delete/pdf/"
          description: "Remove a wide range of previously applied signatures"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Add stamps across multiple file formats"
    exclude: "JPEG"
    description: "The GroupDocs.Signature API supports stamping documents in over 60 formats. Place stamps on any page or area to improve document management and customization."
    items: 
          
        # format loop 1
        - name: "Stamp PDF"
          format: "PDF"
          link: "/signature/java/stamp/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Stamp DOCX"
          format: "DOCX"
          link: "/signature/java/stamp/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Stamp JPEG"
          format: "JPEG"
          link: "/signature/java/stamp/jpeg/"
          description: "JPEG Image"
          
        # format loop 4
        - name: "Stamp PPTX"
          format: "PPTX"
          link: "/signature/java/stamp/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "Stamp XLSX"
          format: "XLSX"
          link: "/signature/java/stamp/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---