---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:34+03:00
draft: false

############################# Head ############################
head_title: "Edit &amp; Update a Digitally Signed OTP file in .NET | Sign Documents"
head_description: "Edit OTP files with digital signatures in .NET - update electronic signatures within popular business documents and image file formats."

############################# Header ############################
title: "Edit Digital Signatures in a OTP File"
description: "C# .NET API to instantly edit electronic signatures in OTP files using popular digital signature types. Manage signature properties and customize signing options within documents and images."
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
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net) is a native .NET API to digitally sign documents using various signature types such as text, image, barcode, stamp, form-field, QR-code and metadata. Users can easily add, edit, verify, remove and find digital signatures within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats with additional support for customizing signature properties as needed.

############################# Steps ############################
steps:
    enable: true
    title_left: "How to Edit Digital Signatures in OTP"
    content_left: |
        [GroupDocs.Signature](https://products.groupdocs.com/signature/net) makes it easy for .NET developers to edit digital signatures from OTP files within their applications by implementing a few easy steps.

        *   Create new instance of Signature class and pass source document path as a constructor parameter.
        *   Instantiate TextSearchOptions object with desired properties.
        *   Call Search method to obtain list of TextSignatures.
        *   Select from list TextSignature object(s) that should be updated.
        *   Call Signature object Update method & pass one / several signatures to it.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installled on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
        
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
        Edit signatures in OTP files right now by visiting [GroupDocs.Signature Live Demos](https://products.groupdocs.app/signature/family) website.  
        The live demo has the following benefits
        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-otp"
          title: "About OTP File Format"
          content: |
            Files with .OTP extension represent presentation template files created by applications in OASIS OpenDocument standard format. The contents of such a file include presentation information in the form of slides with text, images, shapes, multimedia content, transition effects and other slide elements. These template files are used for creating new presentations quickly based on the styling information stored in the template itself. OTP files can be created and saved with several different applications such as Impress that comes with OpenOffice suite and Microsoft PowerPoint. The OTP file format is similar to Microsoft PowerPoint template files .POT and .POTX.

          link: "https://docs.fileformat.com/presentation/otp/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Editing Signatures From Other Digital Document Formats"
    content: |
        Multi format documents and images signatures editing API for .NET. Update signatures from some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Edit e-Signatures from PDF"
          link: "https://products.groupdocs.com/signature/net/edit/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Edit e-Signatures from DOC"
          link: "https://products.groupdocs.com/signature/net/edit/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Edit e-Signatures from DOCM"
          link: "https://products.groupdocs.com/signature/net/edit/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Edit e-Signatures from DOCX"
          link: "https://products.groupdocs.com/signature/net/edit/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Edit e-Signatures from DOT"
          link: "https://products.groupdocs.com/signature/net/edit/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Edit e-Signatures from DOTX"
          link: "https://products.groupdocs.com/signature/net/edit/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Edit e-Signatures from DOTM"
          link: "https://products.groupdocs.com/signature/net/edit/dotm/"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Edit e-Signatures from RTF"
          link: "https://products.groupdocs.com/signature/net/edit/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Edit e-Signatures from ODT"
          link: "https://products.groupdocs.com/signature/net/edit/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Edit e-Signatures from OTT"
          link: "https://products.groupdocs.com/signature/net/edit/ott/"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Edit e-Signatures from XLS"
          link: "https://products.groupdocs.com/signature/net/edit/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Edit e-Signatures from XLSX"
          link: "https://products.groupdocs.com/signature/net/edit/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Edit e-Signatures from XLSM"
          link: "https://products.groupdocs.com/signature/net/edit/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Edit e-Signatures from XLSM"
          link: "https://products.groupdocs.com/signature/net/edit/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Edit e-Signatures from XLSB"
          link: "https://products.groupdocs.com/signature/net/edit/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Edit e-Signatures from XLTX"
          link: "https://products.groupdocs.com/signature/net/edit/xltx/"
          description: "Microsoft Excel template"

        # format loop
        - name: "Edit e-Signatures from XLTM"
          link: "https://products.groupdocs.com/signature/net/edit/xltm/"
          description: "Microsoft Excel macro-enabled template"

        # format loop
        - name: "Edit e-Signatures from ODS"
          link: "https://products.groupdocs.com/signature/net/edit/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Edit e-Signatures from OTS"
          link: "https://products.groupdocs.com/signature/net/edit/ots/"
          description: "OpenDocument Spreadsheet Template"

        # format loop
        - name: "Edit e-Signatures from PPT"
          link: "https://products.groupdocs.com/signature/net/edit/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Edit e-Signatures from PPTX"
          link: "https://products.groupdocs.com/signature/net/edit/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Edit e-Signatures from PPS"
          link: "https://products.groupdocs.com/signature/net/edit/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Edit e-Signatures from PPSX"
          link: "https://products.groupdocs.com/signature/net/edit/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Edit e-Signatures from POTM"
          link: "https://products.groupdocs.com/signature/net/edit/potm/"
          description: "Microsoft PowerPoint Macro-Enabled Template"

        # format loop
        - name: "Edit e-Signatures from POTX"
          link: "https://products.groupdocs.com/signature/net/edit/potx/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Edit e-Signatures from PPTM"
          link: "https://products.groupdocs.com/signature/net/edit/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Edit e-Signatures from ODP"
          link: "https://products.groupdocs.com/signature/net/edit/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Edit e-Signatures from OTP"
          link: "https://products.groupdocs.com/signature/net/edit/otp/"
          description: "OpenDocument Presentation Template"

        # format loop
        - name: "Edit e-Signatures from WEBP"
          link: "https://products.groupdocs.com/signature/net/edit/webp/"
          description: "WebP Image"

        # format loop
        - name: "Edit e-Signatures from TIFF"
          link: "https://products.groupdocs.com/signature/net/edit/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Edit e-Signatures from JPEG"
          link: "https://products.groupdocs.com/signature/net/edit/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Edit e-Signatures from GIF"
          link: "https://products.groupdocs.com/signature/net/edit/gif/"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Edit e-Signatures from PNG"
          link: "https://products.groupdocs.com/signature/net/edit/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Edit e-Signatures from BMP"
          link: "https://products.groupdocs.com/signature/net/edit/bmp/"
          description: "Bitmap File Format"

        # format loop
        - name: "Edit e-Signatures from CDR"
          link: "https://products.groupdocs.com/signature/net/edit/cdr/"
          description: "CorelDraw Vector Graphic Drawing"

        # format loop
        - name: "Edit e-Signatures from SVG"
          link: "https://products.groupdocs.com/signature/net/edit/svg/"
          description: "Scalable Vector Graphics"

        # format loop
        - name: "Edit e-Signatures from PSD"
          link: "https://products.groupdocs.com/signature/net/edit/psd/"
          description: "Adobe Photoshop Document"

        # format loop
        - name: "Edit e-Signatures from WMF"
          link: "https://products.groupdocs.com/signature/net/edit/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Edit e-Signatures from EMF"
          link: "https://products.groupdocs.com/signature/net/edit/emf/"
          description: "Enhanced Metafile Format"

        # format loop
        - name: "Edit e-Signatures from CMX"
          link: "https://products.groupdocs.com/signature/net/edit/cmx/"
          description: "Corel Metafile eXchange Image"

        # format loop
        - name: "Edit e-Signatures from DJVU"
          link: "https://products.groupdocs.com/signature/net/edit/djvu/"
          description: "Deja Vu"

        # format loop
        - name: "Edit e-Signatures from PPSM"
          link: "https://products.groupdocs.com/signature/net/edit/ppsm/"
          description: "Microsoft PowerPoint Macro-Enabled Slide Show"

        # format loop
        - name: "Edit e-Signatures from DCM"
          link: "https://products.groupdocs.com/signature/net/edit/dcm/"
          description: "Digital Imaging and Communications in Medicine"


############################# Back to top ###############################
back_to_top:
    enable: true
---
