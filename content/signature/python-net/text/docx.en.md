



---
############################# Static ############################
layout: "format"
date:  2024-10-08T10:48:34
draft: false
lang: en
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Add text signatures to DOCX using Python"
head_description: "Leverage the Python API to embed text-based signatures in DOCX files, supporting formats like PDF, Word, Excel, PowerPoint, images, and ZIP."

############################# Header ############################
title: "Easily add text signatures to DOCX" 
description: "Seamlessly integrate custom text signatures into your documents using GroupDocs.Signature for Python via .NET. Simplify your workflows with flexible signature customization options."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Try it free today"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Explore the power of GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) offers a comprehensive platform for embedding customizable text signatures, making document workflows smoother. Personalize the content and appearance of signatures across documents to boost efficiency and enhance document management.

############################# Steps ############################
steps:
    enable: true
    title: "How to create DOCX text signatures with Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) enables easy text signature integration in DOCX files within Python via .NET applications. Quickly add functionality to your products with this solution.
      
      1. Provide the DOCX document to the Signature constructor.
      2. Create TextSignOptions with your signature text.
      3. Set the visual properties of the signature.
      4. Insert the signature onto the desired pages of the document.
   
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

            # Initialize the Signature with the document path
            with sg.Signature('input.docx') as signature:

                # Set up TextSignOptions with your desired signature text
                options = sg.TextSignOptions("Approved")

                # Choose the color and font for the signature
                options.ForeColor = sg.Color.Red
                options.Font = sg.SignatureFont()
                options.Font.Size = 12
                options.Font.FamilyName = "Comic Sans MS"

                # Apply the text signature to the document
                result = signature.Sign("output.docx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Complete text signature management"
  description: "GroupDocs.Signature for Python via .NET helps you manage document workflows by adding custom text signatures to popular formats. Easily control the look, placement, and content of signatures to suit your needs."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "Discover GroupDocs.Signature Features"
  features:
    # feature loop
    - title: "Flexible document signatures"
      content: "Add various signature types—text, images, barcodes, QR codes, and stamps—to any document page. Use metadata to include hidden information and secure your files with digital certificates."

    # feature loop
    - title: "Verify and search signatures"
      content: "Use advanced tools to check the integrity of your signed documents. Search and analyze all signatures in a file for further validation."

    # feature loop
    - title: "Edit or remove signatures"
      content: "Easily update the content, appearance, or placement of existing signatures. Remove outdated signatures to keep your documents current."

    # feature loop
    - title: "Specialized text signatures"
      content: "Apply document-specific text signatures, like watermarks for Word files or stamps for PDFs, adding an extra level of control and customization."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Add text signatures to documents"
      content: |
        Learn how to embed text signatures into documents to streamline your processes.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Select the document to sign
              with sg.Signature('input.docx') as signature:

                    # Set up text options with the desired content
                    options = sg.TextSignOptions("Rescheduled to 03/04/2025")

                    # Define the size and placement of the signature
                    options.Left = 100
                    options.Top = 180
                    options.Width = 230
                    options.Height = 30

                    # Set padding from page edges
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # Choose text color and font style
                    options.ForeColor = sg.Color.Red
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # Add a border around the text signature
                    options.Border = sg.Border()
                    options.Border.Color = sg.Color.Red
                    options.Border.DashStyle = sg.DashStyle.DashLongDashDot
                    options.Border.Transparency = 0.5
                    options.Border.Visible = True
                    options.Border.Weight = 2

                    # Customize the background if needed
                    options.Background = sg.Background()
                    options.Background.Color = sg.Color.Yellow
                    options.Background.Transparency = 0.8

                    # Optionally save the signature as an image for compatibility
                    options.SignatureImplementation = sg.TextSignatureImplementation.Image

                    # Save the document with the embedded signature
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
            link: "/examples/signature/formats/signature_text.docx"
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
    title: "Advanced signature features"
    exclude: "text"
    description: "Our API supports complete lifecycle management for seven signature types, allowing you to create, manage, verify, and customize your signatures with ease."
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
    title: "Embed text signatures in multiple formats"
    exclude: "DOCX"
    description: "With the Python via .NET API, you can add text signatures to various Office documents, giving you full control over the document lifecycle and improving security."
    items: 
          
        # format loop 1
        - name: "PDF text signatures"
          format: "PDF"
          link: "/signature/python-net/text/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "DOCX text signatures"
          format: "DOCX"
          link: "/signature/python-net/text/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "JPEG text signatures"
          format: "JPEG"
          link: "/signature/python-net/text/jpeg/"
          description: "JPEG Image"
          
        # format loop 4
        - name: "PPTX text signatures"
          format: "PPTX"
          link: "/signature/python-net/text/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "XLSX text signatures"
          format: "XLSX"
          link: "/signature/python-net/text/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---