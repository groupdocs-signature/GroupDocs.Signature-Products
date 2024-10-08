



---
############################# Static ############################
layout: "format"
date:  2024-10-08T11:43:30
draft: false
lang: en
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Generate a barcode for XLSX with Python"
head_description: "Easily generate a barcode signature and insert it into a XLSX document using Python. Use GroupDocs.Signature to sign a variety of file formats with just a few lines of code."

############################# Header ############################
title: "Generate barcodes for XLSX" 
description: "With GroupDocs.Signature for Python via .NET, you can place barcodes in your business documents wherever needed. Our solution provides flexible options for barcode signature customization."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Free trial"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "About GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) is a powerful document signing tool that supports a wide range of signature types, including text, images, barcodes, digital certificates, and stamps. Compatible with over 60 file formats, such as PDF, MS Office, images, ZIP, and more, it not only allows you to apply signatures but also lets you search, verify, modify, or remove them as needed.

############################# Steps ############################
steps:
    enable: true
    title: "Steps to generate and insert a barcode in XLSX"
    content: |
      [GroupDocs.Signature](/signature/python-net/) allows you to generate and embed barcodes in XLSX documents quickly and easily. Supporting more than 60 barcode formats, Python via .NET applications can seamlessly add barcode signing functionality by integrating our library.
      
      1. Provide the XLSX file or stream for processing.
      2. Assign the barcode text to the BarcodeSignOptions object.
      3. Adjust barcode options, such as position and size.
      4. Save the document with the embedded barcode.
   
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

            # Initialize the Signature object with the document path
            with sg.Signature('input.xlsx') as signature:

                # Use BarcodeSignOptions to add a barcode to the document
                options = sg.BarcodeSignOptions('Business data')

                # Set the barcode type and configure its properties
                options.EncodeType = sg.BarcodeTypes.Code128
                options.Left = 50
                options.Top = 150

                # Save the signed document
                result = signature.Sign('output.xlsx', options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Enhance your documents with advanced signature features"
  description: "The GroupDocs.Signature for Python via .NET library provides comprehensive solutions for signing and processing documents in commonly used formats. You can easily add, modify, verify, or remove various signature types to fit your needs."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Key Features of GroupDocs.Signature"
  features:
    # feature loop
    - title: "Flexible document signing"
      content: "Sign any page in supported documents with text, images, barcodes, QR codes, or stamps. Add hidden metadata like EXIF data in images and ensure content protection with digital certificates to prevent unauthorized changes."

    # feature loop
    - title: "Search and verify signatures"
      content: "Our tool ensures the integrity of your documents by enabling signature verification. You can also retrieve a full list of all signatures in a document for easy management."

    # feature loop
    - title: "Edit signatures easily"
      content: "Modify existing signatures effortlessly. Adjust text, reposition elements, or change colors to suit your document's needs."

    # feature loop
    - title: "Effortlessly remove signatures"
      content: "With full CRUD functionality, GroupDocs.Signature for Python via .NET makes it easy to remove any unwanted or outdated signatures from your documents."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Customize and add a barcode signature"
      content: |
        This example demonstrates how to insert a custom barcode into a XLSX document.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Provide the document to be signed
              with sg.Signature('input.xlsx') as signature:

                  # Set the barcode text and signature options
                  options = sg.BarcodeSignOptions('Accepted')
                  options.EncodeType = sg.BarcodeTypes.Code39FullASCII

                  # Choose the position for the barcode on the page
                  options.VerticalAlignment = sg.VerticalAlignment.Top
                  options.HorizontalAlignment = sg.HorizontalAlignment.Left

                  # Set padding between the barcode and page edge
                  options.Margin = sg.Padding()
                  options.Margin.Top = 180
                  options.Margin.Right = 20

                  # Specify the color of the barcode bars
                  options.ForeColor = sg.Color.Red

                  # Choose the font style for the barcode message
                  options.Font = sg.SignatureFont()
                  options.Font.Size = 12
                  options.Font.FamilyName = 'Arial'

                  # Set the position of the message text
                  options.CodeTextAlignment = sg.CodeTextAlignment.Above

                  # Sign and save the document
                  result = signature.Sign('output.xlsx', options)
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
            link: "/examples/signature/formats/signature_barcode.xlsx"
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
    title: "Explore our key features"
    exclude: "barcode"
    description: "We offer a wide array of signature options and operations for your document needs."
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
    title: "Sign documents in multiple formats"
    exclude: "XLSX"
    description: "The Python via .NET API supports signing more than 60 file formats, allowing you to add various types of signatures to any page or specific location within your documents."
    items: 
          
        # format loop 1
        - name: "Add barcode to PDF"
          format: "PDF"
          link: "/signature/python-net/barcode/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Add barcode to DOCX"
          format: "DOCX"
          link: "/signature/python-net/barcode/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Add barcode to JPEG"
          format: "JPEG"
          link: "/signature/python-net/barcode/jpeg/"
          description: "JPEG Image"
          
        # format loop 4
        - name: "Add barcode to PPTX"
          format: "PPTX"
          link: "/signature/python-net/barcode/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "Add barcode to XLSX"
          format: "XLSX"
          link: "/signature/python-net/barcode/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---