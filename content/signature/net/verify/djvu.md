---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:51+03:00
draft: false

############################# Head ############################
head_title: "Verify Digital Signatures in a DJVU file in C# .NET"
head_description: "C# .NET API to verify &amp; validate digital signatures in a signed DJVU file, other images and document file formats using a few lines of code."

############################# Header ############################
title: "Verify Digital Signatures in a DJVU File"
description: "C# .NET API to verify digital signatures in an already signed DJVU file using popular electronic signature types. Manipulate e-signature properties within your documents by adding a few lined of code."
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
        [GroupDocs.Signature for .NET](/signature/net/) is a advanced .NET API to electronically sign digital documents using various signature types such as text, image, barcode, stamp, form-field, QR-code and metadata. Users can load, edit, validate, save, remove, preview and search digital signatures within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats, with additional support for customizing signature properties as needed.

############################# Steps ############################
steps:
    enable: true
    title_left: "How to Verify Digital Signatures in DJVU"
    content_left: |
        [GroupDocs.Signature](/signature/net/) makes it easy for .NET developers to verify digital signatures in DJVU files from within their applications by implementing a few easy steps.

        1.  Create new instance of Signature class and pass source document path as a constructor parameter.
        2.  Instantiate the DigitalVerifyOptions object according to your requirements and specify verification options.
        3.  Call Verify method of Signature class and pass DigitalVerifyOptions to it.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Signature for .NET from [NuGet](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```cs
        using (Signature signature = new Signature("sample.pdf"))
        {
            DigitalVerifyOptions options = new DigitalVerifyOptions("certificate.pfx")
            {
                Comments = "Test comment"
            };
            // verify document signatures
            VerificationResult result = signature.Verify(options);
            if (result.IsValid)
            {
                Console.WriteLine("\nDocument was verified successfully!");
            }
            else
            {
                Console.WriteLine("\nDocument failed verification process.");
            }
        }
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Verify DJVU Signature Live Demos"
    content: |
        Add DJVU file electronic signatures right now by visiting [GroupDocs.Signature Live Demos](https://products.groupdocs.app/signature/family) website.
        The live demo has the following benefits
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-djvu"
          title: "What is DJVU File Format"
          content: |
            DjVu, pronounced as “déjà vu”, is a graphics file format intended for scanned documents and books especially those which contain the combination of text, drawings, images and photographs. It was developed by AT&T Labs. It uses multiple techniques like image layer separation of text and background images, progressive loading, arithmetic coding and lossy compression for bitonal images. Since DJVU file can contain compressed yet high-quality colour images, photographs, text, and drawings and can be saved in less space therefore, it's used on web as eBooks, manuals, newspapers, ancient documents, etc. Learn more about DJVU file format

          link: "https://docs.fileformat.com/image/djvu/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Other Available Options"
    content: |
        Multi format digital-signatures validation API for documents and images. Verify signatures from some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Verify e-Signatures in PDF"
          link: "/signature/net/verify/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Verify e-Signatures in DOC"
          link: "/signature/net/verify/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Verify e-Signatures in DOCM"
          link: "/signature/net/verify/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Verify e-Signatures in DOCX"
          link: "/signature/net/verify/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Verify e-Signatures in DOT"
          link: "/signature/net/verify/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Verify e-Signatures in DOTX"
          link: "/signature/net/verify/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Verify e-Signatures in DOTM"
          link: "/signature/net/verify/dotm/"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Verify e-Signatures in RTF"
          link: "/signature/net/verify/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Verify e-Signatures in ODT"
          link: "/signature/net/verify/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Verify e-Signatures in OTT"
          link: "/signature/net/verify/ott/"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Verify e-Signatures in XLS"
          link: "/signature/net/verify/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Verify e-Signatures in XLSX"
          link: "/signature/net/verify/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Verify e-Signatures in XLSM"
          link: "/signature/net/verify/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Verify e-Signatures in XLSM"
          link: "/signature/net/verify/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Verify e-Signatures in XLSB"
          link: "/signature/net/verify/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Verify e-Signatures in XLTX"
          link: "/signature/net/verify/xltx/"
          description: "Microsoft Excel template"

        # format loop
        - name: "Verify e-Signatures in XLTM"
          link: "/signature/net/verify/xltm/"
          description: "Microsoft Excel macro-enabled template"

        # format loop
        - name: "Verify e-Signatures in ODS"
          link: "/signature/net/verify/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Verify e-Signatures in OTS"
          link: "/signature/net/verify/ots/"
          description: "OpenDocument Spreadsheet Template"

        # format loop
        - name: "Verify e-Signatures in PPT"
          link: "/signature/net/verify/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Verify e-Signatures in PPTX"
          link: "/signature/net/verify/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Verify e-Signatures in PPS"
          link: "/signature/net/verify/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Verify e-Signatures in PPSX"
          link: "/signature/net/verify/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Verify e-Signatures in POTM"
          link: "/signature/net/verify/potm/"
          description: "Microsoft PowerPoint Macro-Enabled Template"

        # format loop
        - name: "Verify e-Signatures in POTX"
          link: "/signature/net/verify/potx/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Verify e-Signatures in PPTM"
          link: "/signature/net/verify/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Verify e-Signatures in ODP"
          link: "/signature/net/verify/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Verify e-Signatures in OTP"
          link: "/signature/net/verify/otp/"
          description: "OpenDocument Presentation Template"

        # format loop
        - name: "Verify e-Signatures in WEBP"
          link: "/signature/net/verify/webp/"
          description: "WebP Image"

        # format loop
        - name: "Verify e-Signatures in TIFF"
          link: "/signature/net/verify/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Verify e-Signatures in JPEG"
          link: "/signature/net/verify/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Verify e-Signatures in GIF"
          link: "/signature/net/verify/gif/"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Verify e-Signatures in PNG"
          link: "/signature/net/verify/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Verify e-Signatures in BMP"
          link: "/signature/net/verify/bmp/"
          description: "Bitmap File Format"

        # format loop
        - name: "Verify e-Signatures in CDR"
          link: "/signature/net/verify/cdr/"
          description: "CorelDraw Vector Graphic Drawing"

        # format loop
        - name: "Verify e-Signatures in SVG"
          link: "/signature/net/verify/svg/"
          description: "Scalable Vector Graphics"

        # format loop
        - name: "Verify e-Signatures in PSD"
          link: "/signature/net/verify/psd/"
          description: "Adobe Photoshop Document"

        # format loop
        - name: "Verify e-Signatures in WMF"
          link: "/signature/net/verify/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Verify e-Signatures in EMF"
          link: "/signature/net/verify/emf/"
          description: "Enhanced Metafile Format"

        # format loop
        - name: "Verify e-Signatures in CMX"
          link: "/signature/net/verify/cmx/"
          description: "Corel Metafile eXchange Image"

        # format loop
        - name: "Verify e-Signatures in DJVU"
          link: "/signature/net/verify/djvu/"
          description: "Deja Vu"

        # format loop
        - name: "Verify e-Signatures in PPSM"
          link: "/signature/net/verify/ppsm/"
          description: "Microsoft PowerPoint Macro-Enabled Slide Show"

        # format loop
        - name: "Verify e-Signatures in DCM"
          link: "/signature/net/verify/dcm/"
          description: "Digital Imaging and Communications in Medicine"


############################# Back to top ###############################
back_to_top:
    enable: true
---
