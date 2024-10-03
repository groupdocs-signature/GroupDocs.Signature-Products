



---
############################# Static ############################
layout: "format"
date:  2024-10-03T12:32:58
draft: false
lang: en
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Create Round and square stamps in DOCX using Python"
head_description: "Generate and insert personalized stamps into DOCX files with the GroupDocs.Signature for Python via .NET API."

############################# Header ############################
title: "Create stamps for DOCX" 
description: "Easily add custom-designed stamps to any part of your documents with GroupDocs.Signature for Python via .NET, offering great flexibility for placement and configuration to meet your business needs."
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
    title: "Overview of GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) is a comprehensive tool that lets you insert various signature types into documents, including custom stamps. Supporting over 60 file formats—from PDFs and Word docs to images and ZIP files—you can enhance your documents with text, image, barcode, metadata, digital certificates, and stamps. You also have full control to search, verify, edit, or delete any applied signatures.

############################# Steps ############################
steps:
    enable: true
    title: "How to add a stamp to DOCX using Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) provides robust stamp creation tools for enhancing Python via .NET applications. Use it to design and implement custom stamps for your document pages.
      
      1. Provide the DOCX document you want to stamp.
      2. Use StampSignOptions to configure all necessary settings.
      3. Add multiple stamp lines if required.
      4. Apply the stamp and save the updated document.
   
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

            # Attach the document path to the Signature instance
            with sg.Signature('input.docx') as signature:

                # Set up StampSignOptions with the required stamp details
                options = sg.StampSignOptions()

                # Add one or more lines to the stamp
                outerLine = sg.StampLine()
                outerLine.Text = "* European Union *"
                outerLine.TextRepeatType = sg.StampTextRepeatType.FullTextRepeat
                outerLine.Font = sg.SignatureFont()
                outerLine.Font.Size = 12
                outerLine.Font.FamilyName = "Arial"
                outerLine.Height = 22
                outerLine.TextBottomIntent = 6
                outerLine.TextColor = sg.Color.WhiteSmoke
                outerLine.BackgroundColor = sg.Color.DarkSlateBlue
                options.OuterLines.Add(outerLine)

                # Save the document with the applied stamp
                result = signature.Sign("output.docx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Use signatures to secure and improve document integrity"
  description: "With the GroupDocs.Signature for Python via .NET library, you can seamlessly add signature functionality to your documents. Easily create, modify, verify, or delete custom stamps and other signature types, providing flexibility and security for your document workflows."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Stamp Signatures Powered by GroupDocs.Signature"
  features:
    # feature loop
    - title: "Complete document signing"
      content: "Elevate your documents by adding signatures like text, images, barcodes, QR codes, and stamps to any position on any page. Manage embedded metadata and apply digital certificates to protect against unauthorized changes."

    # feature loop
    - title: "Efficient signature search and verification"
      content: "After signing, use advanced search tools to find all embedded signatures. Easily verify or manage signature data to ensure document integrity."

    # feature loop
    - title: "Edit and customize signatures"
      content: "Make changes to previously added signatures with ease. Whether you want to change the content, position, size, or color, GroupDocs.Signature for Python via .NET gives you full control to adjust signatures as needed."

    # feature loop
    - title: "Easily remove signatures"
      content: "If you need to remove signatures, GroupDocs.Signature for Python via .NET offers all the tools necessary to delete any type, including stamps and digital certificates, helping you keep your documents up-to-date and compliant."
      
  code_samples:
    # code sample loop
    - title: "How to add custom stamps to documents"
      content: |
        This example shows how to create and insert custom stamps with specific text details into a document.
        {{< landing/code title="C#">}}
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Provide the document you want to stamp
            with sg.Signature('input.docx') as signature:

                # Set up the stamp options with your desired settings
                options = sg.StampSignOptions()

                # Define the stamp’s size and placement on the page
                options.Height = 300
                options.Width = 300
                options.VerticalAlignment = sg.VerticalAlignment.Center
                options.HorizontalAlignment = sg.HorizontalAlignment.Left
                options.AllPages = True

                # Add outer circular lines with text
                outerLine = sg.StampLine()
                outerLine.Text = "* The best choice *"
                outerLine.TextRepeatType = sg.StampTextRepeatType.FullTextRepeat
                outerLine.Font = sg.SignatureFont()
                outerLine.Font.Size = 12
                outerLine.Font.FamilyName = "Arial"
                outerLine.Height = 22
                outerLine.TextBottomIntent = 6
                outerLine.TextColor = sg.Color.WhiteSmoke
                outerLine.BackgroundColor = sg.Color.DarkSlateBlue
                options.OuterLines.Add(outerLine)

                # Optionally, add inner square lines
                innerLine = sg.StampLine()
                innerLine.Text = "Company #1"
                innerLine.TextColor = sg.Color.MediumVioletRed
                innerLine.Font = sg.SignatureFont()
                innerLine.Font.Size = 20
                innerLine.Font.Bold = True
                innerLine.Height = 40
                options.InnerLines.Add(innerLine)

                # Finalize and save the stamped document
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
    title: "Explore key features"
    exclude: "stamp"
    description: "Find a wide range of options for creating, managing, and removing signatures, giving you complete control over document workflows."
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
    title: "Apply stamps to various document formats"
    exclude: "DOCX"
    description: "With GroupDocs.Signature API, you can insert custom stamps into more than 60 standard file types. Easily apply stamps anywhere in your documents, improving personalization and tracking."
    items: 
          
        # format loop 1
        - name: "Stamp PDF"
          format: "PDF"
          link: "/signature/python-net/stamp/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Stamp DOCX"
          format: "DOCX"
          link: "/signature/python-net/stamp/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Stamp JPEG"
          format: "JPEG"
          link: "/signature/python-net/stamp/jpeg/"
          description: "JPEG Image"
          
        # format loop 4
        - name: "Stamp PPTX"
          format: "PPTX"
          link: "/signature/python-net/stamp/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 5
        - name: "Stamp XLSX"
          format: "XLSX"
          link: "/signature/python-net/stamp/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---