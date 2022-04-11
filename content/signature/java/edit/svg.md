---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:02+03:00
draft: false

############################# Head ############################
head_title: "Java Code Example to View &amp; Edit Digital Signatures from SVG Files"
head_description: "Java code example to view and edit digital signatures from a SVG file using GroupDocs.Siganture API - add customized electronic signatures to popular business documents and image file formats."

############################# Header ############################
title: "Edit Digital Signatures in SVG via Java"
description: "Java library to view &amp; edit digital signatures in a SVG file using popular electronic signature types. Manage svg properties and customize signing options within documents and images."
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
        [GroupDocs.Signature for Java](/signature/java/) is an advanced Java library to digitally sign documents using various signature types such as text, image, barcode, stamp, form-field, QR-code and metadata. By adding just a few lines of code, empower your Java applications with features to view, add, update, validate, remove and search digital signatures within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats. The e-signature API also supports additional features to customize signature properties as per requirements.

############################# Steps ############################
steps:
    enable: true
    title_left: "How to Edit Digital Signatures in SVG"
    content_left: |
        The code example below clearly demonstrates the steps about **how to edit digital signatures in an already signed SVG file in Java** using [GroupDocs.Signature](/signature/java/) library by adding just a few lines of code.

        *   Create new instance of [Signature](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature/Signature) class and pass source document path as a constructor parameter.
        *   Instantiate [ImageSearchOptions](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature.options.search/ImageSearchOptions) object with desired properties.
        *   Call [search](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature/Signature#search(java.lang.Class,%20com.groupdocs.signature.options.search.SearchOptions)) method to obtain list of [ImageSignatures](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature.domain.signatures/ImageSignature).
        *   Select from list [ImageSignature](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature.domain.signatures/ImageSignature) object(s) that should be updated.
        *   Call [Signature](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature/Signature) object [update](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature/Signature#update(java.io.OutputStream,%20com.groupdocs.signature.domain.signatures.BaseSignature)) method and pass one or several signatures to it.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for Java APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Signature for Java from [NuGet](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```java
        Signature signature = new Signature("sampleSigned.pdf");
        try 
        {
            ImageSearchOptions options = new ImageSearchOptions();
        
            // search for image signatures in document
            List signatures = signature.search(ImageSignature.class,options);
            if (signatures.size() > 0)
            {
                ImageSignature imageSignature = signatures.get(0);
                imageSignature.setLeft(100);
                imageSignature.setTop(100);
                boolean result = signature.update("sampleSigned-output.svg",imageSignature);
                if (result)
                {
                    System.out.print("Image signature at location " + imageSignature.getLeft() + "x" + imageSignature.getTop() + " and Size " + imageSignature.getSize() + " was updated in the document [" + fileName + ".");
                }
                else
                {
                    System.out.print("Signature was not updated in the document! Signature at location " + imageSignature.getLeft() + "x" + imageSignature.getTop() + " and Size " + imageSignature.getSize() + " was not found!");
                }
            }
        } catch (Exception e) {
            throw new GroupDocsSignatureException(e.getMessage());
        }
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Edit SVG Signature Live Demos"
    content: |
        Add SVG file electronic signatures right now by visiting [GroupDocs.Signature Live Demos](https://products.groupdocs.app/signature/family) website.
        The live demo has the following benefits
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-svg"
          title: "What is SVG File Format"
          content: |
            SVG files are Scalable Vector Graphics Files that use XML based text format for describing the appearance of image. The word Scalable refers to the fact that the SVG can be scaled to different sizes without losing any quality. Text based description of such files make them independent of resolution. It is one of the mostly used format for building website and print graphics in order to achieve scalability. The format can only be used for two-dimensional graphics though. SVG files can be viewed/opened in almost all modern browsers including Chrome, Internet Explorer, Firefox, and Safari. Learn more about SVG file format

          link: "https://docs.fileformat.com/page-description-language/svg/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Other Available Options"
    content: |
        Multi-format digital signatures editing API for documents and images. Update signatures from some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Edit e-Signatures from PDF"
          link: "/signature/java/edit/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Edit e-Signatures from DOC"
          link: "/signature/java/edit/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Edit e-Signatures from DOCM"
          link: "/signature/java/edit/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Edit e-Signatures from DOCX"
          link: "/signature/java/edit/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Edit e-Signatures from DOT"
          link: "/signature/java/edit/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Edit e-Signatures from DOTX"
          link: "/signature/java/edit/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Edit e-Signatures from DOTM"
          link: "/signature/java/edit/dotm/"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Edit e-Signatures from RTF"
          link: "/signature/java/edit/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Edit e-Signatures from ODT"
          link: "/signature/java/edit/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Edit e-Signatures from OTT"
          link: "/signature/java/edit/ott/"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Edit e-Signatures from XLS"
          link: "/signature/java/edit/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Edit e-Signatures from XLSX"
          link: "/signature/java/edit/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Edit e-Signatures from XLSM"
          link: "/signature/java/edit/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Edit e-Signatures from XLSM"
          link: "/signature/java/edit/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Edit e-Signatures from XLSB"
          link: "/signature/java/edit/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Edit e-Signatures from XLTX"
          link: "/signature/java/edit/xltx/"
          description: "Microsoft Excel template"

        # format loop
        - name: "Edit e-Signatures from XLTM"
          link: "/signature/java/edit/xltm/"
          description: "Microsoft Excel macro-enabled template"

        # format loop
        - name: "Edit e-Signatures from ODS"
          link: "/signature/java/edit/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Edit e-Signatures from OTS"
          link: "/signature/java/edit/ots/"
          description: "OpenDocument Spreadsheet Template"

        # format loop
        - name: "Edit e-Signatures from PPT"
          link: "/signature/java/edit/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Edit e-Signatures from PPTX"
          link: "/signature/java/edit/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Edit e-Signatures from PPS"
          link: "/signature/java/edit/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Edit e-Signatures from PPSX"
          link: "/signature/java/edit/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Edit e-Signatures from POTM"
          link: "/signature/java/edit/potm/"
          description: "Microsoft PowerPoint Macro-Enabled Template"

        # format loop
        - name: "Edit e-Signatures from POTX"
          link: "/signature/java/edit/potx/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Edit e-Signatures from PPTM"
          link: "/signature/java/edit/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Edit e-Signatures from ODP"
          link: "/signature/java/edit/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Edit e-Signatures from OTP"
          link: "/signature/java/edit/otp/"
          description: "OpenDocument Presentation Template"

        # format loop
        - name: "Edit e-Signatures from WEBP"
          link: "/signature/java/edit/webp/"
          description: "WebP Image"

        # format loop
        - name: "Edit e-Signatures from TIFF"
          link: "/signature/java/edit/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Edit e-Signatures from JPEG"
          link: "/signature/java/edit/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Edit e-Signatures from GIF"
          link: "/signature/java/edit/gif/"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Edit e-Signatures from PNG"
          link: "/signature/java/edit/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Edit e-Signatures from BMP"
          link: "/signature/java/edit/bmp/"
          description: "Bitmap File Format"

        # format loop
        - name: "Edit e-Signatures from CDR"
          link: "/signature/java/edit/cdr/"
          description: "CorelDraw Vector Graphic Drawing"

        # format loop
        - name: "Edit e-Signatures from SVG"
          link: "/signature/java/edit/svg/"
          description: "Scalable Vector Graphics"

        # format loop
        - name: "Edit e-Signatures from PSD"
          link: "/signature/java/edit/psd/"
          description: "Adobe Photoshop Document"

        # format loop
        - name: "Edit e-Signatures from WMF"
          link: "/signature/java/edit/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Edit e-Signatures from EMF"
          link: "/signature/java/edit/emf/"
          description: "Enhanced Metafile Format"

        # format loop
        - name: "Edit e-Signatures from CMX"
          link: "/signature/java/edit/cmx/"
          description: "Corel Metafile eXchange Image"

        # format loop
        - name: "Edit e-Signatures from DJVU"
          link: "/signature/java/edit/djvu/"
          description: "Deja Vu"

        # format loop
        - name: "Edit e-Signatures from PPSM"
          link: "/signature/java/edit/ppsm/"
          description: "Microsoft PowerPoint Macro-Enabled Slide Show"

        # format loop
        - name: "Edit e-Signatures from DCM"
          link: "/signature/java/edit/dcm/"
          description: "Digital Imaging and Communications in Medicine"


############################# Back to top ###############################
back_to_top:
    enable: true
---
