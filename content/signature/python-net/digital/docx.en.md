



---
############################# Static ############################
layout: "format"
date:  2024-09-26T16:11:09
draft: false
lang: en
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Apply digital signatures to DOCX using Python"
head_description: "Digitally sign DOCX documents using Python in just a few lines of code. Use GroupDocs.Signature for Python via .NET to sign a wide range of file formats."

############################# Header ############################
title: "Digitally sign DOCX" 
description: "Ensure the security and authenticity of your documents by applying digital certificates through GroupDocs.Signature for Python via .NET. Our solution allows you to easily sign and safeguard your documents with powerful tools."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Get it for free"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "What is GroupDocs.Signature for Python via .NET?"
    link: "/signature/python-net/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) is a comprehensive signing tool that supports a wide array of document processing tasks. It allows you to add text, images, digital certificates, and stamps to over 60 file formats—including PDFs, MS Office files, images, and ZIPs. With GroupDocs.Signature for Python via .NET, you can also search for, verify, update, or remove signatures whenever needed.

############################# Steps ############################
steps:
    enable: true
    title: "How to protect DOCX with digital certificates in Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) helps Python via .NET developers secure DOCX files by adding digital signatures. Strengthen your business applications with robust document protection features.
      
      1. Load the DOCX file into the Signature class.
      2. Apply a digital certificate and its password to secure the file.
      3. Optionally, add a visual display of the digital signature on the document pages.
      4. Sign the document to prevent unauthorized changes.
   
    code:
      platform: "net"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/signature_all.pdf"
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

            # Use Signature to digitally sign the document
            with sg.Signature('input.docx') as signature:

                # Input the digital certificate and its password
                options = sg.DigitalSignOptions("certificate.pfx")
                options.Password = "1234567890"

                # Optionally configure how the signature will look
                options.PageNumber = 1
                options.Left = 50
                options.Top = 50

                # Finalize the document with the digital certificate
                result = signature.Sign("output.docx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Enhance and secure documents with digital signatures"
  description: "The GroupDocs.Signature for Python via .NET library is designed to sign all major file formats. Simplify your workflow by easily adding, verifying, updating, or removing different types of signatures."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Core Features of GroupDocs.Signature"
  features:
    # feature loop
    - title: "Add signatures to your documents"
      content: "Insert text, image, barcode, QR code, or stamp signatures precisely anywhere in supported documents. You can also manage hidden metadata, like EXIF in images, to ensure document integrity with digital signatures."

    # feature loop
    - title: "Verify and search signatures"
      content: "After signing, you can easily verify documents to ensure correct processing. Retrieve and manage all signatures within your files with powerful search capabilities."

    # feature loop
    - title: "Edit existing signatures"
      content: "Most signatures can be fully customized. You can edit text, move elements, change colors, adjust sizes, and more to fit your needs."

    # feature loop
    - title: "Remove unnecessary signatures"
      content: "Our solution supports complete signature management, allowing you to delete signatures, including digital certificates, from any document when needed."
      
  code_samples:
    # code sample loop
    - title: "Protect documents with digital signatures"
      content: |
        Learn how to secure your documents by applying digital signatures to prevent unauthorized modifications.
        {{< landing/code title="C#">}}
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Load the document to be signed
            with sg.Signature('input.docx') as signature:

                # Use a valid digital certificate with its corresponding password
                options = sg.DigitalSignOptions("certificate.pfx")
                options.Password = "1234567890"

                # Add any additional text information if needed
                options.Reason = "Security issue"
                options.Contact = "John Smith"
                options.Location = "Office D.W."

                # Include an image or other options for visual representation of the signature
                options.ImageFilePath = "image.png"
                options.AllPages = True
                options.VerticalAlignment = sg.VerticalAlignment.Center
                options.HorizontalAlignment = sg.HorizontalAlignment.Left
                options.Width = 60
                options.Height = 80

                options.Margin = sg.Padding()
                options.Margin.Bottom = 10
                options.Margin.Right = 10

                # Save the signed document in a secure location
                result = signature.Sign("output.docx", options)
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
    title: "Explore our key features"
    exclude: "digital"
    description: "We offer a broad range of signature options and powerful document operations."
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
    title: "Sign documents across multiple formats"
    exclude: "DOCX"
    description: "With Python via .NET API, you can process over 60 different formats, adding signatures, applying digital certificates for security, and managing signatures across various pages."
    items: 
          
        # format loop 1
        - name: "Protect PDF"
          format: "PDF"
          link: "/signature/python-net/digital/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Protect DOCX"
          format: "DOCX"
          link: "/signature/python-net/digital/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Protect PPTX"
          format: "PPTX"
          link: "/signature/python-net/digital/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Protect XLSX"
          format: "XLSX"
          link: "/signature/python-net/digital/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---