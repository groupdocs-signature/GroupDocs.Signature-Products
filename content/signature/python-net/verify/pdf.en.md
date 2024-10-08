



---
############################# Static ############################
layout: "format"
date:  2024-10-08T18:17:25
draft: false
lang: en
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Verify PDF digital signatures with Python"
head_description: "Utilize GroupDocs.Signature for Python via .NET to verify signatures within PDF files. Confirm the authenticity of signatures in PDFs, Word, Excel, Presentations, Images, and ZIP files."

############################# Header ############################
title: "PDF digital signatures verification" 
description: "Quickly and accurately verify electronic signatures in various formats, including PDFs, Word, Excel, Presentations, Images, and ZIP files using GroupDocs.Signature for Python via .NET."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download free version"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Main features of GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) offers comprehensive document signature management, supporting over 60 file formats such as PDFs, MS Office files, images, and ZIP archives. It allows you to apply various signature types, including text, images, barcodes, digital certificates, metadata, and stamps. Beyond signing, it also enables you to search, verify, edit, or remove signatures.

############################# Steps ############################
steps:
    enable: true
    title: "How to verify PDF signatures using Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) verifies specific signatures in PDF documents. Python via .NET developers can enhance their apps by integrating this verification feature.
      
      1. Load the PDF file into the Signature instance.
      2. Create and configure VerifyOptions to match the desired verification criteria.
      3. Start the verification process.
      4. Interpret the results from the verification process.
   
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

            # Initialize Signature with the document
            with sg.Signature('input.pdf') as signature:

                // Set up TextVerifyOptions to verify signatures with specific text
                options = sg.TextVerifyOptions()
                options.Text = "signature"
                options.MatchType = TextMatchType.Contains

                // Run the signature verification on the document
                result = signature.Verify(options)

                // Review and analyze the verification results
                if result.IsValid :
                    print("\nDocument was verified successfully!")
                    for item in result.Succeeded :
                         print("\nValid signature is found with text", item.Text)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Advanced digital signature tools"
  description: "GroupDocs.Signature provides a complete solution for signing and verifying documents across popular file formats. With support for seven signature types and full CRUD operations, you have total control over document protection and management."
  image: "/img/signature/features_verify.webp" # 500x500 px
  image_description: "Signature verification features"
  features:
    # feature loop
    - title: "Efficient document signing"
      content: "Easily add custom digital signatures to any part of your documents. GroupDocs.Signature for Python via .NET supports text, image, barcode, metadata, stamp, and digital certificate signatures, ensuring your documents meet business requirements."

    # feature loop
    - title: "Full signature lifecycle management"
      content: "Manage signatures throughout their entire lifecycle—access, verify, update, or remove signatures as needed to keep your documents accurate and up-to-date."

    # feature loop
    - title: "Protect document integrity"
      content: "Safeguard your sensitive documents by embedding digital certificates that prevent unauthorized changes. Add hidden metadata to protect crucial information and maintain document integrity."

    # feature loop
    - title: "Custom signature solutions"
      content: "Use document-specific signature types like PDF stamps and Word watermarks. These specialized signatures are perfect for branding, compliance, or adding a professional touch to your business documents."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Verify barcode signatures"
      content: |
        This example demonstrates how to verify barcode signatures in a document.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Load the document with barcode signatures
              with sg.Signature('input.pdf') as signature:

                  # Set the verification options to match specific barcode text
                  options = sg.BarcodeVerifyOptions()
                  options.Text = "12345"
                  options.MatchType = sg.TextMatchType.StartsWith

                  # Verify the signatures in the document
                  result = signature.Verify(options)

                  # Display the verification results
                  if result.IsValid :
                      print("\nDocument was verified successfully!")
                      for item in result.Succeeded :
                             print("\nValid signature is found with text", item.Text)
          ```
        platform: "python-net"
        copy_title: "Copy"
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
    title: "Signature management and operations"
    exclude: "verify"
    description: "Explore the extensive features and signature management operations provided by GroupDocs.Signature to have full control over document signature processes."
    items: 
          
        # operation loop 1
        - name: "Electronic signatures"
          operation: "esign"
          link: "/signature/python-net/esign/pdf/"
          description: "Add various types of signatures to supported file formats"

        # operation loop 2
        - name: "Add text to documents"
          operation: "text"
          link: "/signature/python-net/text/pdf/"
          description: "Enhance document content with customizable text signatures"

        # operation loop 3
        - name: "Image signatures"
          operation: "image"
          link: "/signature/python-net/image/pdf/"
          description: "Place any image at any position within a document"

        # operation loop 4
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/signature/python-net/barcode/pdf/"
          description: "Create and insert various barcodes into supported documents"

        # operation loop 5
        - name: "Generate QR codes"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/pdf/"
          description: "Generate and apply two-dimensional barcodes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "Secure business documents using digital certificates"

        # operation loop 7
        - name: "Stamp signatures"
          operation: "stamp"
          link: "/signature/python-net/stamp/pdf/"
          description: "Use the Stamp Constructor to create custom round or square stamps"
          
        # operation loop 8
        - name: "Search signatures"
          operation: "search"
          link: "/signature/python-net/search/pdf/"
          description: "Locate any previously added signatures within a document"
          
        # operation loop 9
        - name: "Signature verification"
          operation: "verify"
          link: "/signature/python-net/verify/pdf/"
          description: "Verify the authenticity of signatures after they have been applied"
          
        # operation loop 10
        - name: "Modify signatures"
          operation: "modify"
          link: "/signature/python-net/modify/pdf/"
          description: "Easily edit a variety of signatures within a document"
          
        # operation loop 11
        - name: "Delete signatures"
          operation: "delete"
          link: "/signature/python-net/delete/pdf/"
          description: "Remove a wide range of previously applied signatures"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Verify signatures across multiple formats"
    exclude: "PDF"
    description: "GroupDocs.Signature for Python via .NET allows you to verify signatures in a wide range of document formats. Customize verification parameters to ensure document integrity and meet compliance requirements."
    items: 
          
        # format loop 1
        - name: "Verify PDF signatures"
          format: "PDF"
          link: "/signature/python-net/verify/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Verify DOCX signatures"
          format: "DOCX"
          link: "/signature/python-net/verify/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Verify PPTX signatures"
          format: "PPTX"
          link: "/signature/python-net/verify/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Verify XLSX signatures"
          format: "XLSX"
          link: "/signature/python-net/verify/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---