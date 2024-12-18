



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:38
draft: false
lang: en
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Modify PDF signatures with Java applications"
head_description: "The Java signature processing API allows you to modify signatures in PDF files, including PDF, Word, Excel, Presentations, and Images."

############################# Header ############################
title: "Modify PDF signatures" 
description: "Easily modify a wide variety of electronic signatures using GroupDocs.Signature for Java across popular formats like PDF, Word, Excel, Presentations, and Images."
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
       [GroupDocs.Signature for Java](/signature/java/) not only allows you to sign documents but also provides the ability to modify existing signatures. Easily update signatures in widely used formats such as PDF, Word, Excel, and Presentations.

############################# Steps ############################
steps:
    enable: true
    title: "Steps for editing text signatures in PDF using Java"
    content: |
      [GroupDocs.Signature](/signature/java/) allows Java developers to update the content of text signatures previously added to PDF files. Enhance Java applications with robust capabilities.
      
      1. Add the PDF file to the Signature instance.
      2. Retrieve a list of all signatures in the document.
      3. Update the content of any identified signature.
      4. Analyze the results of the modification.
   
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
        // Instantiate a Signature object with the document path
        Signature signature = new Signature("input.pdf");

        // Search for any text signatures within the document
        TextSearchOptions options = new TextSearchOptions();
        List<TextSignature> signatures = signature.search(TextSignature.class, options);

        if (signatures.size() > 0) {
            // Alter the text of the first detected signature
            TextSignature textSignature = signatures.get(0);
            textSignature.setText("New Text");
            boolean result = signature.update('output.pdf', textSignature);

            // Validate the outcome of the modification
            if (result) {
                System.out.print("\nSignature was updated successfully.");
            }
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Signature management for documents"
  description: "GroupDocs.Signature for Java enables you to add, modify, search, verify, and delete signatures across all major industrial file formats."
  image: "/img/signature/features_modify.webp" # 500x500 px
  image_description: "Signature modification"
  features:
    # feature loop
    - title: "Document signatures"
      content: "Our product primarily focuses on signing documents with text, image, barcode, or stamp signatures. You can place them on any page and position. Add or modify hidden metadata, such as EXIF data in images, and protect document content from unauthorized changes using digital certificates."

    # feature loop
    - title: "Signature search and verification"
      content: "Ensure that signatures meet your requirements by verifying signed documents. You can retrieve a complete list of signatures within a document through the search functionality."

    # feature loop
    - title: "Modify existing signatures"
      content: "Modifying previously added signatures is a common task. Use the modification process to update the content, appearance, position, and other properties of a signature."

    # feature loop
    - title: "Signature deletion"
      content: "Our solution fully supports all operations related to signatures. Removing various types of signatures from a document is a simple process."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Modify barcode signatures"
      content: |
        This example elucidates the process of modifying barcode signatures within a document.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Utilize a document that contains barcode signatures
          final Signature signature = new Signature("input.pdf");

          // Search for existing barcode signatures
          BarcodeSearchOptions options = new BarcodeSearchOptions();
          List<BarcodeSignature> signatures = signature.search(BarcodeSignature.class, options);

          if (signatures.size() > 0)
          {
              // Adjust the position of the first barcode and save the updated document
              BarcodeSignature barcodeSignature = signatures.get(0);
              barcodeSignature.setLeft(100);
              barcodeSignature.setTop(100);
              boolean result = signature.update("output.pdf", barcodeSignature);

              // Confirm the result of the modification
              if (result)
              {
                    System.out.print("\nBarcode was updated successfully.");
              }
          }
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
    title: "Investigate our feature portfolio"
    exclude: "modify"
    description: "We proudly support a wide variety of signature formats and operational tools"
    items: 
          
        # operation loop 1
        - name: "Electronic signatures"
          operation: "esign"
          link: "/signature/java/esign/pdf/"
          description: "Add various types of signatures to supported file formats"

        # operation loop 2
        - name: "Add text to documents"
          operation: "text"
          link: "/signature/java/text/pdf/"
          description: "Enhance document content with customizable text signatures"

        # operation loop 3
        - name: "Image signatures"
          operation: "image"
          link: "/signature/java/image/pdf/"
          description: "Place any image at any position within a document"

        # operation loop 4
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/signature/java/barcode/pdf/"
          description: "Create and insert various barcodes into supported documents"

        # operation loop 5
        - name: "Generate QR codes"
          operation: "qrcode"
          link: "/signature/java/qrcode/pdf/"
          description: "Generate and QR Codes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "Secure business and sign documents with digital certificates"

        # operation loop 7
        - name: "Stamp signatures"
          operation: "stamp"
          link: "/signature/java/stamp/pdf/"
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
    title: "Modify signatures in various file formats"
    exclude: "PDF"
    description: "Document formats signed using our API for Java can be modified. Retrieve a list of signatures from a document and update any accessible properties."
    items: 
          
        # format loop 1
        - name: "Modify PDF signatures"
          format: "PDF"
          link: "/signature/java/modify/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Edit DOCX signatures"
          format: "DOCX"
          link: "/signature/java/modify/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Edit PPTX signatures"
          format: "PPTX"
          link: "/signature/java/modify/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Modify XLSX signatures"
          format: "XLSX"
          link: "/signature/java/modify/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---