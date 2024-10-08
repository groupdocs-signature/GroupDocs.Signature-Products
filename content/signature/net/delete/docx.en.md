



---
############################# Static ############################
layout: "format"
date:  2024-10-08T11:43:34
draft: false
lang: en
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Delete signatures from DOCX using C#"
head_description: "Deletion of Digital, Barcode, Text, Image, Metadata signatures from signed DOCX documents can be performed easily using GroupDocs.Signature for .NET."

############################# Header ############################
title: "Remove signatures from DOCX efficiently" 
description: "Beyond just signing business documents, our solution offers comprehensive tools to locate and remove a wide array of signatures using GroupDocs.Signature for .NET."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download at no cost"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Overview of GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/)  is a robust signing tool that facilitates the addition of diverse signature types, ranging from text and images to barcodes, digital certificates, and stamps. Supporting over 60 file formats—including PDF, MS Office, images, ZIP, and other widely-used business formats—this solution ensures flexibility in document management. Additionally, applied signatures can be easily located, authenticated, modified, or removed as needed.

############################# Steps ############################
steps:
    enable: true
    title: "How to delete e-signatures from DOCX using C#"
    content: |
      [GroupDocs.Signature](/signature/net/) simplifies the task for .NET developers to remove electronic signatures in DOCX files by implementing a few straightforward steps.
      
      1. Provide the path of the DOCX file to an instance of the Signature class.
      2. Invoke the Search method to retrieve all signatures within the document.
      3. Delete one or more of the retrieved signatures.
      4. Examine the results of the document processing.
   
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
        // Pass the document containing signatures to the Signature instance
        using (Signature signature = new Signature("input.docx"))
        {
            // Retrieve the digital signatures present within the document
            DigitalSearchOptions options = new DigitalSearchOptions();

            List<DigitalSignature> signatures = signature.Search<DigitalSignature>(options);

            // Remove the first identified digital signature
            if(signatures.Count > 0)
            {
                DigitalSignature digitalSignature = signatures[0];
                bool result = signature.Delete(digitalSignature);

                // Remove the first identified digital signature
                if(result)
                {
                    Console.WriteLine($"Digital signature in DOCX was deleted successfully");
                }
            }
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Optimize document management with advanced signature tools"
  description: "GroupDocs.Signature for .NET is meticulously designed to enhance the signing and processing of business file formats, enabling the addition, modification, verification, or deletion of signatures with ease."
  image: "/img/signature/features_delete.webp" # 500x500 px
  image_description: "Explore the Versatile Features of GroupDocs.Signature"
  features:
    # feature loop
    - title: "Document signing"
      content: "Effortlessly embed text, image, barcode, QR code, or stamp signatures onto any page of supported documents. Additionally, utilize hidden metadata such as EXIF in images or safeguard document integrity with digital certificates, preventing unauthorized alterations."

    # feature loop
    - title: "Signature search and verification"
      content: "Leverage our tools to ensure the authenticity of signatures within your documents. Conduct thorough searches to retrieve a complete list of all signatures, ensuring comprehensive document management."

    # feature loop
    - title: "Signature modification"
      content: "Easily refine previously added signatures by adjusting text, repositioning, or altering colors to meet your specific needs."

    # feature loop
    - title: "Signature deletion"
      content: "Our solution provides full CRUD capabilities for signatures, allowing you to efficiently remove a variety of signature types from your documents when necessary."
      
  code_samples:
    # code sample loop
    - title: "Eliminate all barcode signatures"
      content: |
        Discover how to remove all barcode signatures embedded within a document.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        // Supply a document containing barcode signatures
        using (Signature signature = new Signature("input.docx"))
        {
            // Remove all barcode signatures
            DeleteResult result = signature.Delete(SignatureType.Barcode);

            // Evaluate the outcome of the deletion process
            if (result.Succeeded.Count > 0)
            {
                Console.WriteLine("Following DOCX barcode signatures were deleted:");                    
                int number = 1;
                foreach (BarcodeSignature temp in result.Succeeded)
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


############################# More Operations #####################
more_operations:
    enable: true
    title: "Check out our highlighted features"
    exclude: "delete"
    description: "We are excited to offer a wide selection of supported signature types and operations"
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
          description: "Generate and apply two-dimensional barcodes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/net/digital/docx/"
          description: "Secure business documents using digital certificates"

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
    title: "Remove signatures across multiple file formats"
    exclude: "DOCX"
    description: "GroupDocs.Signature for .NET is engineered to facilitate the removal of signatures from an extensive range of over 60 file formats, ensuring broad compatibility and functionality."
    items: 
          
        # format loop 1
        - name: "Delete PDF signatures"
          format: "PDF"
          link: "/signature/net/delete/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Delete DOCX signatures"
          format: "DOCX"
          link: "/signature/net/delete/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Delete PPTX signatures"
          format: "PPTX"
          link: "/signature/net/delete/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Delete XLSX signatures"
          format: "XLSX"
          link: "/signature/net/delete/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---