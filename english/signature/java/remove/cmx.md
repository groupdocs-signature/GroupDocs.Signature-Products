---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:04+03:00
draft: false

############################# Head ############################
head_title: "Remove Digital Signatures from CMX in Java"
head_description: "Java library to clear &amp; remove digital signatures from CMX file using GroupDocs.Signature API - manipulate Image, Barcode, QR-Code, Stamp, Text, Optical &amp; Metadata signatures from digitally signed documents."

############################# Header ############################
title: "Remove Digital Signature from CMX via Java"
description: "Java eSignature library to remove digital signatures from CMX file. Easily manipulate Image, Barcode, QR-Code, Stamp, Text, Optical and Metadata signatures from digitally signed documents."
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
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java) is an advanced Java eSignature library to digitally sign documents using various signature signature types such as text, image, barcode, stamp, form-field, QR-code and metadata. By adding just a few lines of code, empower your Java applications with features to view, add, edit, validate, delete and search digital signatures within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats. The e-signature API also supports additional features to customize signature properties as per requirements.

############################# Steps ############################
steps:
    enable: true
    title_left: "How to Remove Digital Signatures from CMX"
    content_left: |
        Below Java code example clearly demonstrates the steps to **delete text signatures from CMX file in Java** by adding just a few lines of code.

        *   Create new instance of **Signature** class and pass source document path as a constructor parameter.
        *   Instantiate **TextSearchOptions** object with desired properties.
        *   Call **search** method to obtain list of **TextSignatures**.
        *   Select the **TextSignature** object(s) that should be removed from the document.
        *   Call **Signature** object **delete** method, pass one or several signatures to it.
        *   Analyze **DeleteResult** results to confirm signatures were updated or not.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for Java APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installled on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Signature for Java from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```java
        // initialize Signature instance
        Signature signature = new Signature("signed.pdf");
         
        TextSearchOptions options = new TextSearchOptions();
         
        List signatures = signature.search(TextSignature.class,options);
        List signaturesToDelete = new ArrayList();
        // collect signatures to delete
        for (TextSignature temp : signatures)
        {
            if (temp.getText().contains("JS"))
            {
                signaturesToDelete.add(temp);
            }
        }
        // delete signatures
        DeleteResult deleteResult = signature.delete("signed.cmx", signaturesToDelete);
        if (deleteResult.getSucceeded().size() == signaturesToDelete.size())
        {
            System.out.print("All signatures were successfully deleted!");
        }
        else
        {
            System.out.print("Successfully deleted signatures : " + deleteResult.getSucceeded().size());
            System.out.print("Not deleted signatures : " + deleteResult.getFailed().size());
        }
        System.out.print("List of deleted signatures:");
        for(BaseSignature temp : deleteResult.getSucceeded())
        {
            System.out.print("Signature# Id:"+temp.getSignatureId()+", Location: "+temp.getLeft()+"x"+temp.getTop()+". Size: "+temp.getWidth()+"x"+temp.getHeight());
        }
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Remove CMX Signature Live Demos"
    content: |
        Add CMX file electronic signatures right now by visiting [GroupDocs.Signature Live Demos](https://products.groupdocs.app/signature/family) website.
        The live demo has the following benefits
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-cmx"
          title: "What is CMX File Format"
          content: |
            Files with CMX extension are Corel Exchange image file format that is used as presentation by CorelSuite applications. It contains image data as vector graphics as well as metadata that describes the image. CMX files can be opened by CorelDraw, Corel Presentations, Paint Shop Pro and some versions of Adobe Illustrator. Learn more about CMX file format

          link: "https://docs.fileformat.com/image/cmx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Other Available Options"
    content: |
        Multi-format digital signatures deletion API for documents and images. Remove signatures from some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Remove Signatures from PDF"
          link: "https://products.groupdocs.com/signature/java/remove/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Remove Signatures from DOC"
          link: "https://products.groupdocs.com/signature/java/remove/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Remove Signatures from DOCM"
          link: "https://products.groupdocs.com/signature/java/remove/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Remove Signatures from DOCX"
          link: "https://products.groupdocs.com/signature/java/remove/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Remove Signatures from DOT"
          link: "https://products.groupdocs.com/signature/java/remove/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Remove Signatures from DOTX"
          link: "https://products.groupdocs.com/signature/java/remove/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Remove Signatures from DOTM"
          link: "https://products.groupdocs.com/signature/java/remove/dotm/"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Remove Signatures from RTF"
          link: "https://products.groupdocs.com/signature/java/remove/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Remove Signatures from ODT"
          link: "https://products.groupdocs.com/signature/java/remove/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Remove Signatures from OTT"
          link: "https://products.groupdocs.com/signature/java/remove/ott/"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Remove Signatures from XLS"
          link: "https://products.groupdocs.com/signature/java/remove/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Remove Signatures from XLSX"
          link: "https://products.groupdocs.com/signature/java/remove/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Remove Signatures from XLSM"
          link: "https://products.groupdocs.com/signature/java/remove/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Remove Signatures from XLSM"
          link: "https://products.groupdocs.com/signature/java/remove/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Remove Signatures from XLSB"
          link: "https://products.groupdocs.com/signature/java/remove/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Remove Signatures from XLTX"
          link: "https://products.groupdocs.com/signature/java/remove/xltx/"
          description: "Microsoft Excel template"

        # format loop
        - name: "Remove Signatures from XLTM"
          link: "https://products.groupdocs.com/signature/java/remove/xltm/"
          description: "Microsoft Excel macro-enabled template"

        # format loop
        - name: "Remove Signatures from ODS"
          link: "https://products.groupdocs.com/signature/java/remove/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Remove Signatures from OTS"
          link: "https://products.groupdocs.com/signature/java/remove/ots/"
          description: "OpenDocument Spreadsheet Template"

        # format loop
        - name: "Remove Signatures from PPT"
          link: "https://products.groupdocs.com/signature/java/remove/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Remove Signatures from PPTX"
          link: "https://products.groupdocs.com/signature/java/remove/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Remove Signatures from PPS"
          link: "https://products.groupdocs.com/signature/java/remove/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Remove Signatures from PPSX"
          link: "https://products.groupdocs.com/signature/java/remove/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Remove Signatures from POTM"
          link: "https://products.groupdocs.com/signature/java/remove/potm/"
          description: "Microsoft PowerPoint Macro-Enabled Template"

        # format loop
        - name: "Remove Signatures from POTX"
          link: "https://products.groupdocs.com/signature/java/remove/potx/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Remove Signatures from PPTM"
          link: "https://products.groupdocs.com/signature/java/remove/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Remove Signatures from ODP"
          link: "https://products.groupdocs.com/signature/java/remove/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Remove Signatures from OTP"
          link: "https://products.groupdocs.com/signature/java/remove/otp/"
          description: "OpenDocument Presentation Template"

        # format loop
        - name: "Remove Signatures from WEBP"
          link: "https://products.groupdocs.com/signature/java/remove/webp/"
          description: "WebP Image"

        # format loop
        - name: "Remove Signatures from TIFF"
          link: "https://products.groupdocs.com/signature/java/remove/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Remove Signatures from JPEG"
          link: "https://products.groupdocs.com/signature/java/remove/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Remove Signatures from GIF"
          link: "https://products.groupdocs.com/signature/java/remove/gif/"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Remove Signatures from PNG"
          link: "https://products.groupdocs.com/signature/java/remove/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Remove Signatures from BMP"
          link: "https://products.groupdocs.com/signature/java/remove/bmp/"
          description: "Bitmap File Format"

        # format loop
        - name: "Remove Signatures from CDR"
          link: "https://products.groupdocs.com/signature/java/remove/cdr/"
          description: "CorelDraw Vector Graphic Drawing"

        # format loop
        - name: "Remove Signatures from SVG"
          link: "https://products.groupdocs.com/signature/java/remove/svg/"
          description: "Scalable Vector Graphics"

        # format loop
        - name: "Remove Signatures from PSD"
          link: "https://products.groupdocs.com/signature/java/remove/psd/"
          description: "Adobe Photoshop Document"

        # format loop
        - name: "Remove Signatures from WMF"
          link: "https://products.groupdocs.com/signature/java/remove/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Remove Signatures from EMF"
          link: "https://products.groupdocs.com/signature/java/remove/emf/"
          description: "Enhanced Metafile Format"

        # format loop
        - name: "Remove Signatures from CMX"
          link: "https://products.groupdocs.com/signature/java/remove/cmx/"
          description: "Corel Metafile eXchange Image"

        # format loop
        - name: "Remove Signatures from DJVU"
          link: "https://products.groupdocs.com/signature/java/remove/djvu/"
          description: "Deja Vu"

        # format loop
        - name: "Remove Signatures from PPSM"
          link: "https://products.groupdocs.com/signature/java/remove/ppsm/"
          description: "Microsoft PowerPoint Macro-Enabled Slide Show"

        # format loop
        - name: "Remove Signatures from DCM"
          link: "https://products.groupdocs.com/signature/java/remove/dcm/"
          description: "Digital Imaging and Communications in Medicine"


############################# Back to top ###############################
back_to_top:
    enable: true
---
