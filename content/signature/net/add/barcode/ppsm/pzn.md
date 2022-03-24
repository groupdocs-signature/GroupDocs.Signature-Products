---
############################# Static ############################
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

############################# Head ############################
head_title: "Generate Pzn Barcode and Sign PPSM File in .NET | Sign Documents"
head_description: "Sign PPSM files with Pzn barcode signatures in .NET - add barcodes to popular business documents and image file formats."

############################# Header ############################
title: "Add Pzn Barcode Signatures to PPSM File in C#"
description: "Sign your PPSM files using Pzn barcode. Manipulate signature properties and set up advanced signing options within documents that suit your needs."
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
    title_left: "How to Generate Pzn Barcode for PPSM file in C#"
    content_left: |
        [GroupDocs.Signature](https://products.groupdocs.com/signature/net) makes it easy for .NET developers to add Pzn barcodes to PPSM files within their applications by implementing a few easy steps.

        *   Create new instance of Signature class and pass source PPSM document path as a constructor parameter.
        *   Instantiate the BarcodeSignOptions object with required text and set EncodeType property to PZN.
        *   Call Sign method of Signature class and pass output PPSM file name with BarcodeSignOptions to it.
        *   Analyze SignResult result to check newly created signatures if needed.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installled on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```cs
        using (Signature signature = new Signature("sample.ppsm"))
        {
            // Initialize barcode options with predefined barcode text
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                // setup Barcode encoding type
                EncodeType = BarcodeTypes.PZN,

                // set signature position
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // Sign PPSM file and save result 
            signature.Sign("signed.ppsm", options);
        }
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Live Demos - Online App to Generate Pzn Barcode Signatures"
    content: |
        Add Pzn barcodes to PPSM files right now by visiting [GroupDocs.Signature Live Demos](https://products.groupdocs.app/signature/family) website.  
        The live demo has the following benefits
        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About PZN Barcode"
          content: |
            Pharmazentralnummer (PZN) is a variant of Code 39 - Regular that is used for the distribution and marking of health care and pharmaceutical products in Germany. Two versions are available: PZN7, which encodes six digits plus a check digit, and PZN8, which encodes seven digits plus a check digit. PZN7 is currently being phased out, and after January 1, 2020, only PZN8 will be used.

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Signing Other Document Formats with Pzn Barcode using C#"
    content: |
        .NET barcode signatures management API for documents and images. Add barcode signatures to some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Add e-Signatures to PDF"
          link: "https://products.groupdocs.com/signature/net/add/barcode/pdf/pzn/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Add e-Signatures to DOC"
          link: "https://products.groupdocs.com/signature/net/add/barcode/doc/pzn/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Add e-Signatures to DOCM"
          link: "https://products.groupdocs.com/signature/net/add/barcode/docm/pzn/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Add e-Signatures to DOCX"
          link: "https://products.groupdocs.com/signature/net/add/barcode/docx/pzn/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Add e-Signatures to DOT"
          link: "https://products.groupdocs.com/signature/net/add/barcode/dot/pzn/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Add e-Signatures to DOTX"
          link: "https://products.groupdocs.com/signature/net/add/barcode/dotx/pzn/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Add e-Signatures to DOTM"
          link: "https://products.groupdocs.com/signature/net/add/barcode/dotm/pzn/"
          description: "Microsoft Word Macro-Enabled Template"       

        # format loop
        - name: "Add e-Signatures to ODT"
          link: "https://products.groupdocs.com/signature/net/add/barcode/odt/pzn/"
          description: "Open Document Text"

        # format loop
        - name: "Add e-Signatures to OTT"
          link: "https://products.groupdocs.com/signature/net/add/barcode/ott/pzn/"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Add e-Signatures to XLS"
          link: "https://products.groupdocs.com/signature/net/add/barcode/xls/pzn/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Add e-Signatures to XLSX"
          link: "https://products.groupdocs.com/signature/net/add/barcode/xlsx/pzn/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Add e-Signatures to XLSM"
          link: "https://products.groupdocs.com/signature/net/add/barcode/xlsm/pzn/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Add e-Signatures to XLSB"
          link: "https://products.groupdocs.com/signature/net/add/barcode/xlsb/pzn/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Add e-Signatures to XLTX"
          link: "https://products.groupdocs.com/signature/net/add/barcode/xltx/pzn/"
          description: "Microsoft Excel template"

        # format loop
        - name: "Add e-Signatures to XLTM"
          link: "https://products.groupdocs.com/signature/net/add/barcode/xltm/pzn/"
          description: "Microsoft Excel macro-enabled template"

        # format loop
        - name: "Add e-Signatures to ODS"
          link: "https://products.groupdocs.com/signature/net/add/barcode/ods/pzn/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Add e-Signatures to OTS"
          link: "https://products.groupdocs.com/signature/net/add/barcode/ots/pzn/"
          description: "OpenDocument Spreadsheet Template"

        # format loop
        - name: "Add e-Signatures to PPT"
          link: "https://products.groupdocs.com/signature/net/add/barcode/ppt/pzn/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Add e-Signatures to PPTX"
          link: "https://products.groupdocs.com/signature/net/add/barcode/pptx/pzn/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Add e-Signatures to PPS"
          link: "https://products.groupdocs.com/signature/net/add/barcode/pps/pzn/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Add e-Signatures to PPSX"
          link: "https://products.groupdocs.com/signature/net/add/barcode/ppsx/pzn/"
          description: "PowerPoint Open XML Slide Show"                              

        # format loop
        - name: "Add e-Signatures to ODP"
          link: "https://products.groupdocs.com/signature/net/add/barcode/odp/pzn/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Add e-Signatures to OTP"
          link: "https://products.groupdocs.com/signature/net/add/barcode/otp/pzn/"
          description: "OpenDocument Presentation Template"

        # format loop
        - name: "Add e-Signatures to WEBP"
          link: "https://products.groupdocs.com/signature/net/add/barcode/webp/pzn/"
          description: "WebP Image"

        # format loop
        - name: "Add e-Signatures to TIF"
          link: "https://products.groupdocs.com/signature/net/add/barcode/tif/pzn/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Add e-Signatures to JPG"
          link: "https://products.groupdocs.com/signature/net/add/barcode/jpg/pzn/"
          description: "JPEG Image"

        # format loop
        - name: "Add e-Signatures to GIF"
          link: "https://products.groupdocs.com/signature/net/add/barcode/gif/pzn/"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Add e-Signatures to PNG"
          link: "https://products.groupdocs.com/signature/net/add/barcode/png/pzn/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Add e-Signatures to BMP"
          link: "https://products.groupdocs.com/signature/net/add/barcode/bmp/pzn/"
          description: "Bitmap File Format"

        # format loop
        - name: "Add e-Signatures to CDR"
          link: "https://products.groupdocs.com/signature/net/add/barcode/cdr/pzn/"
          description: "CorelDraw Vector Graphic Drawing"

        # format loop
        - name: "Add e-Signatures to SVG"
          link: "https://products.groupdocs.com/signature/net/add/barcode/svg/pzn/"
          description: "Scalable Vector Graphics"

        # format loop
        - name: "Add e-Signatures to PSD"
          link: "https://products.groupdocs.com/signature/net/add/barcode/psd/pzn/"
          description: "Adobe Photoshop Document"

        # format loop
        - name: "Add e-Signatures to WMF"
          link: "https://products.groupdocs.com/signature/net/add/barcode/wmf/pzn/"
          description: "Windows Metafile"        

        # format loop
        - name: "Add e-Signatures to CMX"
          link: "https://products.groupdocs.com/signature/net/add/barcode/cmx/pzn/"
          description: "Corel Metafile eXchange Image"

        # format loop
        - name: "Add e-Signatures to DJVU"
          link: "https://products.groupdocs.com/signature/net/add/barcode/djvu/pzn/"
          description: "Deja Vu"

        # format loop
        - name: "Add e-Signatures to PPSM"
          link: "https://products.groupdocs.com/signature/net/add/barcode/ppsm/pzn/"
          description: "Microsoft PowerPoint Macro-Enabled Slide Show"

############################# Back to top ###############################
back_to_top:
    enable: true
---
