



---
############################# Static ############################
layout: "format"
date:  2024-09-26T16:11:08
draft: false
lang: en
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Insert image signatures into PDF files with Python"
head_description: "Easily embed image signatures in PDF documents for Python using just a few lines of code. Utilize the GroupDocs.Signature for Python via .NET API to seamlessly add image-based signatures."

############################# Header ############################
title: "Add image signatures to PDF" 
description: "Use GroupDocs.Signature for Python via .NET to effortlessly incorporate image signatures into various office document formats, including PDF, Word, Excel, and image files. Adding an image of your manager's signature enhances professionalism, boosting both visual impact and document authenticity."
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
    title: "Explore GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) provides versatile options for embedding image signatures anywhere within your business documents. Streamline workflows by adding images to PDFs, Word documents, Excel sheets, PowerPoint presentations, and popular image formats using our powerful library.

############################# Steps ############################
steps:
    enable: true
    title: "How to insert an image signature into a PDF file using Python"
    content: |
      Use [GroupDocs.Signature](/signature/python-net/) to give Python via .NET applications the capability to accurately add image signatures anywhere in PDF documents. Easily enhance your product by integrating our solution.
      
      1. Create a Signature instance with the PDF document.
      2. Configure ImageSignOptions with the desired image for the signature.
      3. Precisely position the image at your chosen location on the document.
      4. Save the signed document to the specified location.
   
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

            # Initialize Signature with the document path
            with sg.Signature('input.pdf') as signature:

                # Set up ImageSignOptions with the chosen image for the signature
                options = sg.ImageSignOptions("boss_signature.jpg")

                # Position the image at the top-left corner of each page
                options.AllPages = True
                options.Left = 100
                options.Top = 100
                
                # Save the signed document
                result = signature.Sign("output.pdf", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Comprehensive document signing features"
  description: "Our API supports a broad range of signature functionalities. You can easily add, update, remove, search, and validate different types of signatures, including image-based signatures."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Image Signature Integration"
  features:
    # feature loop
    - title: "Insert images into office documents"
      content: "Embed electronic signatures and images at any chosen spot within a document. Enhance your documents with images, barcodes, text, metadata, or digital certificates to improve functionality and security."

    # feature loop
    - title: "Signature search and validation"
      content: "Ensure document integrity by verifying the authenticity of signatures. Retrieve a detailed list of all signatures within a document and assess their individual properties."

    # feature loop
    - title: "Edit existing signatures"
      content: "Easily update the content, appearance, size, or position of signatures within your documents to meet changing needs."

    # feature loop
    - title: "Remove unnecessary signatures"
      content: "Our API provides full control, allowing you to remove signatures from most supported file formats whenever needed."
      
  code_samples:
    # code sample loop
    - title: "Enhance documents with image signatures"
      content: |
        Learn how to embed image signatures in your business documents to enrich content.
        {{< landing/code title="C#">}}
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Choose the document to be signed
            with sg.Signature('input.pdf') as signature:

                # Set up image options with the image file path
                options = sg.ImageSignOptions("organization_seal.jpg")

                # Specify the size of the image signature
                options.Width = 100
                options.Height = 100

                # Position the image in the bottom-right corner of the page
                options.VerticalAlignment = sg.VerticalAlignment.Bottom
                options.HorizontalAlignment = sg.HorizontalAlignment.Right

                # Apply padding from the page edges as needed
                options.Margin = sg.Padding()
                options.Margin.Bottom = 120
                options.Margin.Right = 120

                # Optionally, add a border around the image
                options.Border = sg.Border()
                options.Border.Visible = True
                options.Border.Color = sg.Color.OrangeRed
                options.Border.DashStyle = sg.DashStyle.DashDotDot
                options.Border.Weight = 5

                # Rotate the image to ensure proper alignment
                options.RotationAngle = 45

                # Save the updated document
                result = signature.Sign("output.pdf", options)
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
    title: "Explore our features"
    exclude: "image"
    description: "Discover the different signature types and operations our platform offers."
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
    title: "Embed images in multiple file formats"
    exclude: "PDF"
    description: "Use the Python via .NET API to insert images into various document formats. Easily resize, position, select specific pages, and apply image-based signatures, giving you complete control over your document's layout."
    items: 
          
        # format loop 1
        - name: "Sign PDF with image"
          format: "PDF"
          link: "/signature/python-net/image/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Sign DOCX with image"
          format: "DOCX"
          link: "/signature/python-net/image/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Sign JPEG with image"
          format: "JPEG"
          link: "/signature/python-net/image/jpeg/"
          description: "JPEG Image"
          
        # format loop 4
        - name: "Sign PPTX with image"
          format: "PPTX"
          link: "/signature/python-net/image/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "Sign XLSX with image"
          format: "XLSX"
          link: "/signature/python-net/image/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---