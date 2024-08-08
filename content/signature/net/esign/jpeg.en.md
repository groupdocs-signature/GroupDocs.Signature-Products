



---
############################# Static ############################
layout: "format"
date:  2024-08-08T16:38:34
draft: false
lang: en
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Add Metadata to JPEG Files in C# Applications"
head_description: "C# metadata processing API to add metadata information to JPEG files. Work with metadata standards XMP, EXIF, IPTC, ID3 etc"

############################# Header ############################
title: "Adding Metadata To JPEG In C#" 
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
    title: "Steps for Signing JPEG Documents with Text Signatures using C#"
    content: |
      [GroupDocs.Signature](/signature/net/) facilitates the incorporation of customized text signatures into JPEG files. .NET developers can seamlessly integrate signing functionality into their applications using our software.
      
      1. Provide the JPEG file to the Signature instance for signing.
      2. Utilize TextSignOptions to specify the signature parameters.
      3. Configure attributes such as size, color, and content.
      4. Save the signed file to the desired destination.
   
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
        // Load the document into a Signature instance
        using (Signature signature = new Signature("input.jpeg"))
        {
            // Create a new TextSignOptions object
            TextSignOptions options = new TextSignOptions("John Smith")
            {
                // Configure all the necessary options
                Left = 50,
                Top = 200,
                ForeColor = Color.Red
            };

            // Persist the signed document to local storage
            SignResult result = signature.Sign("output.jpeg", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Document Metadata Management"
  description: "Our robust API simplifies the management of document metadata. Seamlessly access, edit, and manipulate a variety of document properties to enhance organization and searchability."
  image: "/img/signature/features_esign.webp" # 500x500 px
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
    - title: "How to Affix an Image Signature to a Document"
      content: |
        This example illustrates the procedure for applying an image signature to a specific page within a document.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
        // Provide the source document as an argument
        using (Signature signature = new Signature("input.jpeg"))
        {
            // Specify the path to the image in the signature configuration
            ImageSignOptions options = new ImageSignOptions("image.jpg")
            {
                // Define the dimensions and target pages for the signature
                Left = 50,
                Top = 50,
                AllPages = true
            };

            // Execute the application of the signature to the document
            SignResult result = signature.Sign("output.jpeg", options);
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
    exclude: "JPEG"
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