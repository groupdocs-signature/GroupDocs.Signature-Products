



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:12
draft: false
lang: en
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Search for digital signature  in XLSX by Java"
head_description: "Leverage the GroupDocs.Signature for Java API to search for signatures within XLSX files. Find signatures in PDFs, Word, Excel, Presentations, and Images."

############################# Header ############################
title: "Search for digital signatures in XLSX" 
description: "Retrieve a complete list of e-signatures embedded in PDF, Word, Excel, Presentations, or Image files using GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Free download"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "About GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) offers powerful features for signing documents. It supports adding text, images, barcodes, digital certificates, and stamps to files in 60+ formats, including PDFs, MS Office documents, Images, ZIP files, and other common business formats. In addition, you can search, verify, modify, or delete signatures at any time.

############################# Steps ############################
steps:
    enable: true
    title: "Steps for searching XLSX signatures using Java"
    content: |
      [GroupDocs.Signature](/signature/java/) provides a powerful engine to search for any digital signatures within XLSX files. Java developers can easily enhance their applications with our solution.
      
      1. Provide the XLSX file path for signature search.
      2. Use SearchOptions to refine the search results.
      3. Execute the Search method to obtain the results.
      4. Analyze the list of found signatures.
   
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

        // Create an instance of Signature with the document path
        final Signature signature = new Signature("input.xlsx");

        // Instantiate TextSearchOptions to cover all pages
        TextSearchOptions options = new TextSearchOptions();
        options.setAllPages(true);

        // Search for text signatures within the document
        List<TextSignature> signatures = signature.search(TextSignature.class, options);
        System.out.print("\nSource document contains following text signature(s).");

        // List the found signatures for further analysis
        for (TextSignature textSignature : signatures) {
            System.out.print("Found Text signature at page " + textSignature.getPageNumber() 
                + " with type [" + textSignature.getSignatureImplementation() + "] and 
                text '" + textSignature.getText() + "'.");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Comprehensive document signing solution"
  description: "We are proud to introduce our document signing solution, compatible with all major document formats. Add a wide range of signatures to enhance your documents or secure their content."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "Signature search"
  features:
    # feature loop
    - title: "Sign business documents"
      content: "Insert digital signatures at any position on any page of a document. Use a variety of signature types, such as text, images, barcodes, metadata, stamps, or digital certificates."

    # feature loop
    - title: "Manage signatures"
      content: "After signing, documents may require further processing. Search for all available signatures, and update or delete them whenever necessary."

    # feature loop
    - title: "Protect document content"
      content: "Manage hidden metadata embedded in the document. Add new metadata or remove existing entries. Use corporate digital certificates to safeguard the document’s content from unauthorized alterations."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Search for image signatures"
      content: |
        This example demonstrates how to find an image signature in a specific document.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Pass the source document as a constructor parameter
          final Signature signature = new Signature("input.xlsx");

          // Search for any signatures with a text type
          List<ImageSignature> signatures = signature.search(ImageSignature.class, SignatureType.Image);
          System.out.print("\nSource document contains following image signature(s).");

          // Display the results with the properties of the found signatures
          for (ImageSignature imageSignature : signatures)
          {
              System.out.print("Image signature found at page "+imageSignature.getPageNumber()+
                    " with size "+imageSignature.getSize()+". Created "+imageSignature.getCreatedOn()+
                    ", modified "+imageSignature.getModifiedOn());
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
    title: "Supported operations"
    exclude: "search"
    description: "Our product offers a flexible API for signing documents and managing signatures after signing."
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
          description: "Generate and QR Codes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/java/digital/xlsx/"
          description: "Secure business and sign documents with digital certificates"

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
    title: "Search signatures in various file formats"
    exclude: "XLSX"
    description: "GroupDocs.Signature for Java API enables you to retrieve the list of signatures from any signed file. Extract signatures from popular file formats for further processing."
    items: 
          
        # format loop 1
        - name: "Search signatures in PDF"
          format: "PDF"
          link: "/signature/java/search/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Find signatures in DOCX"
          format: "DOCX"
          link: "/signature/java/search/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Find signatures in PPTX"
          format: "PPTX"
          link: "/signature/java/search/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Search signatures in XLSX"
          format: "XLSX"
          link: "/signature/java/search/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---