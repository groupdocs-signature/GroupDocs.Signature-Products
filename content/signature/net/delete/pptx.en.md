



---
############################# Static ############################
layout: "format"
date:  2024-08-02T12:49:13
draft: false
lang: en
format: Pptx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Add Metadata to PPTX Files in C# Applications"
head_description: "C# metadata processing API to add metadata information to PPTX files. Work with metadata standards XMP, EXIF, IPTC, ID3 etc"

############################# Header ############################
title: "Adding Metadata To PPTX In C#" 
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
    title: "Procedures for Deleting Text Signatures from PPTX using C#"
    content: |
      [GroupDocs.Signature](/signature/net/) simplifies the task for .NET developers to remove text signatures in PPTX files by implementing a few straightforward steps.
      
      1. Provide the path of the PPTX file to an instance of the Signature class.
      2. Invoke the Search method to retrieve all text signatures within the document.
      3. Delete one or more of the retrieved text signatures.
      4. Examine the results of the document processing.
   
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
        // Pass the document containing signatures to the Signature instance
        using (Signature signature = new Signature("input.pptx"))
        {
            // Retrieve the text signatures present within the document
            TextSearchOptions options = new TextSearchOptions();
            List<TextSignature> signatures = signature.Search<TextSignature>(options);

            // Remove the first identified text signature
            if(signatures.Count > 0)
            {
                TextSignature textSignature = signatures[0];
                bool result = signature.Delete(textSignature);

                // Remove the first identified text signature
                if(result)
                {
                    Console.WriteLine($"Signature was deleted successfully");
                }
            }
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Document Metadata Management"
  description: "Our robust API simplifies the management of document metadata. Seamlessly access, edit, and manipulate a variety of document properties to enhance organization and searchability."
  image: "/img/signature/features_delete.webp" # 500x500 px
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
    - title: "Eliminate All QR-Code Signatures"
      content: |
        Discover how to remove all QR-code signatures embedded within a document.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        // Supply a document containing QR-code signatures
        using (Signature signature = new Signature("input.pptx"))
        {
            // Remove all QR-code signatures
            DeleteResult result = signature.Delete(SignatureType.QrCode);

            // Evaluate the outcome of the deletion process
            if (result.Succeeded.Count > 0)
            {
                Console.WriteLine("Following QR-Code signatures were deleted:");                    
                int number = 1;
                foreach (QrCodeSignature temp in result.Succeeded)
                {
                    Console.WriteLine($"Signature #{number++}: Type: {temp.SignatureType} 
                        Id:{temp.SignatureId}, Text: {temp.Text}");
                }
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
    exclude: "PPTX"
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