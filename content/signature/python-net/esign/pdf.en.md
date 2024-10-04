



---
############################# Static ############################
layout: "format"
date:  2024-10-04T11:53:12
draft: false
lang: en
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "E-sign PDF documents with Python apps"
head_description: "Harness the power of the Python API to electronically sign and secure PDF documents like PDFs, Word files, Excel sheets, presentations, and images."

############################# Header ############################
title: "E-sign PDF electronically" 
description: "Use GroupDocs.Signature for Python via .NET to embed a variety of electronic signatures into your documents, ensuring compliance and data integrity across formats like PDFs, Word, Excel, presentations, and images."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download for free"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Overview of the GroupDocs.Signature for Python via .NET API"
    link: "/signature/python-net/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) provides a full suite of tools for adding electronic signatures to documents. Whether you need to sign, search, verify, update, or remove digital signatures, GroupDocs.Signature for Python via .NET makes it easy across multiple formats—PDFs, Word docs, Excel sheets, PowerPoint presentations, and various image formats—without needing third-party software.

############################# Steps ############################
steps:
    enable: true
    title: "Steps to e-sign PDF using Python"
    content: |
      With [GroupDocs.Signature](/signature/python-net/), Python via .NET developers can seamlessly integrate signature functionality into PDF documents. Easily add customized signatures to your applications.
      
      1. Load the PDF file into the Signature instance.
      2. Use SignOptions to configure the signature settings.
      3. Customize signature properties like size, color, and content.
      4. Save the signed document to the desired location.
   
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

            # Load the document into a Signature instance
            with sg.Signature('input.pdf') as signature:

                # Create a new QrCodeSignOptions object
                options = sg.QrCodeSignOptions("QR code text")

                # Set up all required options
                options.Left = 100
                options.Top = 100
                options.ForeColor = sg.Color.Red

                # Save the signed document to your system
                result = signature.Sign("output.pdf", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Advanced e-signature features for documents"
  description: "Our e-signing API streamlines business processes by offering efficient ways to sign, validate, modify, and manage electronic signatures with full automation support."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "E-signature Features"
  features:
    # feature loop
    - title: "E-sign office documents"
      content: "Easily place electronic signatures anywhere in your documents. Customize your content with digital certificates, barcodes, metadata, and visual elements, all while ensuring document security and authenticity."

    # feature loop
    - title: "Full signature management"
      content: "Once a document is signed, you can view and manage all signatures. You can make updates or remove signatures as needed, ensuring complete control over the document."

    # feature loop
    - title: "Boost document security"
      content: "Protect your documents with digital certificates. Embed or retrieve metadata to improve tracking, auditing, and compliance, ensuring the authenticity of your content."
      
  code_samples_ext:
    # code sample ext loop
    - title: "How to add an image signature to a document"
      content: |
        This example demonstrates how to apply an image signature to a specific page of a document.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg
        
          def run():

              # Load the document you want to sign
              with sg.Signature('input.pdf') as signature:

                  # Set the path to the image in the signature options
                  options = sg.ImageSignOptions("image.jpg")

                  # Define the size and placement of the signature on the target pages
                  options.Left = 50
                  options.Top = 50
                  options.AllPages = True

                  # Apply the signature and save the signed document
                  result = signature.Sign("output.pdf", options)
          ```
        platform: "python-net"
        copy_title: "Copy"
        install:
          command: "pip install groupdocs-signature-net"
          copy_tip: "click to copy"
          copy_done: "copied"
        top_links:
          #  loop
          - title: "Download result"
            icon: "download"
            link: "/examples/signature/formats/signature_esign.pdf"
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
    title: "Explore our full feature set"
    exclude: "esign"
    description: "We offer a wide range of signature options and operations for all your e-signature needs."
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
    title: "E-sign a wide range of file formats"
    exclude: "PDF"
    description: "With the Python via .NET API, you can electronically sign over 60 industry-standard formats, offering unparalleled flexibility in securing your business documents."
    items: 
          
        # format loop 1
        - name: "e-Sign PDFs"
          format: "PDF"
          link: "/signature/python-net/esign/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "e-Sign DOCX"
          format: "DOCX"
          link: "/signature/python-net/esign/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "e-Sign JPEG"
          format: "JPEG"
          link: "/signature/python-net/esign/jpeg/"
          description: "JPEG Image"
          
        # format loop 4
        - name: "e-Sign PPTX"
          format: "PPTX"
          link: "/signature/python-net/esign/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "e-Sign XLSX"
          format: "XLSX"
          link: "/signature/python-net/esign/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---