



---
############################# Static ############################
layout: "format"
date:  2024-10-08T10:48:33
draft: false
lang: en
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Create XLSX text signatures with Java"
head_description: "Leverage the Java API to insert text signatures into XLSX files. Seamlessly process popular document formats including PDF, Word, Excel, Presentations, Images, and ZIP."

############################# Header ############################
title: "Create text signatures for XLSX" 
description: "Easily add custom text signatures to your business documents using GroupDocs.Signature for Java. Streamline organizational workflows with signature customization options."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Start for free"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "About the GroupDocs.Signature for Java solution"
    link: "/signature/java/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) offers flexible and customizable text signatures to simplify your document management tasks. Configure the content and design of text signatures and apply them to any page, enhancing your organization’s document workflow with ease.

############################# Steps ############################
steps:
    enable: true
    title: "Steps for adding text signatures to XLSX using Java"
    content: |
      [GroupDocs.Signature](/signature/java/) can be integrated into Java applications to add text signatures to XLSX documents. Developers can quickly enhance their products' functionality by using our solutions.
      
      1. Use the XLSX document as a parameter for the Signature class constructor.
      2. Instantiate TextSignOptions with the appropriate text.
      3. Configure the visual options for the signature.
      4. Add the text signature to any page(s) of the document.
   
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
        // Pass the document path to the Signature constructor
        Signature signature = new Signature("input.xlsx");

        // Instantiate TextSignOptions with the signature text
        TextSignOptions options = new TextSignOptions("Approved");
        
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
  title: "Manage document text signatures"
  description: "With GroupDocs.Signature for Java, you can streamline your company’s document workflow by adding text signatures to popular file formats. Easily configure the appearance and content of signatures."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "Key features of GroupDocs.Signature"
  features:
    # feature loop
    - title: "Document signatures"
      content: "Apply text, image, barcode, QR code, or stamp signatures to any page of supported documents. Leverage metadata to embed hidden content and secure your documents with digital certificates."

    # feature loop
    - title: "Signature search and verification"
      content: "Ensure the integrity of your signed documents with our signature verification tool. You can also retrieve and search all the signatures embedded within a document."

    # feature loop
    - title: "Modify or remove signatures"
      content: "Modify the content, position, and appearance of previously added signatures, or remove them entirely from the document."

    # feature loop
    - title: "Native text signatures"
      content: "Add document-specific text signatures, such as stickers in PDFs or watermarks in Word documents, for enhanced customization."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Mark documents with text signatures"
      content: |
        Learn how to append textual information to business documents to improve business processes.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Select a document to be signed
          Signature signature = new Signature("input.xlsx");

          // Create text options with the desired text
          TextSignOptions options = new TextSignOptions("Rescheduled to 03/04/2025");

          // Specify the signature's size and position on the page
          options.setLeft(100);
          options.setTop(180);
          options.setWidth(230);
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
          border.setColor(Color.RED);
          border.setDashStyle(DashStyle.Dash);
          border.setTransparency(0.5);
          border.setVisible(true);
          border.setWeight(2);
          options.setBorder(border);

          // Background customization is also available
          Background background = new Background();
          background.setColor(Color.YELLOW);
          background.setTransparency(0.8);
          options.setBackground(background);

          // Text can be saved as an image for compatibility
          options.setSignatureImplementation(TextSignatureImplementation.Image);

          // Save the document with the added text
          SignResult result = signature.sign("output.xlsx", options);
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
            link: "/examples/signature/formats/signature_text.xlsx"
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
    title: "Key features and signature options"
    exclude: "text"
    description: "Our solution supports full CRUD operations and more for seven different types of signatures."
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
    title: "Add text signatures to various file formats"
    exclude: "XLSX"
    description: "Utilize the Java API to insert textual signatures into Office documents, ensuring complete control over the content at every stage of the document's lifecycle."
    items: 
          
        # format loop 1
        - name: "PDF text signatures"
          format: "PDF"
          link: "/signature/java/text/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "DOCX text signatures"
          format: "DOCX"
          link: "/signature/java/text/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "JPEG text signatures"
          format: "JPEG"
          link: "/signature/java/text/jpeg/"
          description: "JPEG Image"
          
        # format loop 4
        - name: "PPTX text signatures"
          format: "PPTX"
          link: "/signature/java/text/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "XLSX text signatures"
          format: "XLSX"
          link: "/signature/java/text/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---