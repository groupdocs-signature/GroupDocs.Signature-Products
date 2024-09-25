---
############################# Static ############################
layout: "landing"
date: 2024-09-25T13:59:03
draft: false

lang: en
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java" 
    # supported_platforms loop
    - title: "Python"
      tag: "python-net"  

############################# Head ############################
head_title: "Python Digital Signature API - GroupDocs.Signature"
head_description: "Easily integrate secure e-signatures into Python applications using GroupDocs.Signature. Simplify and streamline your document signing workflows with minimal effort."

############################# Header ############################
title: "Sign Documents with Python API"
description: "Digitally sign documents and images across platforms with our flexible APIs, built for developers and end-users alike."
words:
  for: "for"

actions:
  main: "Download from PyPI"
  main_link: "https://pypi.org/project/groupdocs-signature-net/"
  alt: "Licensing"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
  title: "Ready to get started?"
  description: "Try GroupDocs.Signature features for free or request a license"

release:
  title: "Version {0} released"
  notes: "See what’s new"
  downloads: "Downloads"

code:
  title: "Signing PDFs with Python"
  more: "More examples"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
  install: "pip install groupdocs-signature-net"
  content: |
    ```python {style=abap}   
    import groupdocs.signature as sg

    def run():

        # Select PDF document
        with sg.Signature('sample.pdf') as signature:

            # Provide text
            options = sg.TextSignOptions("John Smith")
    
            # Set color
            options.ForeColor = sg.Color.Red
    
            # Sign document and save to file
            signature.Sign('signed.pdf', options)
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Overview"
  description: "A powerful document signing library designed for use in Python applications."
  features:
    # feature loop
    - title: "Comprehensive Digital Signatures for Business Documents in Python"
      content: "GroupDocs.Signature for Python via .NET provides a wide range of digital signature options, including text, barcodes, images, digital certificates, and metadata for PDFs, Office documents, and images. The solution is optimized for efficient document processing."

    # feature loop
    - title: "Advanced Document Processing"
      content: "GroupDocs.Signature allows you to manage signed documents by searching and validating signatures based on multiple criteria. You can also extract detailed document data or generate page previews."

    # feature loop
    - title: "Flexible Output Formats"
      content: "Our API gives you control over the final format of signed documents, enabling precise positioning of signatures, customization of their appearance, and saving in a variety of formats. Optionally, you can secure documents with passwords."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform independence"
  description: "GroupDocs.Signature for Python via .NET works seamlessly across various operating systems."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Supported file formats"
  description: |
    GroupDocs.Signature for Python via .NET supports operations for a wide range of popular file formats. Learn more [here](https://docs.groupdocs.com/signature/python-net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office formats
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Images & Other Formats
        * **Portable:** PDF
        * **Images:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Other office formats:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Other formats
        * **Web:** HTML, MHTML
        * **Archives:** ZIP, TAR, 7Z
        * **Certificates:** PFX

############################# Features ############################
features:
  enable: true
  title: "Key Features of GroupDocs.Signature"
  description: "Sign PDFs, Office documents, and images with ease using digital signatures."

  items:
    # feature loop
    - icon: "sign"
      title: "Business Signatures"
      content: "Use a variety of signature types to sign documents and place them on any page in the desired location."

    # feature loop
    - icon: "custom"
      title: "Customizable Signature Appearance"
      content: "Easily customize the look of your signatures, including color, font, borders, rotation, and more, to match your needs."

    # feature loop
    - icon: "password"
      title: "Password Protection"
      content: "Add an extra layer of security to signed documents by protecting them with passwords."

    # feature loop
    - icon: "protect"
      title: "Prevent Unauthorized Changes"
      content: "Ensure that important business documents are protected from unauthorized modifications by using digital certificates."

    # feature loop
    - icon: "convert"
      title: "Flexible Output Formats"
      content: "Generate signed documents in multiple formats. Convert Word documents to PDFs seamlessly."

    # feature loop
    - icon: "preview"
      title: "Document Previews"
      content: "Save individual document pages as images for later use."

    # feature loop
    - icon: "search"
      title: "Signature Search"
      content: "Easily find and retrieve information about any previously added signatures in your documents."

    # feature loop
    - icon: "validate"
      title: "Document Validation"
      content: "Verify the authenticity of signatures in any document to ensure integrity."

    # feature loop
    - icon: "update"
      title: "Manage Signatures"
      content: "Easily delete, move, or edit signatures on any page of the document."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Code samples"
  description: "Here are some code examples that demonstrate typical GroupDocs.Signature for Python via .NET operations."
  items:
    # code sample loop
    - title: "Add QR Codes to a PDF"
      content: |
        Integrating [QR codes](https://docs.groupdocs.com/signature/python-net/find-signature-properties/) into specific pages of a PDF can help streamline your business processes. This example shows how to add a QR code using GroupDocs.Signature for Python via .NET in Python.
        {{< landing/code title="How to put QR code to PDF.">}}
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Load the document to sign
            with sg.Signature('file_to_sign.pdf') as signature:

                # Create QR code options with predefined text
                options = sg.QrCodeSignOptions('The document is approved by John Smith')
        
                # Configure QR code encoding type and position on the page
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 100
                options.Top = 100
            
                # Sign the document and save it as the result file
                signature.Sign('file_with_QR.pdf', options)
        ```
        {{< /landing/code >}}

    # code sample loop
    - title: "Protect a DOCX with a Digital Signature"
      content: |
        [Protect your documents](https://docs.groupdocs.com/signature/python-net/adding-signature/) with signatures based on digital certificates. Digital signatures safeguard your business documents from unauthorized changes.
        {{< landing/code title="Here is how to ensure document integrity.">}}
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Load the document to be digitally signed
            with sg.Signature('file_to_sign.docx') as signature:
        
                # Specify digital signing options and provide the path to the certificate file
                options = sg.DigitalSignOptions('certificate.pfx')

                # Set the certificate password
                options.Password = '1234567890'

                # Sign the document and save it to the desired path
                signature.Sign('digitally_signed.docx', options)
        ```
        {{< /landing/code >}}

---
