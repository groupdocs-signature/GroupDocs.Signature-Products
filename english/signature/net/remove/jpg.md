---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:40+03:00
draft: false

############################# Head ############################
head_title: "Find &amp; Remove Digital Signatures in a JPG file in C# .NET"
head_description: "C# .NET API to find &amp; remove digital signatures in a signed JPG file, other images and document file formats using a few lines of code."

############################# Header ############################
title: "Remove Digital Signatures in a JPG File"
description: "C# .NET digital signature API to find &amp; remove e-signatures from digitally signed JPG files by adding just a few lines of code. Sign documents with one or several signature types at the same time as you may require."
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
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net) is an advanced .NET API to electronically sign digital documents using various signature types such as text, image, barcode, stamp, form-field, QR-code and metadata. Users can easily view, edit, validate, save, delete, find and preview digital signatures within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats, with additional support for customizing signature properties as needed.

############################# Steps ############################
steps:
    enable: true
    title_left: "How to Remove Signatures in a JPG File"
    content_left: |
        [GroupDocs.Signature](https://products.groupdocs.com/signature/net) makes it easy for .NET developers to locate & remove digital signatures in a JPG file from within their applications by implementing a few easy steps.

        *   Create new instance of Signature class and pass source document path or its stream as a constructor parameter.
        *   Instantiate DigitalSearchOptions object with desired properties.
        *   Call Search method to obtain list of DigitalSignatures.
        *   Select from list DigitalSignature object(s) that should be removed from the document.
        *   Call Signature object Delete method and pass one or several signatures to it.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installled on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```cs
        using (Signature signature = new Signature("signed.jpg"))
        {
            // search for electronic Digital signatures in the document
            List signatures = signature.Search(SignatureType.Digital);
            if (signatures.Count > 0)
            {
                DigitalSignature digitalSignature = signatures[0];
                bool result = signature.Delete(digitalSignature);
                if (result)
                {
                    Console.WriteLine($"Digital signature #{digitalSignature.Thumbprint} from {digitalSignature.SignTime.ToShortDateString()} was deleted.");
                }
                else
                {
                    Helper.WriteError($"Signature was not deleted from the document! Signature# {digitalSignature.Thumbprint} was not found!");
                }
            }
        }
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Remove JPG Signature Live Demos"
    content: |
        Add JPG file electronic signatures right now by visiting [GroupDocs.Signature Live Demos](https://products.groupdocs.app/signature/family) website.
        The live demo has the following benefits
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-jpg"
          title: "What is JPG File Format"
          content: |
            A JPEG is a type of image format that is saved using the method of lossy compression. The output image, as result of compression, is a trade-off between storage size and image quality. Users can adjust the compression level to achieve the desired quality level while at the same time reduce the storage size. Image quality is negligibly affected if 10:1 compression is applied to the image. The higher the compression value, the higher the degradation in image quality. Learn more about JPG file format

          link: "https://docs.fileformat.com/image/jpeg/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Other Available Options"
    content: |
        Multi format digital-signatures deletion API for documents and images. Remove signatures from some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Remove e-Signatures in PDF"
          link: "https://products.groupdocs.com/signature/net/remove/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Remove e-Signatures in DOC"
          link: "https://products.groupdocs.com/signature/net/remove/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Remove e-Signatures in DOCM"
          link: "https://products.groupdocs.com/signature/net/remove/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Remove e-Signatures in DOCX"
          link: "https://products.groupdocs.com/signature/net/remove/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Remove e-Signatures in DOT"
          link: "https://products.groupdocs.com/signature/net/remove/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Remove e-Signatures in DOTX"
          link: "https://products.groupdocs.com/signature/net/remove/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Remove e-Signatures in DOTM"
          link: "https://products.groupdocs.com/signature/net/remove/dotm/"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Remove e-Signatures in RTF"
          link: "https://products.groupdocs.com/signature/net/remove/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Remove e-Signatures in ODT"
          link: "https://products.groupdocs.com/signature/net/remove/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Remove e-Signatures in OTT"
          link: "https://products.groupdocs.com/signature/net/remove/ott/"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Remove e-Signatures in XLS"
          link: "https://products.groupdocs.com/signature/net/remove/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Remove e-Signatures in XLSX"
          link: "https://products.groupdocs.com/signature/net/remove/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Remove e-Signatures in XLSM"
          link: "https://products.groupdocs.com/signature/net/remove/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Remove e-Signatures in XLSM"
          link: "https://products.groupdocs.com/signature/net/remove/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Remove e-Signatures in XLSB"
          link: "https://products.groupdocs.com/signature/net/remove/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Remove e-Signatures in XLTX"
          link: "https://products.groupdocs.com/signature/net/remove/xltx/"
          description: "Microsoft Excel template"

        # format loop
        - name: "Remove e-Signatures in XLTM"
          link: "https://products.groupdocs.com/signature/net/remove/xltm/"
          description: "Microsoft Excel macro-enabled template"

        # format loop
        - name: "Remove e-Signatures in ODS"
          link: "https://products.groupdocs.com/signature/net/remove/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Remove e-Signatures in OTS"
          link: "https://products.groupdocs.com/signature/net/remove/ots/"
          description: "OpenDocument Spreadsheet Template"

        # format loop
        - name: "Remove e-Signatures in PPT"
          link: "https://products.groupdocs.com/signature/net/remove/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Remove e-Signatures in PPTX"
          link: "https://products.groupdocs.com/signature/net/remove/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Remove e-Signatures in PPS"
          link: "https://products.groupdocs.com/signature/net/remove/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Remove e-Signatures in PPSX"
          link: "https://products.groupdocs.com/signature/net/remove/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Remove e-Signatures in POTM"
          link: "https://products.groupdocs.com/signature/net/remove/potm/"
          description: "Microsoft PowerPoint Macro-Enabled Template"

        # format loop
        - name: "Remove e-Signatures in POTX"
          link: "https://products.groupdocs.com/signature/net/remove/potx/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Remove e-Signatures in PPTM"
          link: "https://products.groupdocs.com/signature/net/remove/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Remove e-Signatures in ODP"
          link: "https://products.groupdocs.com/signature/net/remove/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Remove e-Signatures in OTP"
          link: "https://products.groupdocs.com/signature/net/remove/otp/"
          description: "OpenDocument Presentation Template"

        # format loop
        - name: "Remove e-Signatures in WEBP"
          link: "https://products.groupdocs.com/signature/net/remove/webp/"
          description: "WebP Image"

        # format loop
        - name: "Remove e-Signatures in TIFF"
          link: "https://products.groupdocs.com/signature/net/remove/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Remove e-Signatures in JPEG"
          link: "https://products.groupdocs.com/signature/net/remove/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Remove e-Signatures in GIF"
          link: "https://products.groupdocs.com/signature/net/remove/gif/"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Remove e-Signatures in PNG"
          link: "https://products.groupdocs.com/signature/net/remove/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Remove e-Signatures in BMP"
          link: "https://products.groupdocs.com/signature/net/remove/bmp/"
          description: "Bitmap File Format"

        # format loop
        - name: "Remove e-Signatures in CDR"
          link: "https://products.groupdocs.com/signature/net/remove/cdr/"
          description: "CorelDraw Vector Graphic Drawing"

        # format loop
        - name: "Remove e-Signatures in SVG"
          link: "https://products.groupdocs.com/signature/net/remove/svg/"
          description: "Scalable Vector Graphics"

        # format loop
        - name: "Remove e-Signatures in PSD"
          link: "https://products.groupdocs.com/signature/net/remove/psd/"
          description: "Adobe Photoshop Document"

        # format loop
        - name: "Remove e-Signatures in WMF"
          link: "https://products.groupdocs.com/signature/net/remove/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Remove e-Signatures in EMF"
          link: "https://products.groupdocs.com/signature/net/remove/emf/"
          description: "Enhanced Metafile Format"

        # format loop
        - name: "Remove e-Signatures in CMX"
          link: "https://products.groupdocs.com/signature/net/remove/cmx/"
          description: "Corel Metafile eXchange Image"

        # format loop
        - name: "Remove e-Signatures in DJVU"
          link: "https://products.groupdocs.com/signature/net/remove/djvu/"
          description: "Deja Vu"

        # format loop
        - name: "Remove e-Signatures in PPSM"
          link: "https://products.groupdocs.com/signature/net/remove/ppsm/"
          description: "Microsoft PowerPoint Macro-Enabled Slide Show"

        # format loop
        - name: "Remove e-Signatures in DCM"
          link: "https://products.groupdocs.com/signature/net/remove/dcm/"
          description: "Digital Imaging and Communications in Medicine"


############################# Back to top ###############################
back_to_top:
    enable: true
---
