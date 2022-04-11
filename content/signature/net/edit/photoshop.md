---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:34+03:00
draft: false

############################# Head ############################
head_title: "Edit &amp; Update a Digitally Signed PHOTOSHOP file in .NET | Sign Documents"
head_description: "Edit PHOTOSHOP files with digital signatures in .NET - update electronic signatures within popular business documents and image file formats."

############################# Header ############################
title: "Edit Digital Signatures in a PHOTOSHOP File"
description: "C# .NET API to instantly edit electronic signatures in PHOTOSHOP files using popular digital signature types. Manage signature properties and customize signing options within documents and images."
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
        [GroupDocs.Signature for .NET](/signature/net/) is a native .NET API to digitally sign documents using various signature types such as text, image, barcode, stamp, form-field, QR-code and metadata. Users can easily add, edit, verify, remove and find digital signatures within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats with additional support for customizing signature properties as needed.

############################# Steps ############################
steps:
    enable: true
    title_left: "How to Edit Digital Signatures in PHOTOSHOP"
    content_left: |
        [GroupDocs.Signature](/signature/net/) makes it easy for .NET developers to edit digital signatures from PHOTOSHOP files within their applications by implementing a few easy steps.

        *   Create new instance of Signature class and pass source document path as a constructor parameter.
        *   Instantiate TextSearchOptions object with desired properties.
        *   Call Search method to obtain list of TextSignatures.
        *   Select from list TextSignature object(s) that should be updated.
        *   Call Signature object Update method & pass one / several signatures to it.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Signature for .NET from [NuGet](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```cs
        using (Signature signature = new Signature("sampleSigned.pdf"))
        {
            TextSearchOptions options = new TextSearchOptions();
            // search for text signatures in document
            List signatures = signature.Search(options);
            if(signatures.Count > 0)
            {
                TextSignature textSignature = signatures[0];
                // change Text property
                textSignature.Text = "John Walkman";
                // change position
                textSignature.Left = textSignature.Left + 10;
                textSignature.Top = textSignature.Top + 10;
                // change size. Please note not all documents support changing signature size
                textSignature.Width = 200;
                textSignature.Height = 100;
                bool result = signature.Update(textSignature);
                if(result)
                {
                    Console.WriteLine($"Signature with Text '{textSignature.Text}' was updated in the document ['{fileName}'].");
                }
                else
                {
                    Console.WriteLine($"Signature was not updated in  the document! Signature with Text '{textSignature.Text}' was not found!");
                }
            }
        }
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Live Demos - Online App to Update Digital Signatures"
    content: |
        Edit signatures in PHOTOSHOP files right now by visiting [GroupDocs.Signature Live Demos](https://products.groupdocs.app/signature/family) website.  
        The live demo has the following benefits
        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-photoshop"
          title: "About PHOTOSHOP File Format"
          content: |
            PSD, Photoshop Document, represents Adobe Photoshop’s native file format used for graphics designing and development. PSD files may include image layers, adjustment layers, layer masks, annotations, file information, keywords and other Photoshop-specific elements. Photoshop files have default extension as .PSD and has a maximum height and width of 30,000 pixels, and a length limit of two gigabytes.

          link: "https://docs.fileformat.com/image/psd/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Editing Signatures From Other Digital Document Formats"
    content: |
        Multi format documents and images signatures editing API for .NET. Update signatures from some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Edit e-Signatures from PDF"
          link: "/signature/net/edit/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Edit e-Signatures from DOC"
          link: "/signature/net/edit/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Edit e-Signatures from DOCM"
          link: "/signature/net/edit/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Edit e-Signatures from DOCX"
          link: "/signature/net/edit/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Edit e-Signatures from DOT"
          link: "/signature/net/edit/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Edit e-Signatures from DOTX"
          link: "/signature/net/edit/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Edit e-Signatures from DOTM"
          link: "/signature/net/edit/dotm/"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Edit e-Signatures from RTF"
          link: "/signature/net/edit/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Edit e-Signatures from ODT"
          link: "/signature/net/edit/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Edit e-Signatures from OTT"
          link: "/signature/net/edit/ott/"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Edit e-Signatures from XLS"
          link: "/signature/net/edit/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Edit e-Signatures from XLSX"
          link: "/signature/net/edit/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Edit e-Signatures from XLSM"
          link: "/signature/net/edit/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Edit e-Signatures from XLSM"
          link: "/signature/net/edit/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Edit e-Signatures from XLSB"
          link: "/signature/net/edit/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Edit e-Signatures from XLTX"
          link: "/signature/net/edit/xltx/"
          description: "Microsoft Excel template"

        # format loop
        - name: "Edit e-Signatures from XLTM"
          link: "/signature/net/edit/xltm/"
          description: "Microsoft Excel macro-enabled template"

        # format loop
        - name: "Edit e-Signatures from ODS"
          link: "/signature/net/edit/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Edit e-Signatures from OTS"
          link: "/signature/net/edit/ots/"
          description: "OpenDocument Spreadsheet Template"

        # format loop
        - name: "Edit e-Signatures from PPT"
          link: "/signature/net/edit/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Edit e-Signatures from PPTX"
          link: "/signature/net/edit/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Edit e-Signatures from PPS"
          link: "/signature/net/edit/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Edit e-Signatures from PPSX"
          link: "/signature/net/edit/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Edit e-Signatures from POTM"
          link: "/signature/net/edit/potm/"
          description: "Microsoft PowerPoint Macro-Enabled Template"

        # format loop
        - name: "Edit e-Signatures from POTX"
          link: "/signature/net/edit/potx/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Edit e-Signatures from PPTM"
          link: "/signature/net/edit/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Edit e-Signatures from ODP"
          link: "/signature/net/edit/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Edit e-Signatures from OTP"
          link: "/signature/net/edit/otp/"
          description: "OpenDocument Presentation Template"

        # format loop
        - name: "Edit e-Signatures from WEBP"
          link: "/signature/net/edit/webp/"
          description: "WebP Image"

        # format loop
        - name: "Edit e-Signatures from TIFF"
          link: "/signature/net/edit/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Edit e-Signatures from JPEG"
          link: "/signature/net/edit/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Edit e-Signatures from GIF"
          link: "/signature/net/edit/gif/"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Edit e-Signatures from PNG"
          link: "/signature/net/edit/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Edit e-Signatures from BMP"
          link: "/signature/net/edit/bmp/"
          description: "Bitmap File Format"

        # format loop
        - name: "Edit e-Signatures from CDR"
          link: "/signature/net/edit/cdr/"
          description: "CorelDraw Vector Graphic Drawing"

        # format loop
        - name: "Edit e-Signatures from SVG"
          link: "/signature/net/edit/svg/"
          description: "Scalable Vector Graphics"

        # format loop
        - name: "Edit e-Signatures from PSD"
          link: "/signature/net/edit/psd/"
          description: "Adobe Photoshop Document"

        # format loop
        - name: "Edit e-Signatures from WMF"
          link: "/signature/net/edit/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Edit e-Signatures from EMF"
          link: "/signature/net/edit/emf/"
          description: "Enhanced Metafile Format"

        # format loop
        - name: "Edit e-Signatures from CMX"
          link: "/signature/net/edit/cmx/"
          description: "Corel Metafile eXchange Image"

        # format loop
        - name: "Edit e-Signatures from DJVU"
          link: "/signature/net/edit/djvu/"
          description: "Deja Vu"

        # format loop
        - name: "Edit e-Signatures from PPSM"
          link: "/signature/net/edit/ppsm/"
          description: "Microsoft PowerPoint Macro-Enabled Slide Show"

        # format loop
        - name: "Edit e-Signatures from DCM"
          link: "/signature/net/edit/dcm/"
          description: "Digital Imaging and Communications in Medicine"


############################# Back to top ###############################
back_to_top:
    enable: true
---
