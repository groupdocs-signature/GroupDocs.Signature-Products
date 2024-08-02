



---
############################# Static ############################
layout: "format"
date:  2024-08-02T13:50:41
draft: false
lang: en
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Add Metadata to PDF Files in C# Applications"
head_description: "C# metadata processing API to add metadata information to PDF files. Work with metadata standards XMP, EXIF, IPTC, ID3 etc"

############################# Header ############################
title: "Adding Metadata To PDF In C#" 
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
    title: "Steps for Locating Signatures in PDF using C#"
    content: |
      [GroupDocs.Signature](/signature/net/) offers a robust engine for locating digital signatures within PDF files. .NET developers can effortlessly enhance their applications with our solution.
      
      1. Supply the PDF file path for the signature search.
      2. Employ TextSearchOptions to refine the search criteria.
      3. Invoke the Search method to retrieve the results.
      4. Assess the list of identified signatures.
   
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
        // Initialize a Signature object with the specified document path
        using (Signature signature = new Signature("input.pdf"))
        {
            // Create an instance of TextSearchOptions to encompass all pages
            TextSearchOptions options = new TextSearchOptions()
            {
                AllPages = true
            };

            // Execute a search to identify any text-based signatures in the document
            List<TextSignature> signatures = signature.Search<TextSignature>(options);
            Console.WriteLine($"\nSource document contains following text signature(s).");

            // Compile a list of detected signatures for detailed examination               
            foreach (TextSignature textSignature in signatures)
            {
                Console.WriteLine($"Found Text signature at page {textSignature.PageNumber} with type
                    [{textSignature.SignatureImplementation}] and text '{textSignature.Text}'.");
            }
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Document Metadata Management"
  description: "Our robust API simplifies the management of document metadata. Seamlessly access, edit, and manipulate a variety of document properties to enhance organization and searchability."
  image: "/img/signature/features_search.webp" # 500x500 px
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
    - title: "Locating Image Signatures"
      content: |
        This example illustrates the process of detecting an image signature within a specified document.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
        // Provide the source document as an argument to the constructor
        using (Signature signature = new Signature("input.pdf"))
        {
            // Search for any signatures of the text type
            List<ImageSignature> signatures = signature.Search<ImageSignature>(SignatureType.Image);
            Console.WriteLine($"\nSource document contains following image signature(s).");

            // Present the results with detailed properties of the identified signatures
            foreach (ImageSignature imageSignature in signatures)
            {
                Console.WriteLine($"Found Image signature at page {imageSignature.PageNumber} 
                and size {imageSignature.Size}.");
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
    exclude: "PDF"
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