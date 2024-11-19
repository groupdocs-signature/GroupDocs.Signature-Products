



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:32
draft: false
lang: en
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Search electronic signatures in PDF with C#"
head_description: "Utilize capabilities of the GroupDocs.Signature for .NET API to search for signatures embedded in PDFs, Word, Excel, Presentations, and Images."

############################# Header ############################
title: "Search for digital signatures in PDF" 
description: "Seamlessly extract a comprehensive list of electronic signatures embedded across various formats like PDFs, Word, Excel, Presentations, and Images, all powered by GroupDocs.Signature for .NET."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Start your free download"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Explore GroupDocs.Signature for .NET capabilities"
    link: "/signature/net/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) delivers cutting-edge functionality for digital document signing. With support for over 60 file formats, including PDFs, MS Office documents, Images, and ZIP files, it allows you to add, search, verify, modify, or remove various signatures, such as text, images, barcodes, QR codes, digital certificates, and stamps.

############################# Steps ############################
steps:
    enable: true
    title: "How to search PDF signatures using C#"
    content: |
      [GroupDocs.Signature](/signature/net/) offers a robust engine for locating digital signatures within PDF files. .NET developers can effortlessly enhance their applications with our solution.
      
      1. Supply the PDF file path for the signature search.
      2. Employ SearchOptions to refine the search criteria.
      3. Invoke the Search method to retrieve the results.
      4. Assess the list of identified signatures.
   
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
  title: "Complete document signing ecosystem"
  description: "Discover an advanced, feature-rich document signing solution, specifically designed to enhance and secure your documents with multiple signature types across various formats."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "Signature search and management"
  features:
    # feature loop
    - title: "Sign and secure business documents"
      content: "Add digital signatures to any position within a document. GroupDocs.Signature supports an array of signature types, including text, images, barcodes, metadata, stamps, and digital certificates, ensuring document authenticity and compliance."

    # feature loop
    - title: "Comprehensive signature management"
      content: "After signing, leverage the search feature to retrieve all embedded signatures. Modify or delete signatures as needed, providing you with complete control over document integrity."

    # feature loop
    - title: "Safeguard your document's integrity"
      content: "Utilize advanced tools to manage hidden metadata embedded within documents. Add or remove metadata entries and apply corporate digital certificates to protect against unauthorized edits and ensure document authenticity."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Search image signatures"
      content: |
        This example illustrates the process of detecting an image signature within a specified document.
      code:
        title: "C#"
        content: |
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
    title: "Core functionalities"
    exclude: "search"
    description: "Our API offers extensive flexibility, enabling users to sign documents and conduct comprehensive post-signing operations, such as searching, verifying, and modifying signatures."
    items: 
          
        # operation loop 1
        - name: "Electronic signatures"
          operation: "esign"
          link: "/signature/net/esign/pdf/"
          description: "Add various types of signatures to supported file formats"

        # operation loop 2
        - name: "Add text to documents"
          operation: "text"
          link: "/signature/net/text/pdf/"
          description: "Enhance document content with customizable text signatures"

        # operation loop 3
        - name: "Image signatures"
          operation: "image"
          link: "/signature/net/image/pdf/"
          description: "Place any image at any position within a document"

        # operation loop 4
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/signature/net/barcode/pdf/"
          description: "Create and insert various barcodes into supported documents"

        # operation loop 5
        - name: "Generate QR codes"
          operation: "qrcode"
          link: "/signature/net/qrcode/pdf/"
          description: "Generate and QR Codes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "Secure business and sign documents with digital certificates"

        # operation loop 7
        - name: "Stamp signatures"
          operation: "stamp"
          link: "/signature/net/stamp/pdf/"
          description: "Use the Stamp Constructor to create custom round or square stamps"
          
        # operation loop 8
        - name: "Search signatures"
          operation: "search"
          link: "/signature/net/search/pdf/"
          description: "Locate any previously added signatures within a document"
          
        # operation loop 9
        - name: "Signature verification"
          operation: "verify"
          link: "/signature/net/verify/pdf/"
          description: "Verify the authenticity of signatures after they have been applied"
          
        # operation loop 10
        - name: "Modify signatures"
          operation: "modify"
          link: "/signature/net/modify/pdf/"
          description: "Easily edit a variety of signatures within a document"
          
        # operation loop 11
        - name: "Delete signatures"
          operation: "delete"
          link: "/signature/net/delete/pdf/"
          description: "Remove a wide range of previously applied signatures"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Retrieve signatures from a variety of file formats"
    exclude: "PDF"
    description: "The GroupDocs.Signature for .NET API empowers you to extract and manage signatures from a wide array of document types. Effortlessly retrieve embedded signatures from all major file formats for further analysis or processing."
    items: 
          
        # format loop 1
        - name: "Search signatures in PDF"
          format: "PDF"
          link: "/signature/net/search/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Find signatures in DOCX"
          format: "DOCX"
          link: "/signature/net/search/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Find signatures in PPTX"
          format: "PPTX"
          link: "/signature/net/search/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Search signatures in XLSX"
          format: "XLSX"
          link: "/signature/net/search/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---