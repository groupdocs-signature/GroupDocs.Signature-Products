



---
############################# Static ############################
layout: "format"
date:  2024-09-06T10:45:36
draft: false
lang: en
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Add Metadata to XLSX Files in C# Applications"
head_description: "C# metadata processing API to add metadata information to XLSX files. Work with metadata standards XMP, EXIF, IPTC, ID3 etc"

############################# Header ############################
title: "Adding Metadata To XLSX In C#" 
description: "Add custom metadata properties to a wide range of business documents, images, audio & video file formats using GroupDocs.Signature for .NET API"
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download Free Trial"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "About GroupDocs.Signature for .NET API"
    link: "/signature/net/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) offers an advanced set of metadata management and manipulation features, allowing .NET programmers to easily view, edit, delete, find, compare, swap and export metadata information from images and document formats without using any external software. Add metadata details to PDF, Microsoft Word, Excel, PowerPoint, Outlook, OneNote, Visio, Project, AutoCAD, Archive and Multimedia file formats with additional support to perform metadata operations on any GroupDocs.Signature-based applications with true flexibility

############################# Steps ############################
steps:
    enable: true
    title: "Procedure for Embedding Text Signatures into XLSX Documents Using C#"
    content: |
      [GroupDocs.Signature](/signature/net/) facilitates the incorporation of text signatures into XLSX files within .NET applications. Enhance your product capabilities swiftly with our comprehensive solutions.
      
      1. Pass the XLSX document as a parameter to the Signature class constructor.
      2. Create TextSignOptions with the necessary signature text.
      3. Define the visual attributes for the signature.
      4. Embed the text signature onto any specified page(s) of the document.
   
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
        // Initialize the Signature with the document path
        using (Signature signature = new Signature("input.xlsx"))
        {
            // Create an instance of TextSignOptions with the desired signature text
            TextSignOptions options = new TextSignOptions("John Smith")
            {
                // Configure the text color and font attributes
                ForeColor = Color.Red,
                Font = new SignatureFont { Size = 14, FamilyName = "Comic Sans MS" }
            };

            // Integrate the text signature into the document
            SignResult result = signature.Sign("output.xlsx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Document Metadata Management"
  description: "Our robust API simplifies the management of document metadata. Seamlessly access, edit, and manipulate a variety of document properties to enhance organization and searchability."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "Metadata Manipulation Features"
  features:
    # feature loop
    - title: "Metadata Control"
      content: "Easily retrieve and process metadata from documents. Gain valuable insights into properties such as author, creation date, and more."

    # feature loop
    - title: "Metadata Editing"
      content: "Directly modify document metadata. Update properties to improve organization, boost searchability, and ensure accurate information."

    # feature loop
    - title: "Advanced Metadata Management"
      content: "Execute complex operations on document metadata. Efficiently add custom properties, remove unnecessary data, and maintain data consistency."
      
  code_samples:
    # code sample loop
    - title: "Embed Text Signatures in Documents"
      content: |
        Discover how to incorporate textual signatures into business documents to streamline processes.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        // Select the document to be signed
        using (Signature signature = new Signature("input.xlsx"))
        {
            // Formulate text options with the specified content
            TextSignOptions options = new TextSignOptions("Rescheduled to 03/04/2025")
            {
                // Define the dimensions and position of the signature on the page
                Left = 100,
                Top = 100,
                Width = 100,
                Height = 30,

                // Implement padding from the page edges for signatures
                Margin = new Padding() { Top = 20, Right = 20 },

                // Customize the text color and font style
                ForeColor = Color.Red,
                Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" },

                // Incorporate a border around the text signature
                Border = new Border()
                {
                    Color = Color.IndianRed,
                    DashStyle = DashStyle.DashLongDashDot,
                    Transparency = 0.5,
                    Visible = true,
                    Weight = 2
                },

                // Apply background customization if necessary
                Background = new Background()
                {
                    Color = Color.LimeGreen,
                    Transparency = 0.5,
                    Brush = new LinearGradientBrush(Color.LimeGreen, Color.DarkGreen)
                },

                // Rotate the signature to the desired angle on the page
                RotationAngle = 45,

                // Optionally save the text as an image to ensure compatibility
                SignatureImplementation = TextSignatureImplementation.Image
            };

            // Save the document with the integrated text signature
            SignResult result = signature.Sign("output.xlsx", options);
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
    exclude: "text"
    description: ""
    items: 
          
        # operation loop 1
        - name: "Electronic Signatures"
          operation: "esign"
          link: "/signature/net/esign/xlsx/"
          description: "Add various types of signatures to supported file formats."

        # operation loop 2
        - name: "Add Text to Documents"
          operation: "text"
          link: "/signature/net/text/xlsx/"
          description: "Enhance document content with customizable text signatures."

        # operation loop 3
        - name: "Image Signatures"
          operation: "image"
          link: "/signature/net/image/xlsx/"
          description: "Place any image at any position within a document."

        # operation loop 4
        - name: "Generate Barcodes"
          operation: "barcode"
          link: "/signature/net/barcode/xlsx/"
          description: "Create and insert various barcodes into supported documents."

        # operation loop 5
        - name: "Generate QR Codes"
          operation: "qrcode"
          link: "/signature/net/qrcode/xlsx/"
          description: "Generate and apply two-dimensional barcodes, including QR codes, for document signing."
          
        # operation loop 6
        - name: "Digital Certificates"
          operation: "digital"
          link: "/signature/net/digital/xlsx/"
          description: "Secure business documents using digital certificates."

        # operation loop 7
        - name: "Stamp Signatures"
          operation: "stamp"
          link: "/signature/net/stamp/xlsx/"
          description: "Use the Stamp Constructor to create custom round or square stamps."
          
        # operation loop 8
        - name: "Search Signatures"
          operation: "search"
          link: "/signature/net/search/xlsx/"
          description: "Locate any previously added signatures within a document."
          
        # operation loop 9
        - name: "Signature Verification"
          operation: "verify"
          link: "/signature/net/verify/xlsx/"
          description: "Verify the authenticity of signatures after they have been applied."
          
        # operation loop 10
        - name: "Modify Signatures"
          operation: "modify"
          link: "/signature/net/modify/xlsx/"
          description: "Easily edit a variety of signatures within a document."
          
        # operation loop 11
        - name: "Delete Signatures"
          operation: "delete"
          link: "/signature/net/delete/xlsx/"
          description: "Remove a wide range of previously applied signatures."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Adding Metadata Properties To Other File Formats"
    exclude: "XLSX"
    description: "Multi format documents and images metadata addition API for GroupDocs.Signature. Retrieve metadata of some of the popular file formats as stated below."
    items: 
          
        # format loop 1
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/signature/net/text/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Watermark JPEG"
          format: "JPEG"
          link: "/signature/net/text/jpeg/"
          description: "JPEG Image"
          
        # format loop 3
        - name: "Watermark PDF"
          format: "PDF"
          link: "/signature/net/text/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 4
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/signature/net/text/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/signature/net/text/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---