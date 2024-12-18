



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:28
draft: false
lang: en
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Sign XLSX via C# electronically"
head_description: "Utilize XLSX to add a range of electronic signature types to documents, ensuring security and compliance across formats like PDF, Word, Excel, Presentations, and Images."

############################# Header ############################
title: "Electronic signing of XLSX files" 
description: "Embed a variety of electronic signatures into your documents using GroupDocs.Signature for .NET, ensuring compliance and integrity for formats such as PDFs, Word, Excel, Presentations, and Images."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download for free"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "About GroupDocs.Signature for .NET API"
    link: "/signature/net/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) offers a comprehensive suite of electronic signing capabilities. With it, you can seamlessly add, search, verify, update, and remove digital signatures across a wide array of document types, without the need for third-party tools. It supports signing PDF files, Word documents, Excel sheets, PowerPoint presentations, and various image formats effortlessly.

############################# Steps ############################
steps:
    enable: true
    title: "Steps for signing XLSX using C#"
    content: |
      [GroupDocs.Signature](/signature/net/) facilitates the incorporation of customized signatures into XLSX files. .NET developers can seamlessly integrate signing functionality into their applications using our software.
      
      1. Provide the XLSX file to the Signature instance for signing.
      2. Utilize SignOptions to specify the signature parameters.
      3. Configure attributes such as size, color, and content.
      4. Save the signed file to the desired destination.
   
    code:
      platform: "net"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Sample signatures"
      install:
        command: "dotnet add package GroupDocs.Signature"
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```csharp {style=abap}
        // Load the document into a Signature instance
        using (Signature signature = new Signature("input.xlsx"))
        {
            // Create a new QrCodeSignOptions object
            QrCodeSignOptions options = new QrCodeSignOptions("QR code text")
            {
                // Configure all the necessary options
                Left = 50,
                Top = 200,
                ForeColor = Color.Red
            };

            // Persist the signed document to local storage
            SignResult result = signature.Sign("output.xlsx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Advanced document electronic signatures"
  description: "Our sophisticated e-signing API enhances business workflows, enabling efficient signing, validation, modification, and management of electronic signatures with full automation capabilities."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "Electronic signature capabilities"
  features:
    # feature loop
    - title: "Electronic signing for office documents"
      content: "Seamlessly insert electronic signatures at any position within a document. Customize and enrich content with digital certificates, metadata, barcodes, or visual elements, while ensuring authenticity and security."

    # feature loop
    - title: "Comprehensive signature management"
      content: "Once signed, documents can be further processed with ease. Access a complete overview of existing signatures, enabling precise updates or deletion of signatures where necessary."

    # feature loop
    - title: "Enhanced content security"
      content: "Protect the integrity of your documents using digital certificates. Embed or extract metadata for enhanced document tracking and auditing, ensuring compliance and content authenticity."
      
  code_samples_ext:
    # code sample ext loop
    - title: "How to add an image signature to a document"
      content: |
        This example illustrates the procedure for applying an image signature to a specific page within a document.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Provide the source document as an argument
          using (Signature signature = new Signature("input.xlsx"))
          {
              // Specify the path to the image in the signature configuration
              ImageSignOptions options = new ImageSignOptions("image.jpg")
              {
                  // Define the dimensions and target pages for the signature
                  VerticalAlignment = VerticalAlignment.Bottom,
                  HorizontalAlignment = HorizontalAlignment.Right,
                  Height = 150,
                  Width = 200,
                  Margin = new Padding(50),
                  AllPages = true
              };

              // Execute the application of the signature to the document
              SignResult result = signature.Sign("output.xlsx", options);
          }

          ```
        platform: "net"
        copy_title: "Copy"
        install:
          command: "dotnet add package GroupDocs.Signature"
          copy_tip: "click to copy"
          copy_done: "copied"
        top_links:
          #  loop
          - title: "Download result"
            icon: "download"
            link: "/examples/signature/formats/signature_esign.xlsx"
        links:
          #  loop
          - title: "More examples"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/signature/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Ready to get started?"
  description: "Try GroupDocs.Signature features for free or request a license"
  items:
    #  loop
    - title: "Nuget download"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Explore the full scope of our features"
    exclude: "esign"
    description: "We’re proud to offer a vast array of signature options and associated operations"
    items: 
          
        # operation loop 1
        - name: "Electronic signatures"
          operation: "esign"
          link: "/signature/net/esign/xlsx/"
          description: "Add various types of signatures to supported file formats"

        # operation loop 2
        - name: "Add text to documents"
          operation: "text"
          link: "/signature/net/text/xlsx/"
          description: "Enhance document content with customizable text signatures"

        # operation loop 3
        - name: "Image signatures"
          operation: "image"
          link: "/signature/net/image/xlsx/"
          description: "Place any image at any position within a document"

        # operation loop 4
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/signature/net/barcode/xlsx/"
          description: "Create and insert various barcodes into supported documents"

        # operation loop 5
        - name: "Generate QR codes"
          operation: "qrcode"
          link: "/signature/net/qrcode/xlsx/"
          description: "Generate and QR Codes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/net/digital/xlsx/"
          description: "Secure business and sign documents with digital certificates"

        # operation loop 7
        - name: "Stamp signatures"
          operation: "stamp"
          link: "/signature/net/stamp/xlsx/"
          description: "Use the Stamp Constructor to create custom round or square stamps"
          
        # operation loop 8
        - name: "Search signatures"
          operation: "search"
          link: "/signature/net/search/xlsx/"
          description: "Locate any previously added signatures within a document"
          
        # operation loop 9
        - name: "Signature verification"
          operation: "verify"
          link: "/signature/net/verify/xlsx/"
          description: "Verify the authenticity of signatures after they have been applied"
          
        # operation loop 10
        - name: "Modify signatures"
          operation: "modify"
          link: "/signature/net/modify/xlsx/"
          description: "Easily edit a variety of signatures within a document"
          
        # operation loop 11
        - name: "Delete signatures"
          operation: "delete"
          link: "/signature/net/delete/xlsx/"
          description: "Remove a wide range of previously applied signatures"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Digitally sign a wide range of file formats"
    exclude: "XLSX"
    description: "The .NET API empowers you to electronically sign over 60 industry-standard file formats, offering unparalleled flexibility in securing your business documents."
    items: 
          
        # format loop 1
        - name: "e-Sign PDF"
          format: "PDF"
          link: "/signature/net/esign/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "e-Sign DOCX"
          format: "DOCX"
          link: "/signature/net/esign/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "e-Sign JPEG"
          format: "JPEG"
          link: "/signature/net/esign/jpeg/"
          description: "JPEG Image"
          
        # format loop 4
        - name: "e-Sign PPTX"
          format: "PPTX"
          link: "/signature/net/esign/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "e-Sign XLSX"
          format: "XLSX"
          link: "/signature/net/esign/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---