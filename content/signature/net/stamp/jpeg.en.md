



---
############################# Static ############################
layout: "format"
date:  2024-10-08T11:43:25
draft: false
lang: en
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Round and square stamps JPEG via C#"
head_description: "Use GroupDocs.Signature for .NET to generate and embed personalized stamps across JPEG files."

############################# Header ############################
title: "Generate stamps for JPEG files" 
description: "Seamlessly integrate custom-designed stamps into any section of your documents using GroupDocs.Signature for .NET, offering extensive flexibility for stamp placement and configuration to meet your business needs."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Get your free download"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Overview of GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) is a versatile tool that enables the insertion of multiple signature types into documents, including customizable stamps. Supporting over 60 file formats, from PDFs and Word documents to images and ZIP files, you can enrich your documents with text, image, barcode, metadata, digital certificates, and stamps. Furthermore, you have full control to search, validate, modify, or remove any signatures applied to your files.

############################# Steps ############################
steps:
    enable: true
    title: "How to embed stamp into JPEG using C#"
    content: |
      [GroupDocs.Signature](/signature/net/) offers a robust stamp creation feature, ideal for enhancing .NET applications. Leverage this tool to design and implement highly customized stamps on your document pages.
      
      1. Provide the JPEG document to be stamped.
      2. Utilize StampSignOptions to meticulously configure all requisite parameters.
      3. Add multiple stamp lines as per your requirements.
      4. Apply the configured stamp and save the modified document.
   
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
        // Integrate the document path with the Signature instance
        using (Signature signature = new Signature("input.jpeg"))
        {
            // Initialize StampSignOptions with the required signature content
            StampSignOptions options = new StampSignOptions();
            options.Height = 180;
            options.Width = 180;

            // Incorporate one or multiple stamp lines
            options.OuterLines.Add(
                new StampLine()
                {
                    Text = "* The Best Company *",
                    TextRepeatType = StampTextRepeatType.FullTextRepeat,
                    Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                    Height = 22,
                    TextBottomIntent = 6,
                    TextColor = Color.WhiteSmoke,
                    BackgroundColor = Color.DarkSlateBlue
                }
            );

            // Preserve the document with the applied stamp
            SignResult result = signature.Sign("output.jpeg", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Leverage signatures to secure and enhance document integrity"
  description: "With the GroupDocs.Signature for .NET library, you can seamlessly integrate signature functionality into your documents. Easily add, modify, verify, or remove custom stamps and other signature types, offering flexibility and precision for secure document management."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Stamp Signatures Powered by GroupDocs.Signature"
  features:
    # feature loop
    - title: "Comprehensive document signing"
      content: "Enhance your documents by placing signatures, including text, images, barcodes, QR codes, and stamps, at any position or page within the file. Additionally, manage embedded metadata and apply digital certificates to safeguard against unauthorized changes."

    # feature loop
    - title: "Efficient signature search and validation"
      content: "After signing, verify the authenticity and integrity of document signatures. Utilize advanced search functionality to retrieve and manage all signature data embedded in the document."

    # feature loop
    - title: "Modify and customize signatures"
      content: "Adjust previously inserted signatures with ease. Whether you need to change the content, position, size, or color, our solution offers full flexibility for signature modification."

    # feature loop
    - title: "Effortlessly remove signatures"
      content: "When signatures need to be removed, GroupDocs.Signature for .NET provides a complete set of tools to delete any type of signature, including stamps, digital certificates, and more, ensuring that your documents remain up-to-date and compliant."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Implement custom stamps in documents"
      content: |
        Discover how to craft and integrate custom stamps bearing critical textual details into your documents.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Supply the document to be stamped
          using (Signature signature = new Signature("input.jpeg"))
          {
              // Initialize the stamp options with the desired configurations
              StampSignOptions options = new StampSignOptions()
              {
                    // Define the stamp’s dimensions and position on the page
                    Height = 200,
                    Width = 200,
                    VerticalAlignment = VerticalAlignment.Bottom,
                    HorizontalAlignment = HorizontalAlignment.Right,
                    AllPages = true
              };

              // Incorporate outer circular lines with text
              options.OuterLines.Add(
                    new StampLine()
                    {
                        Text = "* The best  choice *",
                        TextRepeatType = StampTextRepeatType.FullTextRepeat,
                        Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                        Height = 22,
                        TextBottomIntent = 6,
                        TextColor = Color.WhiteSmoke,
                        BackgroundColor = Color.DarkSlateBlue
                    }
              );

              // Integrate inner square lines if necessary
              options.InnerLines.Add(
                    new StampLine()
                    { 
                        Text = "Company #1",
                        TextColor = Color.MediumVioletRed,
                        Font = new SignatureFont() { Size = 20, Bold = true },
                        Height = 40
                    }
              );

              // Finalize and save the stamped document
              SignResult result = signature.Sign("output.jpeg", options);
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
            link: "/examples/signature/formats/signature_stamp.jpeg"
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
    title: "Explore core functionalities"
    exclude: "stamp"
    description: "Discover a broad range of options to create, manage, and delete various types of signatures, ensuring comprehensive control over your document workflows."
    items: 
          
        # operation loop 1
        - name: "Electronic signatures"
          operation: "esign"
          link: "/signature/net/esign/jpeg/"
          description: "Add various types of signatures to supported file formats"

        # operation loop 2
        - name: "Add text to documents"
          operation: "text"
          link: "/signature/net/text/jpeg/"
          description: "Enhance document content with customizable text signatures"

        # operation loop 3
        - name: "Image signatures"
          operation: "image"
          link: "/signature/net/image/jpeg/"
          description: "Place any image at any position within a document"

        # operation loop 4
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/signature/net/barcode/jpeg/"
          description: "Create and insert various barcodes into supported documents"

        # operation loop 5
        - name: "Generate QR codes"
          operation: "qrcode"
          link: "/signature/net/qrcode/jpeg/"
          description: "Generate and apply two-dimensional barcodes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "Secure business documents using digital certificates"

        # operation loop 7
        - name: "Stamp signatures"
          operation: "stamp"
          link: "/signature/net/stamp/jpeg/"
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
    title: "Apply stamps across various document formats"
    exclude: "JPEG"
    description: "The GroupDocs.Signature API allows you to embed stamps across more than 60 industry-standard file types. Effortlessly apply custom stamps to any location within your documents, enabling enhanced document tracking and personalization."
    items: 
          
        # format loop 1
        - name: "Stamp PDF"
          format: "PDF"
          link: "/signature/net/stamp/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Stamp DOCX"
          format: "DOCX"
          link: "/signature/net/stamp/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Stamp JPEG"
          format: "JPEG"
          link: "/signature/net/stamp/jpeg/"
          description: "JPEG Image"
          
        # format loop 4
        - name: "Stamp PPTX"
          format: "PPTX"
          link: "/signature/net/stamp/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "Stamp XLSX"
          format: "XLSX"
          link: "/signature/net/stamp/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---