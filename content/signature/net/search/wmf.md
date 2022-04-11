---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:50+03:00
draft: false

############################# Head ############################
head_title: "Search &amp; Validate Digital Signatures in a WMF file in C# .NET"
head_description: "C# .NET API to search digital signatures in a signed WMF file, other images and document file formats using a few lines of code."

############################# Header ############################
title: "Search Digital Signatures in WMF File"
description: "C# .NET native API to view &amp; search digital signatures in an already signed WMF file and analyze signature certificate. Perform advanced e-signature operations within your documents using a few lines of code."
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
        [GroupDocs.Signature for .NET](/signature/net/) is an advanced .NET API to electronically sign digital documents using various signature types such as text, image, barcode, stamp, form-field, QR-code and metadata. Users can load, edit, validate, save, remove, find and preview digital signatures within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats, with additional support for customizing signature properties as needed.

############################# Steps ############################
steps:
    enable: true
    title_left: "How to Search Signatures in WMF"
    content_left: |
        [GroupDocs.Signature](/signature/net/) makes it easy for .NET developers to view & search digital signatures in WMF files from within their applications by implementing a few easy steps.

        *   Create new instance of Signature class and pass source document path as a constructor parameter.
        *   Instantiate the DigitalSearchOptions object according to your requirements and specify search options.
        *   Call Search method of Signature class instance and pass DigitalSearchOptions to it.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Signature for .NET from [NuGet](https://www.nuget.org/packages/groupdocs.signature)
        
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
    title: "Search WMF Signature Live Demos"
    content: |
        Add WMF file electronic signatures right now by visiting [GroupDocs.Signature Live Demos](https://products.groupdocs.app/signature/family) website.
        The live demo has the following benefits
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-wmf"
          title: "What is WMF File Format"
          content: |
            Files with WMF extension represent Microsoft Windows Metafile (WMF) for storing vector as well as bitmap-format images data. To be more accurate, WMF belongs to the vector file format category of Graphics file formats that is device independent. Windows Graphical Device Interface (GDI) uses the functions stored in a WMF file to display an image on the screen. A more enhanced version of WMF, known as Enhanced Meta Files (EMF), was published later that makes the format more feature rich. Practically, WMF are similar to SVG. Learn more about WMF file format

          link: "https://docs.fileformat.com/image/wmf/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Other Available Options"
    content: |
        Multi format digital-signatures searching API for documents and images. Find signatures from some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Search e-Signatures in PDF"
          link: "/signature/net/search/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Search e-Signatures in DOC"
          link: "/signature/net/search/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Search e-Signatures in DOCM"
          link: "/signature/net/search/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Search e-Signatures in DOCX"
          link: "/signature/net/search/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Search e-Signatures in DOT"
          link: "/signature/net/search/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Search e-Signatures in DOTX"
          link: "/signature/net/search/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Search e-Signatures in DOTM"
          link: "/signature/net/search/dotm/"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Search e-Signatures in RTF"
          link: "/signature/net/search/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Search e-Signatures in ODT"
          link: "/signature/net/search/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Search e-Signatures in OTT"
          link: "/signature/net/search/ott/"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Search e-Signatures in XLS"
          link: "/signature/net/search/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Search e-Signatures in XLSX"
          link: "/signature/net/search/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Search e-Signatures in XLSM"
          link: "/signature/net/search/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Search e-Signatures in XLSM"
          link: "/signature/net/search/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Search e-Signatures in XLSB"
          link: "/signature/net/search/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Search e-Signatures in XLTX"
          link: "/signature/net/search/xltx/"
          description: "Microsoft Excel template"

        # format loop
        - name: "Search e-Signatures in XLTM"
          link: "/signature/net/search/xltm/"
          description: "Microsoft Excel macro-enabled template"

        # format loop
        - name: "Search e-Signatures in ODS"
          link: "/signature/net/search/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Search e-Signatures in OTS"
          link: "/signature/net/search/ots/"
          description: "OpenDocument Spreadsheet Template"

        # format loop
        - name: "Search e-Signatures in PPT"
          link: "/signature/net/search/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Search e-Signatures in PPTX"
          link: "/signature/net/search/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Search e-Signatures in PPS"
          link: "/signature/net/search/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Search e-Signatures in PPSX"
          link: "/signature/net/search/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Search e-Signatures in POTM"
          link: "/signature/net/search/potm/"
          description: "Microsoft PowerPoint Macro-Enabled Template"

        # format loop
        - name: "Search e-Signatures in POTX"
          link: "/signature/net/search/potx/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Search e-Signatures in PPTM"
          link: "/signature/net/search/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Search e-Signatures in ODP"
          link: "/signature/net/search/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Search e-Signatures in OTP"
          link: "/signature/net/search/otp/"
          description: "OpenDocument Presentation Template"

        # format loop
        - name: "Search e-Signatures in WEBP"
          link: "/signature/net/search/webp/"
          description: "WebP Image"

        # format loop
        - name: "Search e-Signatures in TIFF"
          link: "/signature/net/search/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Search e-Signatures in JPEG"
          link: "/signature/net/search/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Search e-Signatures in GIF"
          link: "/signature/net/search/gif/"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Search e-Signatures in PNG"
          link: "/signature/net/search/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Search e-Signatures in BMP"
          link: "/signature/net/search/bmp/"
          description: "Bitmap File Format"

        # format loop
        - name: "Search e-Signatures in CDR"
          link: "/signature/net/search/cdr/"
          description: "CorelDraw Vector Graphic Drawing"

        # format loop
        - name: "Search e-Signatures in SVG"
          link: "/signature/net/search/svg/"
          description: "Scalable Vector Graphics"

        # format loop
        - name: "Search e-Signatures in PSD"
          link: "/signature/net/search/psd/"
          description: "Adobe Photoshop Document"

        # format loop
        - name: "Search e-Signatures in WMF"
          link: "/signature/net/search/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Search e-Signatures in EMF"
          link: "/signature/net/search/emf/"
          description: "Enhanced Metafile Format"

        # format loop
        - name: "Search e-Signatures in CMX"
          link: "/signature/net/search/cmx/"
          description: "Corel Metafile eXchange Image"

        # format loop
        - name: "Search e-Signatures in DJVU"
          link: "/signature/net/search/djvu/"
          description: "Deja Vu"

        # format loop
        - name: "Search e-Signatures in PPSM"
          link: "/signature/net/search/ppsm/"
          description: "Microsoft PowerPoint Macro-Enabled Slide Show"

        # format loop
        - name: "Search e-Signatures in DCM"
          link: "/signature/net/search/dcm/"
          description: "Digital Imaging and Communications in Medicine"


############################# Back to top ###############################
back_to_top:
    enable: true
---
