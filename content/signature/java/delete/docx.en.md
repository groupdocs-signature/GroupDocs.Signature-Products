



---
############################# Static ############################
layout: "format"
date:  2024-09-12T11:45:41
draft: false
lang: en
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Remove Signatures from DOCX Files Using Java Applications"
head_description: "Enhance your Java applications with GroupDocs.Signature for Java, enabling the removal of previously added signatures from DOCX files."

############################# Header ############################
title: "Remove Signatures from DOCX Files with Java" 
description: "Our solution not only allows you to sign business documents but also provides the capability to locate and remove various types of signatures using GroupDocs.Signature for Java."
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
       [GroupDocs.Signature for Java](/signature/java/) offers a comprehensive signing solution, capable of handling various types of signatures such as text, images, barcodes, digital certificates, and stamps. This tool supports over 60 different file formats, including PDFs, MS Office documents, image files, ZIP archives, and many other commonly used formats. Moreover, once signatures are applied, they can be easily searched, verified, edited, or removed whenever needed.

############################# Steps ############################
steps:
    enable: true
    title: "Steps for Deleting Text Signatures from DOCX using Java"
    content: |
      [GroupDocs.Signature](/signature/java/) makes it easy for Java developers to delete text signatures in DOCX files using their applications by following a few simple steps.
      
      1. Pass the DOCX path to an instance of the Signature class.
      2. Use the Search method to retrieve all text signatures from the document.
      3. Delete one or more of the located text signatures.
      4. Analyze the results of the document processing.
   
    code:
      platform: "java"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/signature_all.pdf"
      result_title: "Sample signatures"
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
        // Pass the document containing the signatures to be deleted to Signature
        Signature signature = new Signature("input.docx");

        // Retrieve the text signatures present in the document
        TextSearchOptions options = new TextSearchOptions();
        List<TextSignature> signatures = signature.search(TextSignature.class, options);

        // Delete the first located text signature
        if(signatures.size() > 0)
        {
            TextSignature textSignature = signatures.get(0);
            boolean result = signature.delete("output.docx", textSignature);

            // Process the result of the deletion
            if(result)
            {
                System.out.print("\nSignature was deleted successfully");
            }
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Enhance Business Processes with Signature Management"
  description: "GroupDocs.Signature for Java is designed for signing and managing business file formats, allowing you to add, modify, verify, or delete signatures as needed."
  image: "/img/signature/features_delete.webp" # 500x500 px
  image_description: "GroupDocs.Signature Capabilities"
  features:
    # feature loop
    - title: "Sign Documents"
      content: "Easily add text, image, barcode, QR code, or stamp signatures to any page of supported documents. Utilize hidden metadata like EXIF in images or secure document content from unauthorized modifications with digital certificates."

    # feature loop
    - title: "Search and Verification"
      content: "Maximize the potential of signed documents by verifying signatures to ensure their validity. You can also retrieve a comprehensive list of all signatures within a document through a simple search."

    # feature loop
    - title: "Modify Signatures"
      content: "Most previously added signatures can be adjusted. You can easily modify text, reposition the signature, or change its color."

    # feature loop
    - title: "Delete Signatures"
      content: "Our solution fully supports CRUD operations for signatures, allowing you to delete various types of signatures from a document as needed."
      
  code_samples:
    # code sample loop
    - title: "Remove All QR-Code Signatures"
      content: |
        Learn how to remove all QR-code signatures embedded within a document.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        // Provide a document that contains QR-code signatures
        Signature signature = new Signature("input.docx");

        // Delete all QR-code signatures
        DeleteResult result = signature.delete("output.docx", SignatureType.QrCode);

        // Process the result of the deletion
        if (result.getSucceeded().size() > 0)
        {
            System.out.print("\nFollowing QR-Code signatures were deleted:");
            int number = 1;
            for (BaseSignature temp : result.getSucceeded())
            {
                System.out.print("Signature #"+number++ +
                ": Type: "+temp.getSignatureType()+" Id:"+temp.getSignatureId()+
                ", Text: "+((QrCodeSignature)temp).getText());
            }
        }
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
    title: "Learn About Our Key Features"
    exclude: "delete"
    description: "Explore the diverse operations and signature methods available with our platform"
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
          description: "Generate and apply two-dimensional barcodes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/java/digital/docx/"
          description: "Secure business documents using digital certificates"

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
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Remove Signatures from Various File Formats"
    exclude: "DOCX"
    description: "Our GroupDocs.Signature for Java solution supports the removal of signatures from over 60 different file formats."
    items: 
          
        # format loop 1
        - name: "Delete PDF signatures"
          format: "PDF"
          link: "/signature/java/delete/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Delete DOCX signatures"
          format: "DOCX"
          link: "/signature/java/delete/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Delete PPTX signatures"
          format: "PPTX"
          link: "/signature/java/delete/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Delete XLSX signatures"
          format: "XLSX"
          link: "/signature/java/delete/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---