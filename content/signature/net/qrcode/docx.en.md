



---
############################# Static ############################
layout: "format"
date:  2024-08-08T16:38:33
draft: false
lang: en
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Add Metadata to DOCX Files in C# Applications"
head_description: "C# metadata processing API to add metadata information to DOCX files. Work with metadata standards XMP, EXIF, IPTC, ID3 etc"

############################# Header ############################
title: "Adding Metadata To DOCX In C#" 
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
  title: "Document Metadata Management"
  description: "Our robust API simplifies the management of document metadata. Seamlessly access, edit, and manipulate a variety of document properties to enhance organization and searchability."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
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


############################# More Formats #####################
more_formats:
    enable: true
    title: "Adding Metadata Properties To Other File Formats"
    exclude: "DOCX"
    description: "Multi format documents and images metadata addition API for GroupDocs.Signature. Retrieve metadata of some of the popular file formats as stated below."
    items: 
          
        # format loop 1
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/signature/net//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Watermark JPEG"
          format: "JPEG"
          link: "/signature/net//jpeg/"
          description: "JPEG Image"
          
        # format loop 3
        - name: "Watermark PDF"
          format: "PDF"
          link: "/signature/net//pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 4
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/signature/net//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/signature/net//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---