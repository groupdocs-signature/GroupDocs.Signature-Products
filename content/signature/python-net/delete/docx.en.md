



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:20
draft: false
lang: en
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Remove signatures from DOCX using Python"
head_description: "Effortlessly remove digital, barcode, text, image, and metadata signatures from DOCX documents with GroupDocs.Signature for Python via .NET."

############################# Header ############################
title: "Easily remove signatures from DOCX" 
description: "In addition to signing documents, GroupDocs.Signature for Python via .NET provides a complete toolkit to locate and delete various types of signatures from your files."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Free Download"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "What is GroupDocs.Signature for Python via .NET?"
    link: "/signature/python-net/"
    link_title: "Learn more"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) is a powerful solution for managing signatures of all types, including text, images, barcodes, digital certificates, and stamps. Supporting more than 60 different formats like PDF, MS Office documents, images, and ZIP files, it offers maximum flexibility in document handling. You can easily add, verify, update, or remove signatures as needed.

############################# Steps ############################
steps:
    enable: true
    title: "Steps to delete e-signatures from DOCX using Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) allows Python via .NET developers to remove electronic signatures from DOCX files by following these simple steps:
      
      1. Load the DOCX document into the Signature class instance.
      2. Use the Search function to find all signatures in the document.
      3. Delete one or more of the found signatures.
      4. Review the results after processing.
   
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

            # Pass the document with signatures to the Signature instance
            with sg.Signature('input.docx') as signature:

                # Retrieve the list of digital signatures in the document
                options = sg.DigitalSearchOptions()

                signatures = signature.Search(options)

                # Remove the first signature from the list
                digitalSignature = signatures[0]
                result = signature.Delete(digitalSignature)

                # Process and verify the deletion results
                if result:
                    print("\nDigital signature in DOCX was deleted successfully")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Streamline document management with advanced signature features"
  description: "GroupDocs.Signature for Python via .NET is expertly designed to enhance the process of adding, verifying, editing, and deleting signatures in key business document formats."
  image: "/img/signature/features_delete.webp" # 500x500 px
  image_description: "Key Features of GroupDocs.Signature"
  features:
    # feature loop
    - title: "Sign your documents"
      content: "Quickly apply text, image, barcode, QR code, or stamp signatures to any page. Additionally, you can manage hidden metadata like EXIF in images and ensure document integrity with digital certificates."

    # feature loop
    - title: "Find and verify signatures"
      content: "Use our powerful tools to locate and verify the signatures in your documents, giving you a complete list of all signatures for thorough management."

    # feature loop
    - title: "Edit signatures"
      content: "Easily modify existing signatures by changing the text, repositioning elements, or adjusting colors to match your preferences."

    # feature loop
    - title: "Delete unwanted signatures"
      content: "Take full control of document signatures with complete create, read, update, and delete (CRUD) operations, allowing you to remove any signature type when needed."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Remove all barcode signatures"
      content: |
        Learn how to delete all barcode signatures from a document.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Provide a document containing barcode signatures
              with sg.Signature('input.docx') as signature:

                    # Remove all barcode signatures
                    result = signature.Delete(SignatureType.Barcode)

                    # Check the results of the deletion process
                    if result.Succeeded.Count > 0:
                        print("\n DOCX barcode signatures were deleted") 
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
    title: "Discover our key features"
    exclude: "delete"
    description: "Explore a wide range of signature types and operations available with our solution."
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
          description: "Generate and QR Codes, including QR codes, for document signing"
          
        # operation loop 6
        - name: "Digital certificates"
          operation: "digital"
          link: "/signature/python-net/digital/docx/"
          description: "Secure business and sign documents with digital certificates"

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
    title: "Delete signatures from multiple file formats"
    exclude: "DOCX"
    description: "GroupDocs.Signature for Python via .NET is built to support signature removal from over 60 different file formats, ensuring compatibility and ease of use."
    items: 
          
        # format loop 1
        - name: "Delete PDF signatures"
          format: "PDF"
          link: "/signature/python-net/delete/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Remove DOCX signatures"
          format: "DOCX"
          link: "/signature/python-net/delete/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 3
        - name: "Delete PPTX signatures"
          format: "PPTX"
          link: "/signature/python-net/delete/pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 4
        - name: "Delete XLSX signatures"
          format: "XLSX"
          link: "/signature/python-net/delete/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"


          

---