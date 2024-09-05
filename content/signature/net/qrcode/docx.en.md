



---
############################# Static ############################
layout: "format"
date:  2024-09-05T19:56:56
draft: false
lang: en
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Create 2D Barcodes for DOCX Documents Using C# Applications"
head_description: "Harness the GroupDocs.Signature API to generate 2D barcodes for DOCX files. Seamlessly embed QR codes on any page for enhanced functionality."

############################# Header ############################
title: "Generate QR Codes for DOCX with C#" 
description: "Effortlessly generate 2D barcodes using text or numeric data and apply them across multiple pages and formats, including PDFs, Word, Excel, and more, via GroupDocs.Signature for .NET."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Start Your Free Trial"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Discover the Capabilities of GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) offers an expansive range of features, empowering users to generate and embed various signature types across leading document formats. Whether it’s PDFs, Word documents, Excel sheets, PowerPoint presentations, or image files, you can elevate your documents with Text, Image, Barcode, QR Code, Metadata, Digital, and Stamp signatures.

############################# Steps ############################
steps:
    enable: true
    title: "Procedure to Generate and Embed a QR-Code on DOCX Pages"
    content: |
      [GroupDocs.Signature](/signature/net/) facilitates the generation of QR-Codes in various popular formats and their placement on DOCX pages. Supporting over 10 types of QR-Codes, our library can be seamlessly integrated into .NET applications. Enhance your documents with QR-Code signatures using our product.
      
      1. Acquire the DOCX file or stream to be signed with a QR-Code.
      2. Provide the requisite text to QrCodeSignOptions.
      3. Customize visual parameters such as color, position, size, etc.
      4. Persist the document with the embedded QR-Code.
   
    code:
      platform: "net"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/signature_all.pdf"
      result_title: "Download signatures"
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
        // Initialize a new Signature instance with the document
        using (Signature signature = new Signature("input.docx"))
        {
            // Utilize QrCodeSignOptions to embed a QR-Code into the document
            QrCodeSignOptions options = new QrCodeSignOptions("Text Content")
                {
                    // Specify the signature type and designate its position on the page
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150
                };

            // Persist the document with the integrated QR-Code
            SignResult result = signature.Sign("output.docx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Comprehensive Signature Integration for Documents"
  description: "With GroupDocs.Signature for .NET API, users can effortlessly generate, modify, search, validate, and remove an array of signature types, streamlining document workflows with unparalleled precision."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Key Features of GroupDocs.Signature"
  features:
    # feature loop
    - title: "Document Signing with Multiple Signature Types"
      content: "GroupDocs.Signature enables the application of Text, Image, Barcode, QR Code, and Stamp signatures to any document format. Signatures can be precisely placed on any page, and metadata can be seamlessly managed through metadata signatures. Protect the integrity of your documents by incorporating digital certificates that prevent unauthorized alterations."

    # feature loop
    - title: "Signature Search and Validation"
      content: "Verify the authenticity and accuracy of document signatures through an advanced validation process. Easily retrieve a detailed list of all signatures embedded in a document for comprehensive oversight."

    # feature loop
    - title: "Customizable Signature Modification"
      content: "Update and refine previously applied signatures by adjusting content, placement, color, size, and other attributes to meet your specific needs."
      
  code_samples:
    # code sample loop
    - title: "How to Customize a Generated QR-Code"
      content: |
        This example demonstrates how to place a customized QR-Code on a DOCX page.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        // Retrieve the document to be signed and pass it to Signature
        using (Signature signature = new Signature("input.docx"))
        {
            // Configure QR-Code options with the necessary text
            QrCodeSignOptions options = new QrCodeSignOptions("Archived on July 11, 2019")
            {
                // Designate the relative position of the QR-Code on the page
                VerticalAlignment = Domain.VerticalAlignment.Top,
                HorizontalAlignment = Domain.HorizontalAlignment.Right,

                // Set the signature padding
                Margin = new Padding() { Top = 20, Right = 20 },

                // Specify the QR-Code color
                ForeColor = Color.Red,

                // Define the font options for the message
                Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" },

                // Customize the QR-Code background color and brush
                Background = new Background()
                {
                    Color = Color.LimeGreen,
                    Transparency = 0.5,
                    Brush = new LinearGradientBrush(Color.LimeGreen, Color.DarkGreen)
                }
            }

            // Embed the QR-Code into the document
            SignResult result = signature.Sign("output.docx", options);
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
    title: ""
    exclude: "qrcode"
    description: ""
    items: 
          
        # operation loop 1
        - name: "Electronic Signatures"
          operation: "esign"
          link: "/signature/net/esign/docx/"
          description: "Add various types of signatures to supported file formats."

        # operation loop 2
        - name: "Add Text to Documents"
          operation: "text"
          link: "/signature/net/text/docx/"
          description: "Enhance document content with customizable text signatures."

        # operation loop 3
        - name: "Image Signatures"
          operation: "image"
          link: "/signature/net/image/docx/"
          description: "Place any image at any position within a document."

        # operation loop 4
        - name: "Generate Barcodes"
          operation: "barcode"
          link: "/signature/net/barcode/docx/"
          description: "Create and insert various barcodes into supported documents."

        # operation loop 5
        - name: "Generate QR Codes"
          operation: "qrcode"
          link: "/signature/net/qrcode/docx/"
          description: "Generate and apply two-dimensional barcodes, including QR codes, for document signing."
          
        # operation loop 6
        - name: "Digital Certificates"
          operation: "digital"
          link: "/signature/net/digital/docx/"
          description: "Secure business documents using digital certificates."

        # operation loop 7
        - name: "Stamp Signatures"
          operation: "stamp"
          link: "/signature/net/stamp/docx/"
          description: "Use the Stamp Constructor to create custom round or square stamps."
          
        # operation loop 8
        - name: "Search Signatures"
          operation: "search"
          link: "/signature/net/search/docx/"
          description: "Locate any previously added signatures within a document."
          
        # operation loop 9
        - name: "Signature Verification"
          operation: "verify"
          link: "/signature/net/verify/docx/"
          description: "Verify the authenticity of signatures after they have been applied."
          
        # operation loop 10
        - name: "Modify Signatures"
          operation: "modify"
          link: "/signature/net/modify/docx/"
          description: "Easily edit a variety of signatures within a document."
          
        # operation loop 11
        - name: "Delete Signatures"
          operation: "delete"
          link: "/signature/net/delete/docx/"
          description: "Remove a wide range of previously applied signatures."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Generate QR Codes for Diverse Document Formats"
    exclude: "DOCX"
    description: "Enhance all industry-standard file formats with the ability to embed QR codes through the .NET API. Store and encode critical information into 2D barcodes for seamless scanning and data retrieval."
    items: 
          
        # format loop 1
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/signature/net/qrcode/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Watermark JPEG"
          format: "JPEG"
          link: "/signature/net/qrcode/jpeg/"
          description: "JPEG Image"
          
        # format loop 3
        - name: "Watermark PDF"
          format: "PDF"
          link: "/signature/net/qrcode/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 4
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/signature/net/qrcode/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/signature/net/qrcode/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---