---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:24+03:00
draft: false

############################# Head ############################
head_title: "Sign XLSX files with JPG Image Signatures in C# .NET"
head_description: "Add JPG image signatures to digitally sign XLSX documents in C# .NET - add customized electronic signatures to popular business documents and image file formats."

############################# Header ############################
title: "Add Image Signatures to XLSX Files in .NET"
description: "Digitally sign your XLSX files using JPG and other popular image signature types. Manipulate signature properties and set up advance signing options within documents that suit your needs."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download Free Trial"
    link: "https://downloads.groupdocs.com/signature/net"

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"

    middle:
        button:

            # button loop
            - link: "https://apireference.groupdocs.com/signature/net"
              text: "API Reference"

            # button loop
            - link: "https://github.com/groupdocs-signature"
              text: "Code Examples"

            # button loop
            - link: "https://products.groupdocs.app/signature/family"
              text: "Live Demos"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/net"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/net"
        link_buy: "https://purchase.groupdocs.com"

############################# About ############################
about:
    enable: true
    title: "About GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net) is a native .NET API to electronically sign digital documents using various signature types such as text, image, barcode, stamp, form-field, QR-code and metadata. Users can add, edit, verify, delete and search digital signatures within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats with additional support for customizing signature properties as needed.

############################# Steps ############################
steps:
    enable: true
    title_left: "How to Add Image Signatures to XLSX"
    content_left: |
        [GroupDocs.Signature](https://products.groupdocs.com/signature/net) makes it easy for .NET developers to add image signatures to XLSX files within their applications by implementing a few easy steps.

        *   Create new instance of Signature class and pass source document path as a constructor parameter.
        *   Instantiate the ImageSignOptions object according to your requirements and specify Image signature options.
        *   Call Sign method of Signature class instance and pass ImageSignOptions to it.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installled on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```cs
        using (Signature signature = new Signature("sample.xlsx"))
        {
            ImageSignOptions options = new ImageSignOptions("signature.jpg")
            {
                // set signature position
                Left = 100,
                Top = 100,
                AllPages = true                
            };
            signature.Sign("SampleSigned.xlsx", options);
        }
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Live Demos - Online App to Add Digital Signatures"
    content: |
        Add signatures to XLSX files right now by visiting [GroupDocs.Signature Live Demos](https://products.groupdocs.app/signature/family) website.  
        The live demo has the following benefits
        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-excel-o"
          title: "About XLSX File Format"
          content: |
            XLSX is well-known format for Microsoft Excel documents that was introduced by Microsoft with the release of Microsoft Office 2007. Based on structure organized according to the Open Packaging Conventions as outlined in Part 2 of the OOXML standard ECMA-376, the new format is a zip package that contains a number of XML files. The underlying structure and files can be examined by simply unzipping the .xlsx file.

          link: "https://docs.fileformat.com/spreadsheet/xlsx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Signing Other Digital Document Formats"
    content: |
        .NET digital signatures management API for documents and images. Add image signatures to some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Add image signatures to PDF"
          link: "https://products.groupdocs.com/signature/net/add/jpg/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Add image signatures to DOC"
          link: "https://products.groupdocs.com/signature/net/add/jpg/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Add image signatures to DOCM"
          link: "https://products.groupdocs.com/signature/net/add/jpg/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Add image signatures to DOCX"
          link: "https://products.groupdocs.com/signature/net/add/jpg/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Add image signatures to DOT"
          link: "https://products.groupdocs.com/signature/net/add/jpg/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Add image signatures to DOTX"
          link: "https://products.groupdocs.com/signature/net/add/jpg/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Add image signatures to DOTM"
          link: "https://products.groupdocs.com/signature/net/add/jpg/dotm/"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Add image signatures to RTF"
          link: "https://products.groupdocs.com/signature/net/add/jpg/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Add image signatures to ODT"
          link: "https://products.groupdocs.com/signature/net/add/jpg/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Add image signatures to OTT"
          link: "https://products.groupdocs.com/signature/net/add/jpg/ott/"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Add image signatures to XLS"
          link: "https://products.groupdocs.com/signature/net/add/jpg/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Add image signatures to XLSX"
          link: "https://products.groupdocs.com/signature/net/add/jpg/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Add image signatures to XLSM"
          link: "https://products.groupdocs.com/signature/net/add/jpg/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Add image signatures to XLSM"
          link: "https://products.groupdocs.com/signature/net/add/jpg/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Add image signatures to XLSB"
          link: "https://products.groupdocs.com/signature/net/add/jpg/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Add image signatures to XLTX"
          link: "https://products.groupdocs.com/signature/net/add/jpg/xltx/"
          description: "Microsoft Excel template"

        # format loop
        - name: "Add image signatures to XLTM"
          link: "https://products.groupdocs.com/signature/net/add/jpg/xltm/"
          description: "Microsoft Excel macro-enabled template"

        # format loop
        - name: "Add image signatures to ODS"
          link: "https://products.groupdocs.com/signature/net/add/jpg/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Add image signatures to OTS"
          link: "https://products.groupdocs.com/signature/net/add/jpg/ots/"
          description: "OpenDocument Spreadsheet Template"

        # format loop
        - name: "Add image signatures to PPT"
          link: "https://products.groupdocs.com/signature/net/add/jpg/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Add image signatures to PPTX"
          link: "https://products.groupdocs.com/signature/net/add/jpg/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Add image signatures to PPS"
          link: "https://products.groupdocs.com/signature/net/add/jpg/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Add image signatures to PPSX"
          link: "https://products.groupdocs.com/signature/net/add/jpg/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Add image signatures to POTM"
          link: "https://products.groupdocs.com/signature/net/add/jpg/potm/"
          description: "Microsoft PowerPoint Macro-Enabled Template"

        # format loop
        - name: "Add image signatures to POTX"
          link: "https://products.groupdocs.com/signature/net/add/jpg/potx/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Add image signatures to PPTM"
          link: "https://products.groupdocs.com/signature/net/add/jpg/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Add image signatures to ODP"
          link: "https://products.groupdocs.com/signature/net/add/jpg/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Add image signatures to OTP"
          link: "https://products.groupdocs.com/signature/net/add/jpg/otp/"
          description: "OpenDocument Presentation Template"

        # format loop
        - name: "Add image signatures to WEBP"
          link: "https://products.groupdocs.com/signature/net/add/jpg/webp/"
          description: "WebP Image"

        # format loop
        - name: "Add image signatures to TIFF"
          link: "https://products.groupdocs.com/signature/net/add/jpg/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Add image signatures to JPEG"
          link: "https://products.groupdocs.com/signature/net/add/jpg/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Add image signatures to GIF"
          link: "https://products.groupdocs.com/signature/net/add/jpg/gif/"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Add image signatures to PNG"
          link: "https://products.groupdocs.com/signature/net/add/jpg/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Add image signatures to BMP"
          link: "https://products.groupdocs.com/signature/net/add/jpg/bmp/"
          description: "Bitmap File Format"

        # format loop
        - name: "Add image signatures to CDR"
          link: "https://products.groupdocs.com/signature/net/add/jpg/cdr/"
          description: "CorelDraw Vector Graphic Drawing"

        # format loop
        - name: "Add image signatures to SVG"
          link: "https://products.groupdocs.com/signature/net/add/jpg/svg/"
          description: "Scalable Vector Graphics"

        # format loop
        - name: "Add image signatures to PSD"
          link: "https://products.groupdocs.com/signature/net/add/jpg/psd/"
          description: "Adobe Photoshop Document"

        # format loop
        - name: "Add image signatures to WMF"
          link: "https://products.groupdocs.com/signature/net/add/jpg/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Add image signatures to EMF"
          link: "https://products.groupdocs.com/signature/net/add/jpg/emf/"
          description: "Enhanced Metafile Format"

        # format loop
        - name: "Add image signatures to CMX"
          link: "https://products.groupdocs.com/signature/net/add/jpg/cmx/"
          description: "Corel Metafile eXchange Image"

        # format loop
        - name: "Add image signatures to DJVU"
          link: "https://products.groupdocs.com/signature/net/add/jpg/djvu/"
          description: "Deja Vu"

        # format loop
        - name: "Add image signatures to PPSM"
          link: "https://products.groupdocs.com/signature/net/add/jpg/ppsm/"
          description: "Microsoft PowerPoint Macro-Enabled Slide Show"

        # format loop
        - name: "Add image signatures to DCM"
          link: "https://products.groupdocs.com/signature/net/add/jpg/dcm/"
          description: "Digital Imaging and Communications in Medicine"


############################# Back to top ###############################
back_to_top:
    enable: true
---
