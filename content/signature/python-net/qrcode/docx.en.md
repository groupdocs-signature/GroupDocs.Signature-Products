



---
############################# Static ############################
layout: "format"
date:  2024-10-08T11:43:29
draft: false
lang: en
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Generate QR codes for DOCX files using Python"
head_description: "Use the GroupDocs.Signature API to generate and embed QR codes in DOCX files. Easily place QR codes on any page to add extra functionality."

############################# Header ############################
title: "Generate QR codes for DOCX" 
description: "Effortlessly create 2D barcodes using text or numeric data and apply them to various pages and formats, including PDFs, Word, Excel, and more with GroupDocs.Signature for Python via .NET."
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
    title: "Explore the features of GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) offers a wide range of capabilities, enabling users to generate and embed different signature types across major document formats. Whether it's PDFs, Word, Excel, PowerPoint, or images, enhance your documents with Text, Image, Barcode, QR Code, Metadata, Digital, or Stamp signatures.

############################# Steps ############################
steps:
    enable: true
    title: "Steps to generate and insert a QR code in DOCX"
    content: |
      [GroupDocs.Signature](/signature/python-net/) lets you create QR codes in popular formats and place them on DOCX pages. With support for over 10 QR code types, you can seamlessly integrate this functionality into Python via .NET applications. Enhance your documents with QR code signatures using our product.
      
      1. Obtain the DOCX file or stream where the QR code will be added.
      2. Provide the required text to QrCodeSignOptions.
      3. Customize visual settings like color, position, and size.
      4. Save the document with the embedded QR code.
   
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

            # Initialize a new Signature instance with the document
            with sg.Signature('input.docx') as signature:

                # Use QrCodeSignOptions to embed a QR code into the document
                options = sg.QrCodeSignOptions("Text Content")

                # Specify the signature type and set its position on the page
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 50
                options.Top = 150

                # Save the document with the embedded QR code
                result = signature.Sign("output.docx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Complete signature integration for documents"
  description: "With the GroupDocs.Signature for Python via .NET API, users can generate, modify, search, validate, and remove different signature types, simplifying document workflows with precision."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Key Features of GroupDocs.Signature"
  features:
    # feature loop
    - title: "Apply multiple signature types"
      content: "GroupDocs.Signature allows the application of Text, Image, Barcode, QR Code, and Stamp signatures to any document. You can precisely place signatures on any page and manage metadata easily. Protect your documents from unauthorized changes with digital certificates."

    # feature loop
    - title: "Search and validate signatures"
      content: "Verify document signatures for authenticity and accuracy using advanced validation tools. Easily get a detailed list of all signatures embedded in a document for better oversight."

    # feature loop
    - title: "Modify existing signatures"
      content: "You can update previously applied signatures by adjusting content, position, color, size, and other attributes to suit your specific needs."

    # feature loop
    - title: "Easily remove signatures"
      content: "Streamline document management by quickly removing unwanted signatures. Whether it’s a digital certificate or another signature type, removal can be done efficiently."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Customize a Generated QR Code"
      content: |
        This example shows how to place a customized QR code on a DOCX page.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Get the document to be signed and pass it to Signature
              with sg.Signature('input.docx') as signature:

                    # Configure QR code options with the required text
                    options = sg.QrCodeSignOptions("Archived on July 11, 2019")

                    # Set the QR code’s position on the page
                    options.VerticalAlignment = sg.Domain.VerticalAlignment.Top
                    options.HorizontalAlignment = sg.Domain.HorizontalAlignment.Right

                    # Set the padding for the signature
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # Choose the color of the QR code
                    options.ForeColor = sg.Color.Red

                    # Define the font options for the message
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # Set the background color and brush for the QR code
                    options.Background = sg.Background()
                    options.Background.Color = Color.LimeGreen
                    options.Background.Transparency = 0.5
                    options.Background.Brush = sg.LinearGradientBrush(sg.Color.LimeGreen, sg.Color.DarkGreen)

                    # Embed the QR code into the document
                    result = signature.Sign("output.docx", options)
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
            link: "/examples/signature/formats/signature_qrcode.docx"
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
    title: "Explore our signature solutions"
    exclude: "qrcode"
    description: "We offer a wide variety of signature types and operations to meet your document needs."
    items: 
          
        # operation loop 1
        - name: "Electronic signatures"
          operation: "esign"
          link: "/signature/python-net/esign/docx/"
          description: "Add various types of signatures to supported file formats"

        # operation loop 2
        - name: "Add text to documents"
          operation: "text"
          link: "/signature/python-net/text/docx/"
          description: "Enhance document content with customizable text signatures"

        # operation loop 3
        - name: "Image signatures"
          operation: "image"
          link: "/signature/python-net/image/docx/"
          description: "Place any image at any position within a document"

        # operation loop 4
        - name: "Generate barcodes"
          operation: "barcode"
          link: "/signature/python-net/barcode/docx/"
          description: "Create and insert various barcodes into supported documents"

        # operation loop 5
        - name: "Generate QR codes"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/docx/"
          description: "Generate and apply two-dimensional barcodes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/python-net/digital/docx/"
          description: "Secure business documents using digital certificates"

        # operation loop 7
        - name: "Stamp signatures"
          operation: "stamp"
          link: "/signature/python-net/stamp/docx/"
          description: "Use the Stamp Constructor to create custom round or square stamps"
          
        # operation loop 8
        - name: "Search signatures"
          operation: "search"
          link: "/signature/python-net/search/docx/"
          description: "Locate any previously added signatures within a document"
          
        # operation loop 9
        - name: "Signature verification"
          operation: "verify"
          link: "/signature/python-net/verify/docx/"
          description: "Verify the authenticity of signatures after they have been applied"
          
        # operation loop 10
        - name: "Modify signatures"
          operation: "modify"
          link: "/signature/python-net/modify/docx/"
          description: "Easily edit a variety of signatures within a document"
          
        # operation loop 11
        - name: "Delete signatures"
          operation: "delete"
          link: "/signature/python-net/delete/docx/"
          description: "Remove a wide range of previously applied signatures"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Embed QR codes in various document formats"
    exclude: "DOCX"
    description: "Use the Python via .NET API to embed QR codes into any industry-standard document format. Store and encode important information into 2D barcodes for easy scanning and data retrieval."
    items: 
          
        # format loop 1
        - name: "QR-Code for PDF"
          format: "PDF"
          link: "/signature/python-net/qrcode/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "QR-Code for DOCX"
          format: "DOCX"
          link: "/signature/python-net/qrcode/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "QR-Code for JPEG"
          format: "JPEG"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "JPEG Image"
          
        # format loop 4
        - name: "QR-Code for PPTX"
          format: "PPTX"
          link: "/signature/python-net/qrcode/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "QR-Code for XLSX"
          format: "XLSX"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---