---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:20+03:00
draft: false

############################# Head ############################
head_title: "How to Verify Digital Signatures in POTX in Java"
head_description: "Learn how to verify digital signatures in a POTX file in Java using GroupDocs.Siganture API - add customized electronic signatures to popular business documents and image file formats."

############################# Header ############################
title: "Verify Digital Signatures in POTX via Java"
description: "Java library to verify all popular digital signature types within a POTX file. Easily manipulate potx properties and customize signing options within documents and images."
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
        [GroupDocs.Signature for Java](/signature/java/) is an advanced Java library to digitally sign documents using various signature types such as text, image, barcode, stamp, form-field, QR-code and metadata. By adding just a few lines of code, empower your Java applications with features to view, add, edit, validate, delete and search digital signatures within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats. The e-signature API also supports additional features to customize signature properties as per requirements.

############################# Steps ############################
steps:
    enable: true
    title_left: "How to Verify Digital Signatures in a POTX File"
    content_left: |
        The code example below clearly demonstrates the steps about **how to verify digital signatures in an already signed POTX file in Java** using [GroupDocs.Signature](/signature/java/) library by adding just a few lines of code.

        *   Create new instance of [Signature](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature) class and pass source document path as a constructor parameter.
        *   Instantiate the [DigitalVerifyOptions](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature.options.verify/DigitalVerifyOptions) object according to your requirements and specify verification options.
        *   Call [verify](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature#verify(com.groupdocs.signature.options.verify.VerifyOptions)) method of [Signature](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature) class and pass [DigitalVerifyOptions](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature.options.verify/DigitalVerifyOptions) to it.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for Java APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Signature for Java from [NuGet](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```java
        Signature signature = new Signature("sample.pdf");
        DigitalVerifyOptions options = new DigitalVerifyOptions(Constants.CertificatePfx);
        options.setComments("Test comment");
        options.setPassword("1234567890");
        
        // verify document signatures
        VerificationResult result = signature.verify(options);
        if (result.isValid())
        {
            System.out.print("\nDocument was verified successfully!");
        }
        else
        {
            System.out.print("\nDocument failed verification process.");
        }
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Verify POTX Signature Live Demos"
    content: |
        Add POTX file electronic signatures right now by visiting [GroupDocs.Signature Live Demos](https://products.groupdocs.app/signature/family) website.
        The live demo has the following benefits
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-potx"
          title: "What is POTX File Format"
          content: |
            Files with .POTX extension represent Microsoft PowerPoint template presentations that are created with Microsoft PowerPoint 2007 and above. This format was created to replace the POT file format that is based on the binary file format and is supported with PowerPoint 97-2003. The files generated can be used to create presentations that have same layout and other settings required to be applied to new files. These settings can include styles, backgrounds, colour palette, fonts and defaults. Such files are generated in order to create ready-to-use template files for official use. Learn more about POTX file format

          link: "https://docs.fileformat.com/presentation/potx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Other Available Options"
    content: |
        Multi-format digital signatures validation API for documents and images. Update signatures from some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Verify e-Signatures in PDF"
          link: "/signature/java/verify/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Verify e-Signatures in DOC"
          link: "/signature/java/verify/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Verify e-Signatures in DOCM"
          link: "/signature/java/verify/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Verify e-Signatures in DOCX"
          link: "/signature/java/verify/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Verify e-Signatures in DOT"
          link: "/signature/java/verify/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Verify e-Signatures in DOTX"
          link: "/signature/java/verify/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Verify e-Signatures in DOTM"
          link: "/signature/java/verify/dotm/"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Verify e-Signatures in RTF"
          link: "/signature/java/verify/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Verify e-Signatures in ODT"
          link: "/signature/java/verify/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Verify e-Signatures in OTT"
          link: "/signature/java/verify/ott/"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Verify e-Signatures in XLS"
          link: "/signature/java/verify/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Verify e-Signatures in XLSX"
          link: "/signature/java/verify/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Verify e-Signatures in XLSM"
          link: "/signature/java/verify/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Verify e-Signatures in XLSM"
          link: "/signature/java/verify/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Verify e-Signatures in XLSB"
          link: "/signature/java/verify/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Verify e-Signatures in XLTX"
          link: "/signature/java/verify/xltx/"
          description: "Microsoft Excel template"

        # format loop
        - name: "Verify e-Signatures in XLTM"
          link: "/signature/java/verify/xltm/"
          description: "Microsoft Excel macro-enabled template"

        # format loop
        - name: "Verify e-Signatures in ODS"
          link: "/signature/java/verify/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Verify e-Signatures in OTS"
          link: "/signature/java/verify/ots/"
          description: "OpenDocument Spreadsheet Template"

        # format loop
        - name: "Verify e-Signatures in PPT"
          link: "/signature/java/verify/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Verify e-Signatures in PPTX"
          link: "/signature/java/verify/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Verify e-Signatures in PPS"
          link: "/signature/java/verify/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Verify e-Signatures in PPSX"
          link: "/signature/java/verify/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Verify e-Signatures in POTM"
          link: "/signature/java/verify/potm/"
          description: "Microsoft PowerPoint Macro-Enabled Template"

        # format loop
        - name: "Verify e-Signatures in POTX"
          link: "/signature/java/verify/potx/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Verify e-Signatures in PPTM"
          link: "/signature/java/verify/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Verify e-Signatures in ODP"
          link: "/signature/java/verify/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Verify e-Signatures in OTP"
          link: "/signature/java/verify/otp/"
          description: "OpenDocument Presentation Template"

        # format loop
        - name: "Verify e-Signatures in WEBP"
          link: "/signature/java/verify/webp/"
          description: "WebP Image"

        # format loop
        - name: "Verify e-Signatures in TIFF"
          link: "/signature/java/verify/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Verify e-Signatures in JPEG"
          link: "/signature/java/verify/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Verify e-Signatures in GIF"
          link: "/signature/java/verify/gif/"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Verify e-Signatures in PNG"
          link: "/signature/java/verify/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Verify e-Signatures in BMP"
          link: "/signature/java/verify/bmp/"
          description: "Bitmap File Format"

        # format loop
        - name: "Verify e-Signatures in CDR"
          link: "/signature/java/verify/cdr/"
          description: "CorelDraw Vector Graphic Drawing"

        # format loop
        - name: "Verify e-Signatures in SVG"
          link: "/signature/java/verify/svg/"
          description: "Scalable Vector Graphics"

        # format loop
        - name: "Verify e-Signatures in PSD"
          link: "/signature/java/verify/psd/"
          description: "Adobe Photoshop Document"

        # format loop
        - name: "Verify e-Signatures in WMF"
          link: "/signature/java/verify/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Verify e-Signatures in EMF"
          link: "/signature/java/verify/emf/"
          description: "Enhanced Metafile Format"

        # format loop
        - name: "Verify e-Signatures in CMX"
          link: "/signature/java/verify/cmx/"
          description: "Corel Metafile eXchange Image"

        # format loop
        - name: "Verify e-Signatures in DJVU"
          link: "/signature/java/verify/djvu/"
          description: "Deja Vu"

        # format loop
        - name: "Verify e-Signatures in PPSM"
          link: "/signature/java/verify/ppsm/"
          description: "Microsoft PowerPoint Macro-Enabled Slide Show"

        # format loop
        - name: "Verify e-Signatures in DCM"
          link: "/signature/java/verify/dcm/"
          description: "Digital Imaging and Communications in Medicine"


############################# Back to top ###############################
back_to_top:
    enable: true
---
