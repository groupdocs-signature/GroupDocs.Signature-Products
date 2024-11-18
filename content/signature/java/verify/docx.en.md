



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:14
draft: false
lang: en
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Verify DOCX e-signatures using Java"
head_description: "GroupDocs.Signature for Java enables the verification of signatures placed in DOCX files. Validate signatures in PDFs, Word documents, Excel sheets, Presentations, Images, or ZIP archives."

############################# Header ############################
title: "e-Signature verification for DOCX" 
description: "Verify all supported e-signatures in PDF, Word, Excel, Presentations, Images, or ZIP files with GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download free version"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Applications of GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) supports full CRUD operations for document signing and more. Sign 60+ document formats, including PDFs, MS Office files, Images, and ZIP archives, with text, image, barcode, digital certificates, metadata, and stamps. Additional operations such as searching, verifying, modifying, or deleting signatures are also available.

############################# Steps ############################
steps:
    enable: true
    title: "Steps for verifying signatures in DOCX using Java"
    content: |
      [GroupDocs.Signature](/signature/java/) can verify the presence of specific signatures in a DOCX document. Java developers can easily empower their applications by adding features provided by our solution.
      
      1. Load the DOCX file into the Signature instance.
      2. Instantiate and configure VerifyOptions to achieve the desired result.
      3. Initiate the verification process.
      4. Review the verification results.
   
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
        // Instantiate a Signature with the document
        Signature signature = new Signature("input.docx");

        // Create TextVerifyOptions to validate signatures containing specific text
        TextVerifyOptions options = new TextVerifyOptions();
        options.setText("signature");
        options.setMatchType(TextMatchType.Contains);

        // Verify the signatures in the document
        VerificationResult result = signature.verify(options);

        // Process the verification results
        if (result.isValid())
        {
            System.out.print("\nDocument was verified successfully!");
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Comprehensive document signing solution"
  description: "GroupDocs.Signature enhances popular office document formats with 7 types of signatures and full CRUD operations, offering robust protection for your document content."
  image: "/img/signature/features_verify.webp" # 500x500 px
  image_description: "Signature verification"
  features:
    # feature loop
    - title: "Sign corporate documents"
      content: "Add professional digital signatures to any document. Our solution supports various types of signatures, including text, images, barcodes, metadata, stamps, and digital certificates."

    # feature loop
    - title: "Signature CRUD operations"
      content: "In many cases, signed documents require further processing. Retrieve a list of all signatures in a document, verify them, modify their properties, or remove them when necessary."

    # feature loop
    - title: "Protect document content"
      content: "Safeguard corporate documents with digital certificates to prevent unauthorized changes. Embed hidden metadata to further protect document content."

    # feature loop
    - title: "Native signatures"
      content: "Utilize document-specific text signatures, such as PDF stamps or Word watermarks, to create tailored, professional documents for corporate use."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Verify barcode signatures"
      content: |
        This example demonstrates how to verify barcode signatures in a document.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Provide the document that contains barcode signatures
          final Signature signature = new Signature("input.docx");

          // Configure options to verify barcodes against specific text
          BarcodeVerifyOptions options = new BarcodeVerifyOptions();
          options.setText("12345");
          options.setMatchType(TextMatchType.StartsWith);

          // Verify the signatures that were applied to the document
          VerificationResult result = signature.verify(options);

          // Display the results of the verification
          if (result.isValid())
          {
              System.out.print("\nDocument was verified successfully!");
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
    title: "Supported operations and signature types"
    exclude: "verify"
    description: "Explore the full range of features and signature operations supported by GroupDocs.Signature."
    items: 
          
        # operation loop 1
        - name: "Electronic signatures"
          operation: "esign"
          link: "/signature/java/esign/docx/"
          description: "Add various types of signatures to supported file formats"

        # operation loop 2
        - name: "Add text to documents"
          operation: "text"
          link: "/signature/java/text/docx/"
          description: "Enhance document content with customizable text signatures"

        # operation loop 3
        - name: "Image signatures"
          operation: "image"
          link: "/signature/java/image/docx/"
          description: "Place any image at any position within a document"

        # operation loop 4
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/signature/java/barcode/docx/"
          description: "Create and insert various barcodes into supported documents"

        # operation loop 5
        - name: "Generate QR codes"
          operation: "qrcode"
          link: "/signature/java/qrcode/docx/"
          description: "Generate and QR Codes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/java/digital/docx/"
          description: "Secure business and sign documents with digital certificates"

        # operation loop 7
        - name: "Stamp signatures"
          operation: "stamp"
          link: "/signature/java/stamp/docx/"
          description: "Use the Stamp Constructor to create custom round or square stamps"
          
        # operation loop 8
        - name: "Search signatures"
          operation: "search"
          link: "/signature/java/search/docx/"
          description: "Locate any previously added signatures within a document"
          
        # operation loop 9
        - name: "Signature verification"
          operation: "verify"
          link: "/signature/java/verify/docx/"
          description: "Verify the authenticity of signatures after they have been applied"
          
        # operation loop 10
        - name: "Modify signatures"
          operation: "modify"
          link: "/signature/java/modify/docx/"
          description: "Easily edit a variety of signatures within a document"
          
        # operation loop 11
        - name: "Delete signatures"
          operation: "delete"
          link: "/signature/java/delete/docx/"
          description: "Remove a wide range of previously applied signatures"
          
############################# More Formats #####################
more_formats:
    enable: true
    title: "Signature verification across file formats"
    exclude: "DOCX"
    description: "GroupDocs.Signature for Java simplifies the process of verifying all signatures in a document. Set custom verification parameters to ensure the integrity of signed documents."
    items: 
          
        # format loop 1
        - name: "Verify PDF signatures"
          format: "PDF"
          link: "/signature/java/verify/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Verify DOCX signatures"
          format: "DOCX"
          link: "/signature/java/verify/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Verify PPTX signatures"
          format: "PPTX"
          link: "/signature/java/verify/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Validate XLSX signatures"
          format: "XLSX"
          link: "/signature/java/verify/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---