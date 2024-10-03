



---
############################# Static ############################
layout: "format"
date:  2024-10-03T12:33:02
draft: false
lang: en
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Electronic signatures search for XLSX using Python"
head_description: "Leverage the GroupDocs.Signature for Python via .NET API to search for electronic signatures embedded in formats like PDFs, Word, Excel, Presentations, and Images."

############################# Header ############################
title: "XLSX digital signatures search" 
description: "Easily extract a complete list of electronic signatures from multiple formats, including PDFs, Word, Excel, Presentations, and Images, with the power of GroupDocs.Signature for Python via .NET."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download now"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Unleash the potential of GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) offers advanced capabilities for signing and managing digital documents. With support for over 60 file formats, including PDFs, Office documents, Images, and ZIP files, you can add, search, verify, modify, or remove signatures like text, images, barcodes, QR codes, digital certificates, and stamps.

############################# Steps ############################
steps:
    enable: true
    title: "How to search for signatures in XLSX using Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) provides a powerful engine for detecting digital signatures in XLSX files. Python via .NET developers can easily enhance their apps with this functionality.
      
      1. Provide the XLSX file path for the signature search.
      2. Use SearchOptions to refine the search criteria.
      3. Call the Search method to retrieve the results.
      4. Review the list of identified signatures.
   
    code:
      platform: "python-net"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Sample signatures"
      install:
        command: "pip install groupdocs-signature-net"
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/signature/python-net/"
          
      content: |
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Initialize a Signature object with the document's file path
            with sg.Signature('input.xlsx') as signature:

                # Create an instance of TextSearchOptions to search all pages
                options = sg.TextSearchOptions()
                options.AllPages = True

                # Run a search to locate any text-based signatures in the document
                signatures = signature.Search(options)
                print("\nSource document contains following text signature(s).")

                # Compile a list of found signatures for detailed review
                for textSignature in signatures:
                    print("\nFound Text signature at page ", textSignature.PageNumber)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "A complete document signing platform"
  description: "Experience a powerful, feature-rich signing solution that secures your documents with multiple signature types, spanning various file formats."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "Search and manage signatures"
  features:
    # feature loop
    - title: "Sign and secure business documents"
      content: "Add electronic signatures anywhere in a document. GroupDocs.Signature supports multiple signature types, including text, images, barcodes, metadata, stamps, and digital certificates, ensuring the document's authenticity and security."

    # feature loop
    - title: "Comprehensive signature management"
      content: "Once a document is signed, use the search feature to find all embedded signatures. You can modify or remove signatures as needed, giving you full control over the document’s integrity."

    # feature loop
    - title: "Ensure document integrity"
      content: "Use advanced tools to manage hidden metadata within documents. Add or remove metadata, and apply digital certificates to safeguard your documents from unauthorized changes, ensuring their authenticity."
      
  code_samples:
    # code sample loop
    - title: "Search for image signatures"
      content: |
        This example demonstrates how to find an image signature within a specific document.
        {{< landing/code title="C#">}}
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Pass the source document to the constructor
            with sg.Signature('input.xlsx') as signature:

                # Search for any text-based signatures
                signatures = signature.Search(sg.SignatureType.Image)
                print("\nSource document contains following image signature(s).")

                # Display detailed properties of the identified signatures
                for imageSignature in signatures:
                    print("\nFound image signature at page ", imageSignature.PageNumber)
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Ready to get started?"
  description: "Try GroupDocs.Signature features for free or request a license"
  items:
    #  loop
    - title: "PyPi download"
      link: "https://releases.groupdocs.com/signature/python-net/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Core features"
    exclude: "search"
    description: "Our API provides extensive flexibility, enabling users to sign documents and perform post-signing operations like searching, verifying, and editing signatures."
    items: 
          
        # operation loop 1
        - name: "Electronic signatures"
          operation: "esign"
          link: "/signature/python-net/esign/xlsx/"
          description: "Add various types of signatures to supported file formats"

        # operation loop 2
        - name: "Add text to documents"
          operation: "text"
          link: "/signature/python-net/text/xlsx/"
          description: "Enhance document content with customizable text signatures"

        # operation loop 3
        - name: "Image signatures"
          operation: "image"
          link: "/signature/python-net/image/xlsx/"
          description: "Place any image at any position within a document"

        # operation loop 4
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/signature/python-net/barcode/xlsx/"
          description: "Create and insert various barcodes into supported documents"

        # operation loop 5
        - name: "Generate QR codes"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "Generate and apply two-dimensional barcodes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/python-net/digital/xlsx/"
          description: "Secure business documents using digital certificates"

        # operation loop 7
        - name: "Stamp signatures"
          operation: "stamp"
          link: "/signature/python-net/stamp/xlsx/"
          description: "Use the Stamp Constructor to create custom round or square stamps"
          
        # operation loop 8
        - name: "Search signatures"
          operation: "search"
          link: "/signature/python-net/search/xlsx/"
          description: "Locate any previously added signatures within a document"
          
        # operation loop 9
        - name: "Signature verification"
          operation: "verify"
          link: "/signature/python-net/verify/xlsx/"
          description: "Verify the authenticity of signatures after they have been applied"
          
        # operation loop 10
        - name: "Modify signatures"
          operation: "modify"
          link: "/signature/python-net/modify/xlsx/"
          description: "Easily edit a variety of signatures within a document"
          
        # operation loop 11
        - name: "Delete signatures"
          operation: "delete"
          link: "/signature/python-net/delete/xlsx/"
          description: "Remove a wide range of previously applied signatures"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Extract signatures from multiple file formats"
    exclude: "XLSX"
    description: "The GroupDocs.Signature for Python via .NET API allows you to extract and manage signatures from a wide variety of document formats. Easily retrieve embedded signatures from major file types for further analysis or processing."
    items: 
          
        # format loop 1
        - name: "Search signatures in PDF"
          format: "PDF"
          link: "/signature/python-net/search/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Search signatures in DOCX"
          format: "DOCX"
          link: "/signature/python-net/search/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Search signatures in PPTX"
          format: "PPTX"
          link: "/signature/python-net/search/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Search signatures in XLSX"
          format: "XLSX"
          link: "/signature/python-net/search/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---