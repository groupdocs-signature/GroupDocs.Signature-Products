---
############################# Static ############################
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

############################# Head ############################
head_title: "Generate Swisspostparcel Barcode and Sign XLSX File in .NET | Sign Documents"
head_description: "Sign XLSX files with Swisspostparcel barcode signatures in .NET - add barcodes to popular business documents and image file formats."

############################# Header ############################
title: "Add Swisspostparcel Barcode Signatures to XLSX File in C#"
description: "Sign your XLSX files using Swisspostparcel barcode. Manipulate signature properties and set up advanced signing options within documents that suit your needs."
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
    title_left: "How to Generate Swisspostparcel Barcode for XLSX file in C#"
    content_left: |
        [GroupDocs.Signature](https://products.groupdocs.com/signature/net) makes it easy for .NET developers to add Swisspostparcel barcodes to XLSX files within their applications by implementing a few easy steps.

        *   Create new instance of Signature class and pass source XLSX document path as a constructor parameter.
        *   Instantiate the BarcodeSignOptions object with required text and set EncodeType property to SwissPostParcel.
        *   Call Sign method of Signature class and pass output XLSX file name with BarcodeSignOptions to it.
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
        using (Signature signature = new Signature("sample.xlsx"))
        {
            // Initialize barcode options with predefined barcode text
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                // setup Barcode encoding type
                EncodeType = BarcodeTypes.SwissPostParcel,

                // set signature position
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // Sign XLSX file and save result 
            signature.Sign("signed.xlsx", options);
        }
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Live Demos - Online App to Generate Swisspostparcel Barcode Signatures"
    content: |
        Add Swisspostparcel barcodes to XLSX files right now by visiting [GroupDocs.Signature Live Demos](https://products.groupdocs.app/signature/family) website.  
        The live demo has the following benefits
        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About SwissPostParcel Barcode"
          content: |
            Swiss Post Parcel is postal barcode used in Switzerland for mails tracking.

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Signing Other Document Formats with Swisspostparcel Barcode using C#"
    content: |
        .NET barcode signatures management API for documents and images. Add barcode signatures to some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Add e-Signatures to PDF"
          link: "https://products.groupdocs.com/signature/net/add/barcode/pdf/swisspostparcel/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Add e-Signatures to DOC"
          link: "https://products.groupdocs.com/signature/net/add/barcode/doc/swisspostparcel/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Add e-Signatures to DOCM"
          link: "https://products.groupdocs.com/signature/net/add/barcode/docm/swisspostparcel/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Add e-Signatures to DOCX"
          link: "https://products.groupdocs.com/signature/net/add/barcode/docx/swisspostparcel/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Add e-Signatures to DOT"
          link: "https://products.groupdocs.com/signature/net/add/barcode/dot/swisspostparcel/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Add e-Signatures to DOTX"
          link: "https://products.groupdocs.com/signature/net/add/barcode/dotx/swisspostparcel/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Add e-Signatures to DOTM"
          link: "https://products.groupdocs.com/signature/net/add/barcode/dotm/swisspostparcel/"
          description: "Microsoft Word Macro-Enabled Template"       

        # format loop
        - name: "Add e-Signatures to ODT"
          link: "https://products.groupdocs.com/signature/net/add/barcode/odt/swisspostparcel/"
          description: "Open Document Text"

        # format loop
        - name: "Add e-Signatures to OTT"
          link: "https://products.groupdocs.com/signature/net/add/barcode/ott/swisspostparcel/"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Add e-Signatures to XLS"
          link: "https://products.groupdocs.com/signature/net/add/barcode/xls/swisspostparcel/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Add e-Signatures to XLSX"
          link: "https://products.groupdocs.com/signature/net/add/barcode/xlsx/swisspostparcel/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Add e-Signatures to XLSM"
          link: "https://products.groupdocs.com/signature/net/add/barcode/xlsm/swisspostparcel/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Add e-Signatures to XLSB"
          link: "https://products.groupdocs.com/signature/net/add/barcode/xlsb/swisspostparcel/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Add e-Signatures to XLTX"
          link: "https://products.groupdocs.com/signature/net/add/barcode/xltx/swisspostparcel/"
          description: "Microsoft Excel template"

        # format loop
        - name: "Add e-Signatures to XLTM"
          link: "https://products.groupdocs.com/signature/net/add/barcode/xltm/swisspostparcel/"
          description: "Microsoft Excel macro-enabled template"

        # format loop
        - name: "Add e-Signatures to ODS"
          link: "https://products.groupdocs.com/signature/net/add/barcode/ods/swisspostparcel/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Add e-Signatures to OTS"
          link: "https://products.groupdocs.com/signature/net/add/barcode/ots/swisspostparcel/"
          description: "OpenDocument Spreadsheet Template"

        # format loop
        - name: "Add e-Signatures to PPT"
          link: "https://products.groupdocs.com/signature/net/add/barcode/ppt/swisspostparcel/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Add e-Signatures to PPTX"
          link: "https://products.groupdocs.com/signature/net/add/barcode/pptx/swisspostparcel/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Add e-Signatures to PPS"
          link: "https://products.groupdocs.com/signature/net/add/barcode/pps/swisspostparcel/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Add e-Signatures to PPSX"
          link: "https://products.groupdocs.com/signature/net/add/barcode/ppsx/swisspostparcel/"
          description: "PowerPoint Open XML Slide Show"                              

        # format loop
        - name: "Add e-Signatures to ODP"
          link: "https://products.groupdocs.com/signature/net/add/barcode/odp/swisspostparcel/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Add e-Signatures to OTP"
          link: "https://products.groupdocs.com/signature/net/add/barcode/otp/swisspostparcel/"
          description: "OpenDocument Presentation Template"

        # format loop
        - name: "Add e-Signatures to WEBP"
          link: "https://products.groupdocs.com/signature/net/add/barcode/webp/swisspostparcel/"
          description: "WebP Image"

        # format loop
        - name: "Add e-Signatures to TIF"
          link: "https://products.groupdocs.com/signature/net/add/barcode/tif/swisspostparcel/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Add e-Signatures to JPG"
          link: "https://products.groupdocs.com/signature/net/add/barcode/jpg/swisspostparcel/"
          description: "JPEG Image"

        # format loop
        - name: "Add e-Signatures to GIF"
          link: "https://products.groupdocs.com/signature/net/add/barcode/gif/swisspostparcel/"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Add e-Signatures to PNG"
          link: "https://products.groupdocs.com/signature/net/add/barcode/png/swisspostparcel/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Add e-Signatures to BMP"
          link: "https://products.groupdocs.com/signature/net/add/barcode/bmp/swisspostparcel/"
          description: "Bitmap File Format"

        # format loop
        - name: "Add e-Signatures to CDR"
          link: "https://products.groupdocs.com/signature/net/add/barcode/cdr/swisspostparcel/"
          description: "CorelDraw Vector Graphic Drawing"

        # format loop
        - name: "Add e-Signatures to SVG"
          link: "https://products.groupdocs.com/signature/net/add/barcode/svg/swisspostparcel/"
          description: "Scalable Vector Graphics"

        # format loop
        - name: "Add e-Signatures to PSD"
          link: "https://products.groupdocs.com/signature/net/add/barcode/psd/swisspostparcel/"
          description: "Adobe Photoshop Document"

        # format loop
        - name: "Add e-Signatures to WMF"
          link: "https://products.groupdocs.com/signature/net/add/barcode/wmf/swisspostparcel/"
          description: "Windows Metafile"        

        # format loop
        - name: "Add e-Signatures to CMX"
          link: "https://products.groupdocs.com/signature/net/add/barcode/cmx/swisspostparcel/"
          description: "Corel Metafile eXchange Image"

        # format loop
        - name: "Add e-Signatures to DJVU"
          link: "https://products.groupdocs.com/signature/net/add/barcode/djvu/swisspostparcel/"
          description: "Deja Vu"

        # format loop
        - name: "Add e-Signatures to PPSM"
          link: "https://products.groupdocs.com/signature/net/add/barcode/ppsm/swisspostparcel/"
          description: "Microsoft PowerPoint Macro-Enabled Slide Show"

############################# Back to top ###############################
back_to_top:
    enable: true
---
