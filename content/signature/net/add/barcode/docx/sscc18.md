---
############################# Static ############################
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

############################# Head ############################
head_title: "Generate Sscc18 Barcode and Sign DOCX File in .NET | Sign Documents"
head_description: "Sign DOCX files with Sscc18 barcode signatures in .NET - add barcodes to popular business documents and image file formats."

############################# Header ############################
title: "Add Sscc18 Barcode Signatures to DOCX File in C#"
description: "Sign your DOCX files using Sscc18 barcode. Manipulate signature properties and set up advanced signing options within documents that suit your needs."
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
        [GroupDocs.Signature for .NET](/signature/net/) is a native .NET API to electronically sign digital documents using various signature types such as text, image, barcode, stamp, form-field, QR-code and metadata. Users can add, edit, verify, delete and search digital signatures within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats with additional support for customizing signature properties as needed.

############################# Steps ############################
steps:
    enable: true
    title_left: "How to Generate Sscc18 Barcode for DOCX file in C#"
    content_left: |
        [GroupDocs.Signature](/signature/net/) makes it easy for .NET developers to add Sscc18 barcodes to DOCX files within their applications by implementing a few easy steps.

        *   Create new instance of Signature class and pass source DOCX document path as a constructor parameter.
        *   Instantiate the BarcodeSignOptions object with required text and set EncodeType property to SSCC18.
        *   Call Sign method of Signature class and pass output DOCX file name with BarcodeSignOptions to it.
        *   Analyze SignResult result to check newly created signatures if needed.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Signature for .NET from [NuGet](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```cs
        using (Signature signature = new Signature("sample.docx"))
        {
            // Initialize barcode options with predefined barcode text
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                // setup Barcode encoding type
                EncodeType = BarcodeTypes.SSCC18,

                // set signature position
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // Sign DOCX file and save result 
            signature.Sign("signed.docx", options);
        }
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Live Demos - Online App to Generate Sscc18 Barcode Signatures"
    content: |
        Add Sscc18 barcodes to DOCX files right now by visiting [GroupDocs.Signature Live Demos](https://products.groupdocs.app/signature/family) website.  
        The live demo has the following benefits
        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About SSCC18 Barcode"
          content: |
            SSCC-18 (Serialized Shipping Container Code) is commonly used to uniquely identify shipping containers.

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Signing Other Document Formats with Sscc18 Barcode using C#"
    content: |
        .NET barcode signatures management API for documents and images. Add barcode signatures to some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Add e-Signatures to PDF"
          link: "/signature/net/add/barcode/pdf/sscc18/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Add e-Signatures to DOC"
          link: "/signature/net/add/barcode/doc/sscc18/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Add e-Signatures to DOCM"
          link: "/signature/net/add/barcode/docm/sscc18/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Add e-Signatures to DOCX"
          link: "/signature/net/add/barcode/docx/sscc18/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Add e-Signatures to DOT"
          link: "/signature/net/add/barcode/dot/sscc18/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Add e-Signatures to DOTX"
          link: "/signature/net/add/barcode/dotx/sscc18/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Add e-Signatures to DOTM"
          link: "/signature/net/add/barcode/dotm/sscc18/"
          description: "Microsoft Word Macro-Enabled Template"       

        # format loop
        - name: "Add e-Signatures to ODT"
          link: "/signature/net/add/barcode/odt/sscc18/"
          description: "Open Document Text"

        # format loop
        - name: "Add e-Signatures to OTT"
          link: "/signature/net/add/barcode/ott/sscc18/"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Add e-Signatures to XLS"
          link: "/signature/net/add/barcode/xls/sscc18/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Add e-Signatures to XLSX"
          link: "/signature/net/add/barcode/xlsx/sscc18/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Add e-Signatures to XLSM"
          link: "/signature/net/add/barcode/xlsm/sscc18/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Add e-Signatures to XLSB"
          link: "/signature/net/add/barcode/xlsb/sscc18/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Add e-Signatures to XLTX"
          link: "/signature/net/add/barcode/xltx/sscc18/"
          description: "Microsoft Excel template"

        # format loop
        - name: "Add e-Signatures to XLTM"
          link: "/signature/net/add/barcode/xltm/sscc18/"
          description: "Microsoft Excel macro-enabled template"

        # format loop
        - name: "Add e-Signatures to ODS"
          link: "/signature/net/add/barcode/ods/sscc18/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Add e-Signatures to OTS"
          link: "/signature/net/add/barcode/ots/sscc18/"
          description: "OpenDocument Spreadsheet Template"

        # format loop
        - name: "Add e-Signatures to PPT"
          link: "/signature/net/add/barcode/ppt/sscc18/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Add e-Signatures to PPTX"
          link: "/signature/net/add/barcode/pptx/sscc18/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Add e-Signatures to PPS"
          link: "/signature/net/add/barcode/pps/sscc18/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Add e-Signatures to PPSX"
          link: "/signature/net/add/barcode/ppsx/sscc18/"
          description: "PowerPoint Open XML Slide Show"                              

        # format loop
        - name: "Add e-Signatures to ODP"
          link: "/signature/net/add/barcode/odp/sscc18/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Add e-Signatures to OTP"
          link: "/signature/net/add/barcode/otp/sscc18/"
          description: "OpenDocument Presentation Template"

        # format loop
        - name: "Add e-Signatures to WEBP"
          link: "/signature/net/add/barcode/webp/sscc18/"
          description: "WebP Image"

        # format loop
        - name: "Add e-Signatures to TIF"
          link: "/signature/net/add/barcode/tif/sscc18/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Add e-Signatures to JPG"
          link: "/signature/net/add/barcode/jpg/sscc18/"
          description: "JPEG Image"

        # format loop
        - name: "Add e-Signatures to GIF"
          link: "/signature/net/add/barcode/gif/sscc18/"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Add e-Signatures to PNG"
          link: "/signature/net/add/barcode/png/sscc18/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Add e-Signatures to BMP"
          link: "/signature/net/add/barcode/bmp/sscc18/"
          description: "Bitmap File Format"

        # format loop
        - name: "Add e-Signatures to CDR"
          link: "/signature/net/add/barcode/cdr/sscc18/"
          description: "CorelDraw Vector Graphic Drawing"

        # format loop
        - name: "Add e-Signatures to SVG"
          link: "/signature/net/add/barcode/svg/sscc18/"
          description: "Scalable Vector Graphics"

        # format loop
        - name: "Add e-Signatures to PSD"
          link: "/signature/net/add/barcode/psd/sscc18/"
          description: "Adobe Photoshop Document"

        # format loop
        - name: "Add e-Signatures to WMF"
          link: "/signature/net/add/barcode/wmf/sscc18/"
          description: "Windows Metafile"        

        # format loop
        - name: "Add e-Signatures to CMX"
          link: "/signature/net/add/barcode/cmx/sscc18/"
          description: "Corel Metafile eXchange Image"

        # format loop
        - name: "Add e-Signatures to DJVU"
          link: "/signature/net/add/barcode/djvu/sscc18/"
          description: "Deja Vu"

        # format loop
        - name: "Add e-Signatures to PPSM"
          link: "/signature/net/add/barcode/ppsm/sscc18/"
          description: "Microsoft PowerPoint Macro-Enabled Slide Show"

############################# Back to top ###############################
back_to_top:
    enable: true
---