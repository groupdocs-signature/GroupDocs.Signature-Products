---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:12+03:00
draft: false

############################# Head ############################
head_title: "Search Digital Signatures in J2K via Java Library"
head_description: "Java library to search &amp; validate digital signatures in a J2K file using GroupDocs.Siganture API - manipulate Image, Barcode, QR-Code, Stamp, Text, Optical &amp; Metadata signatures from digitally signed documents."

############################# Header ############################
title: "Search Digital Signature in J2K via Java"
description: "Java eSignature API to search &amp; validate digital signatures in a J2K file. Manipulate Image, Barcode, QR-Code, Stamp, Text, Optical &amp; Metadata signatures from digitally signed documents."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download Free Trial"
    link: "https://downloads.groupdocs.com/signature/java"

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:

            # button loop
            - link: "https://apireference.groupdocs.com/signature/java"
              text: "API Reference"

            # button loop
            - link: "https://github.com/groupdocs-signature"
              text: "Code Examples"

            # button loop
            - link: "https://products.groupdocs.app/signature/family"
              text: "Live Demos"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java"
        link_buy: "https://purchase.groupdocs.com"

############################# About ############################
about:
    enable: true
    title: "About GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](/signature/java/) is an advanced Java eSignature library to digitally sign documents using various signature signature types such as text, image, barcode, stamp, form-field, QR-code and metadata. By adding just a few lines of code, empower your Java applications with features to view, create, edit, validate, remove and find digital signatures within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats. The e-signature API also supports additional features to customize signature properties as per requirements.

############################# Steps ############################
steps:
    enable: true
    title_left: "How to Search Digital Signatures from J2K"
    content_left: |
        Below Java code example clearly demonstrates the steps to **search for digital signatures within a J2K file in Java** by adding just a few lines of code.

        *   Create new instance of **Signature** class and pass source document path as a constructor parameter.
        *   Instantiate the **DigitalSearchOptions** object according to your requirements and specify search options.
        *   Call **search** method of **Signature** class instance and pass **DigitalSearchOptions** to it.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for Java APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Signature for Java from [NuGet](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```java
        Signature signature = new Signature("signed.pdf");
        DigitalSearchOptions options = new DigitalSearchOptions();
        // specify special search criteria
        options.setComments("Test comment");
        // certificate issues criteria
        options.setIssuerName("John");
        // digital certificate subject
        options.setSubjectName("Test");
        // specify date range period of signature
        options.setSignDateTimeFrom(DateUtils.addMonths(new Date(), -1));
        options.setSignDateTimeTo(new Date());
         
        // search for signatures in document
        List signatures = signature.search(DigitalSignature.class, options);
        System.out.print("\nSource document contains following signatures.");
        for (DigitalSignature digitalSignature : signatures)
        {
            System.out.print("Digital signature found from "+digitalSignature.getSignTime()+" with validation flag "+digitalSignature.isValid()+". Certificate SN "+ digitalSignature.getCertificate().getType());
        }
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Search J2K Signature Live Demos"
    content: |
        Add J2K file electronic signatures right now by visiting [GroupDocs.Signature Live Demos](https://products.groupdocs.app/signature/family) website.
        The live demo has the following benefits
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-j2k"
          title: "What is J2K File Format"
          content: |
            A J2K file is an image that is compressed using the wavelet compression instead of DCT compression. This file format is used by the Joint Photographic Experts Group (JPEG) 2000 files. J2K files store metadata information about the image file in XML unlike .jpeg or .jpg that use the EXIF format for this purpose. J2K files support 15-bit color, alpha transparency, and lossless compression. Several commercial APIs exist to decode JPEG 2000 images such as J2K-Codec. A J2K file can be opened on Windows OS using the standard image viewers. Learn more about J2K file format

          link: "https://docs.fileformat.com/image/j2k/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Other Available Options"
    content: |
        Multi-format digital signatures searching API for documents and images. Find signatures from within some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Search Signatures in PDF"
          link: "/signature/java/search/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Search Signatures in DOC"
          link: "/signature/java/search/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Search Signatures in DOCM"
          link: "/signature/java/search/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Search Signatures in DOCX"
          link: "/signature/java/search/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Search Signatures in DOT"
          link: "/signature/java/search/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Search Signatures in DOTX"
          link: "/signature/java/search/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Search Signatures in DOTM"
          link: "/signature/java/search/dotm/"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Search Signatures in RTF"
          link: "/signature/java/search/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Search Signatures in ODT"
          link: "/signature/java/search/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Search Signatures in OTT"
          link: "/signature/java/search/ott/"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Search Signatures in XLS"
          link: "/signature/java/search/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Search Signatures in XLSX"
          link: "/signature/java/search/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Search Signatures in XLSM"
          link: "/signature/java/search/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Search Signatures in XLSM"
          link: "/signature/java/search/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Search Signatures in XLSB"
          link: "/signature/java/search/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Search Signatures in XLTX"
          link: "/signature/java/search/xltx/"
          description: "Microsoft Excel template"

        # format loop
        - name: "Search Signatures in XLTM"
          link: "/signature/java/search/xltm/"
          description: "Microsoft Excel macro-enabled template"

        # format loop
        - name: "Search Signatures in ODS"
          link: "/signature/java/search/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Search Signatures in OTS"
          link: "/signature/java/search/ots/"
          description: "OpenDocument Spreadsheet Template"

        # format loop
        - name: "Search Signatures in PPT"
          link: "/signature/java/search/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Search Signatures in PPTX"
          link: "/signature/java/search/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Search Signatures in PPS"
          link: "/signature/java/search/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Search Signatures in PPSX"
          link: "/signature/java/search/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Search Signatures in POTM"
          link: "/signature/java/search/potm/"
          description: "Microsoft PowerPoint Macro-Enabled Template"

        # format loop
        - name: "Search Signatures in POTX"
          link: "/signature/java/search/potx/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Search Signatures in PPTM"
          link: "/signature/java/search/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Search Signatures in ODP"
          link: "/signature/java/search/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Search Signatures in OTP"
          link: "/signature/java/search/otp/"
          description: "OpenDocument Presentation Template"

        # format loop
        - name: "Search Signatures in WEBP"
          link: "/signature/java/search/webp/"
          description: "WebP Image"

        # format loop
        - name: "Search Signatures in TIFF"
          link: "/signature/java/search/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Search Signatures in JPEG"
          link: "/signature/java/search/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Search Signatures in GIF"
          link: "/signature/java/search/gif/"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Search Signatures in PNG"
          link: "/signature/java/search/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Search Signatures in BMP"
          link: "/signature/java/search/bmp/"
          description: "Bitmap File Format"

        # format loop
        - name: "Search Signatures in CDR"
          link: "/signature/java/search/cdr/"
          description: "CorelDraw Vector Graphic Drawing"

        # format loop
        - name: "Search Signatures in SVG"
          link: "/signature/java/search/svg/"
          description: "Scalable Vector Graphics"

        # format loop
        - name: "Search Signatures in PSD"
          link: "/signature/java/search/psd/"
          description: "Adobe Photoshop Document"

        # format loop
        - name: "Search Signatures in WMF"
          link: "/signature/java/search/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Search Signatures in EMF"
          link: "/signature/java/search/emf/"
          description: "Enhanced Metafile Format"

        # format loop
        - name: "Search Signatures in CMX"
          link: "/signature/java/search/cmx/"
          description: "Corel Metafile eXchange Image"

        # format loop
        - name: "Search Signatures in DJVU"
          link: "/signature/java/search/djvu/"
          description: "Deja Vu"

        # format loop
        - name: "Search Signatures in PPSM"
          link: "/signature/java/search/ppsm/"
          description: "Microsoft PowerPoint Macro-Enabled Slide Show"

        # format loop
        - name: "Search Signatures in DCM"
          link: "/signature/java/search/dcm/"
          description: "Digital Imaging and Communications in Medicine"


############################# Back to top ###############################
back_to_top:
    enable: true
---
