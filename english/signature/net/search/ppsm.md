---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:48+03:00
draft: false

############################# Head ############################
head_title: "Search &amp; Validate Digital Signatures in a PPSM file in C# .NET"
head_description: "C# .NET API to search digital signatures in a signed PPSM file, other images and document file formats using a few lines of code."

############################# Header ############################
title: "Search Digital Signatures in PPSM File"
description: "C# .NET native API to view &amp; search digital signatures in an already signed PPSM file and analyze signature certificate. Perform advanced e-signature operations within your documents using a few lines of code."
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
            - link: "https://docs.groupdocs.com/signature/net/release-notes"
              text: "Release Notes"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/net"
        link_buy: "https://purchase.groupdocs.com"

############################# About ############################
about:
    enable: true
    title: "About GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net) is an advanced .NET API to electronically sign digital documents using various signature types such as text, image, barcode, stamp, form-field, QR-code and metadata. Users can load, edit, validate, save, remove, find and preview digital signatures within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats, with additional support for customizing signature properties as needed.

############################# Steps ############################
steps:
    enable: true
    title_left: "How to Search Signatures in PPSM"
    content_left: |
        [GroupDocs.Signature](https://products.groupdocs.com/signature/net) makes it easy for .NET developers to view & search digital signatures in PPSM files from within their applications by implementing a few easy steps.

        *   Create new instance of Signature class and pass source document path as a constructor parameter.
        *   Instantiate the DigitalSearchOptions object according to your requirements and specify search options.
        *   Call Search method of Signature class instance and pass DigitalSearchOptions to it.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installled on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```cs
        using (Signature signature = new Signature("signed.pdf"))
        {
            DigitalSearchOptions options = new DigitalSearchOptions()
            {
                // specify special search criteria
                Comments = "Test comment",
                // certificate issues criteria
                IssuerName = "John",
                // digital certificate subject
                SubjectName = "Test",
                // specify date range period of signature
                SignDateTimeFrom = DateTime.Now.AddMonths(-1),
                SignDateTimeTo = DateTime.Now,
                //
            };
            // search for signatures in document
            List signatures = signature.Search(options);
            Console.WriteLine("\nSource document contains following signatures.");
            foreach (var digitalSignature in signatures)
            {
                Console.WriteLine("Digital signature found from {0} with validation flag {1}. Certificate SN {2}",
                    digitalSignature.SignTime, digitalSignature.IsValid, digitalSignature.Certificate?.SerialNumber);
            }
        }
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Search PPSM Signature Live Demos"
    content: |
        Add PPSM file electronic signatures right now by visiting [GroupDocs.Signature Live Demos](https://products.groupdocs.app/signature/family) website.
        The live demo has the following benefits
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-ppsm"
          title: "What is PPSM File Format"
          content: |
            Files with PPSM extension represent Macro-enabled Slide Show file format created with Microsoft PowerPoint 2007 or higher. Another similar file format is PPTM which differs in opening with Microsoft PowerPoint in editable format instead of running as Slide Show. When run as slide show, the PPSM file shows the presentation slides with contents intact in the slide show and is in read-only mode by default. PPSM files can still be edited in Microsoft PowerPoint by opening it in PowerPoint. Learn more about PPSM file format

          link: "https://docs.fileformat.com/presentation/ppsm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Other Available Options"
    content: |
        Multi format digital-signatures searching API for documents and images. Find signatures from some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Search e-Signatures in PDF"
          link: "https://products.groupdocs.com/signature/net/search/pdf"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Search e-Signatures in DOC"
          link: "https://products.groupdocs.com/signature/net/search/doc"
          description: "Microsoft Word Document"

        # format loop
        - name: "Search e-Signatures in DOCM"
          link: "https://products.groupdocs.com/signature/net/search/docm"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Search e-Signatures in DOCX"
          link: "https://products.groupdocs.com/signature/net/search/docx"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Search e-Signatures in DOT"
          link: "https://products.groupdocs.com/signature/net/search/dot"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Search e-Signatures in DOTX"
          link: "https://products.groupdocs.com/signature/net/search/dotx"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Search e-Signatures in DOTM"
          link: "https://products.groupdocs.com/signature/net/search/dotm"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Search e-Signatures in RTF"
          link: "https://products.groupdocs.com/signature/net/search/rtf"
          description: "Rich Text Document"

        # format loop
        - name: "Search e-Signatures in ODT"
          link: "https://products.groupdocs.com/signature/net/search/odt"
          description: "Open Document Text"

        # format loop
        - name: "Search e-Signatures in OTT"
          link: "https://products.groupdocs.com/signature/net/search/ott"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Search e-Signatures in XLS"
          link: "https://products.groupdocs.com/signature/net/search/xls"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Search e-Signatures in XLSX"
          link: "https://products.groupdocs.com/signature/net/search/xlsx"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Search e-Signatures in XLSM"
          link: "https://products.groupdocs.com/signature/net/search/xlsm"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Search e-Signatures in XLSM"
          link: "https://products.groupdocs.com/signature/net/search/xlsm"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Search e-Signatures in XLSB"
          link: "https://products.groupdocs.com/signature/net/search/xlsb"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Search e-Signatures in XLTX"
          link: "https://products.groupdocs.com/signature/net/search/xltx"
          description: "Microsoft Excel template"

        # format loop
        - name: "Search e-Signatures in XLTM"
          link: "https://products.groupdocs.com/signature/net/search/xltm"
          description: "Microsoft Excel macro-enabled template"

        # format loop
        - name: "Search e-Signatures in ODS"
          link: "https://products.groupdocs.com/signature/net/search/ods"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Search e-Signatures in OTS"
          link: "https://products.groupdocs.com/signature/net/search/ots"
          description: "OpenDocument Spreadsheet Template"

        # format loop
        - name: "Search e-Signatures in PPT"
          link: "https://products.groupdocs.com/signature/net/search/ppt"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Search e-Signatures in PPTX"
          link: "https://products.groupdocs.com/signature/net/search/pptx"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Search e-Signatures in PPS"
          link: "https://products.groupdocs.com/signature/net/search/pps"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Search e-Signatures in PPSX"
          link: "https://products.groupdocs.com/signature/net/search/ppsx"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Search e-Signatures in POTM"
          link: "https://products.groupdocs.com/signature/net/search/potm"
          description: "Microsoft PowerPoint Macro-Enabled Template"

        # format loop
        - name: "Search e-Signatures in POTX"
          link: "https://products.groupdocs.com/signature/net/search/potx"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Search e-Signatures in PPTM"
          link: "https://products.groupdocs.com/signature/net/search/pptm"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Search e-Signatures in ODP"
          link: "https://products.groupdocs.com/signature/net/search/odp"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Search e-Signatures in OTP"
          link: "https://products.groupdocs.com/signature/net/search/otp"
          description: "OpenDocument Presentation Template"

        # format loop
        - name: "Search e-Signatures in WEBP"
          link: "https://products.groupdocs.com/signature/net/search/webp"
          description: "WebP Image"

        # format loop
        - name: "Search e-Signatures in TIFF"
          link: "https://products.groupdocs.com/signature/net/search/tiff"
          description: "Tagged Image File Format"

        # format loop
        - name: "Search e-Signatures in JPEG"
          link: "https://products.groupdocs.com/signature/net/search/jpeg"
          description: "JPEG Image"

        # format loop
        - name: "Search e-Signatures in GIF"
          link: "https://products.groupdocs.com/signature/net/search/gif"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Search e-Signatures in PNG"
          link: "https://products.groupdocs.com/signature/net/search/png"
          description: "Portable Network Graphic"

        # format loop
        - name: "Search e-Signatures in BMP"
          link: "https://products.groupdocs.com/signature/net/search/bmp"
          description: "Bitmap File Format"

        # format loop
        - name: "Search e-Signatures in CDR"
          link: "https://products.groupdocs.com/signature/net/search/cdr"
          description: "CorelDraw Vector Graphic Drawing"

        # format loop
        - name: "Search e-Signatures in SVG"
          link: "https://products.groupdocs.com/signature/net/search/svg"
          description: "Scalable Vector Graphics"

        # format loop
        - name: "Search e-Signatures in PSD"
          link: "https://products.groupdocs.com/signature/net/search/psd"
          description: "Adobe Photoshop Document"

        # format loop
        - name: "Search e-Signatures in WMF"
          link: "https://products.groupdocs.com/signature/net/search/wmf"
          description: "Windows Metafile"

        # format loop
        - name: "Search e-Signatures in EMF"
          link: "https://products.groupdocs.com/signature/net/search/emf"
          description: "Enhanced Metafile Format"

        # format loop
        - name: "Search e-Signatures in CMX"
          link: "https://products.groupdocs.com/signature/net/search/cmx"
          description: "Corel Metafile eXchange Image"

        # format loop
        - name: "Search e-Signatures in DJVU"
          link: "https://products.groupdocs.com/signature/net/search/djvu"
          description: "Deja Vu"

        # format loop
        - name: "Search e-Signatures in PPSM"
          link: "https://products.groupdocs.com/signature/net/search/ppsm"
          description: "Microsoft PowerPoint Macro-Enabled Slide Show"

        # format loop
        - name: "Search e-Signatures in DCM"
          link: "https://products.groupdocs.com/signature/net/search/dcm"
          description: "Digital Imaging and Communications in Medicine"


############################# Back to top ###############################
back_to_top:
    enable: true
---
