---
############################# Static ############################
layout: "landing"
date: 2024-09-25T12:45:24
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
      tag: "python-net" 
    # supported_platforms loop
    - title: "Python"
      tag: "python-net" 

############################# Head ############################
head_title: "{index-content-python-net.head_title}"
head_description: "{index-content-python-net.head_description}"

############################# Header ############################
title: "{index-content-python-net.title}"
description: "{index-content-python-net.description}"
words:
  for: "for"

actions:
  main: "{index-content-python-net.actions_main}"
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
  title: "{index-content-python-net.code_title}"
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
  description: "{index-content-python-net.overview_description}"
  features:
    # feature loop
    - title: "{index-content-python-net.overview_feature_1.title}"
      content: "{index-content-python-net.overview_feature_1.description}"

    # feature loop
    - title: "{index-content-python-net.overview_feature_2.title}"
      content: "{index-content-python-net.overview_feature_2.description}"

    # feature loop
    - title: "{index-content-python-net.overview_feature_3.title}"
      content: "{index-content-python-net.overview_feature_3.description}"

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform independence"
  description: "{index-content-python-net.platforms_description}"
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
    {index-content-python-net.formats_description}
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
  title: "{index-content-python-net.features.title}"
  description: "{index-content-python-net.features.description}"

  items:
    # feature loop
    - icon: "sign"
      title: "{index-content-python-net.features.feature_1.title}"
      content: "{index-content-python-net.features.feature_1.content}"

    # feature loop
    - icon: "custom"
      title: "{index-content-python-net.features.feature_2.title}"
      content: "{index-content-python-net.features.feature_2.content}"

    # feature loop
    - icon: "password"
      title: "{index-content-python-net.features.feature_3.title}"
      content: "{index-content-python-net.features.feature_3.content}"

    # feature loop
    - icon: "protect"
      title: "{index-content-python-net.features.feature_4.title}"
      content: "{index-content-python-net.features.feature_4.content}"

    # feature loop
    - icon: "convert"
      title: "{index-content-python-net.features.feature_5.title}"
      content: "{index-content-python-net.features.feature_5.content}"

    # feature loop
    - icon: "preview"
      title: "{index-content-python-net.features.feature_6.title}"
      content: "{index-content-python-net.features.feature_6.content}"

    # feature loop
    - icon: "search"
      title: "{index-content-python-net.features.feature_7.title}"
      content: "{index-content-python-net.features.feature_7.content}"

    # feature loop
    - icon: "validate"
      title: "{index-content-python-net.features.feature_8.title}"
      content: "{index-content-python-net.features.feature_8.content}"

    # feature loop
    - icon: "update"
      title: "{index-content-python-net.features.feature_9.title}"
      content: "{index-content-python-net.features.feature_9.content}"

############################# Code samples ############################
code_samples:
  enable: true
  title: "Code samples"
  description: "{index-content-python-net.code_samples_description}"
  items:
    # code sample loop
    - title: "{index-content-python-net.code_title_sample_1}"
      content: |
        {index-content-python-net.code_samples_sample_1_content_1} {index-content-python-net.code_samples_sample_1_content_2}
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
    - title: "{index-content-python-net.code_title_sample_2}"
      content: |
        {index-content-python-net.code_samples_sample_2_content_1} {index-content-python-net.code_samples_sample_2_content_2}
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
