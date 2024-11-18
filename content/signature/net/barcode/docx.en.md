



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:06
draft: false
lang: en
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Generate barcode for DOCX using C# API"
head_description: "Generate a barcode signature and secure DOCX document using C# with just a few lines of code. Utilize GroupDocs.Signature for signing a wide range of file formats."

############################# Header ############################
title: "Generate barcode for DOCX documents" 
description: "Utilize GroupDocs.Signature for .NET to place barcodes anywhere within your business documents. Our API offers extensive customization options for barcode signatures."
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
    title: "Overview of GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) is a sophisticated document signing solution that supports an extensive array of signature types, including text, images, barcodes, digital certificates, and stamps. Compatible with over 60 file formats—such as PDF, MS Office, images, ZIP files, and more—this tool enables you to not only apply signatures but also search, verify, modify, or remove them as needed.

############################# Steps ############################
steps:
    enable: true
    title: "Steps to generate and embed a barcode in DOCX file"
    content: |
      [GroupDocs.Signature](/signature/net/) facilitates the generation of barcodes in numerous popular formats and their placement on DOCX pages. Supporting over 60 barcode types, .NET applications can be effortlessly augmented with barcode signing functionalities by integrating our library.
      
      1. Supply the DOCX file or stream for processing.
      2. Pass the barcode text to the BarcodeSignOptions instance.
      3. Tailor barcode options such as position, size, etc.
      4. Persist the file with the newly appended barcode.
   
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
        // Instantiate a new Signature object with the document path
        using (Signature signature = new Signature("input.docx"))
        {
            // Employ BarcodeSignOptions to append a barcode to the document
            BarcodeSignOptions options = new BarcodeSignOptions("Business data")
            {
                // Configure the barcode type and additional properties
                EncodeType = BarcodeTypes.Code128,
                Left = 50,
                Top = 150
            };

            // Persist the signed file
            SignResult result = signature.Sign("output.docx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Enhance and safeguard your documents with advanced signature capabilities"
  description: "The GroupDocs.Signature for .NET library is engineered to facilitate comprehensive document signing and processing across widely used file formats. With ease, you can add, adjust, verify, or remove different types of signatures."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Key Features of GroupDocs.Signature"
  features:
    # feature loop
    - title: "Versatile document signing"
      content: "Efficiently sign any page within supported documents using text, images, barcodes, QR codes, or stamps. Additionally, embed hidden metadata, such as EXIF data in images, or secure your document’s content against unauthorized alterations using digital certificates."

    # feature loop
    - title: "Comprehensive signature search and verification"
      content: "Our tool offers robust functionality for working with signed documents. Ensure the integrity of your documents by verifying signatures, and easily retrieve a comprehensive list of all signatures within a document through our search feature."

    # feature loop
    - title: "Edit signatures with ease"
      content: "Nearly all previously applied signatures can be modified. Conveniently update text, adjust positioning, or change colors to meet your needs."

    # feature loop
    - title: "Efficient signature deletion"
      content: "Our approach fully supports CRUD operations for signatures, allowing for the swift removal of any unwanted or outdated signatures from your documents."
      
  code_samples_ext:
    # code sample ext loop
    - title: "How to generate a barcode signature"
      content: |
        This example shows how to embed a customized barcode on DOCX document pages.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          using (Signature signature = new Signature("input.docx"))
          {
              // Formulate signature options with the desired text
              BarcodeSignOptions options = new BarcodeSignOptions("Accepted")
              {
                  EncodeType = BarcodeTypes.Code39FullASCII,

                  // Determine the relative barcode position on the page
                  VerticalAlignment = Domain.VerticalAlignment.Top,
                  HorizontalAlignment = Domain.HorizontalAlignment.Left,

                  // Define the barcode padding from the page edge
                  Margin = new Padding() { Top = 180, Right = 20 },

                  // Specify the color of the bars
                  ForeColor = Color.Red,

                  // Select the message font style
                  Font = new SignatureFont { Size = 12, FamilyName = "Arial" },

                  // Indicate the message position
                  CodeTextAlignment = CodeTextAlignment.Above
              };

              // Sign and persist the document
              SignResult result = signature.Sign("output.docx", options);
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
            link: "/examples/signature/formats/signature_barcode.docx"
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
    title: "Uncover our main features"
    exclude: "barcode"
    description: "We offer an impressive selection of signature options and operations"
    items: 
          
        # operation loop 1
        - name: "Electronic signatures"
          operation: "esign"
          link: "/signature/net/esign/docx/"
          description: "Add various types of signatures to supported file formats"

        # operation loop 2
        - name: "Add text to documents"
          operation: "text"
          link: "/signature/net/text/docx/"
          description: "Enhance document content with customizable text signatures"

        # operation loop 3
        - name: "Image signatures"
          operation: "image"
          link: "/signature/net/image/docx/"
          description: "Place any image at any position within a document"

        # operation loop 4
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/signature/net/barcode/docx/"
          description: "Create and insert various barcodes into supported documents"

        # operation loop 5
        - name: "Generate QR codes"
          operation: "qrcode"
          link: "/signature/net/qrcode/docx/"
          description: "Generate and QR Codes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/net/digital/docx/"
          description: "Secure business and sign documents with digital certificates"

        # operation loop 7
        - name: "Stamp signatures"
          operation: "stamp"
          link: "/signature/net/stamp/docx/"
          description: "Use the Stamp Constructor to create custom round or square stamps"
          
        # operation loop 8
        - name: "Search signatures"
          operation: "search"
          link: "/signature/net/search/docx/"
          description: "Locate any previously added signatures within a document"
          
        # operation loop 9
        - name: "Signature verification"
          operation: "verify"
          link: "/signature/net/verify/docx/"
          description: "Verify the authenticity of signatures after they have been applied"
          
        # operation loop 10
        - name: "Modify signatures"
          operation: "modify"
          link: "/signature/net/modify/docx/"
          description: "Easily edit a variety of signatures within a document"
          
        # operation loop 11
        - name: "Delete signatures"
          operation: "delete"
          link: "/signature/net/delete/docx/"
          description: "Remove a wide range of previously applied signatures"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Sign documents across a variety of formats"
    exclude: "DOCX"
    description: "Our .NET API supports the signing of more than 60 different formats. Effortlessly place various types of signatures on any page or at any desired position within your documents."
    items: 
          
        # format loop 1
        - name: "Add barcode to PDF"
          format: "PDF"
          link: "/signature/net/barcode/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Add barcode to DOCX"
          format: "DOCX"
          link: "/signature/net/barcode/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Add barcode to JPEG"
          format: "JPEG"
          link: "/signature/net/barcode/jpeg/"
          description: "JPEG Image"
          
        # format loop 4
        - name: "Add barcode to PPTX"
          format: "PPTX"
          link: "/signature/net/barcode/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "Add barcode to XLSX"
          format: "XLSX"
          link: "/signature/net/barcode/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---