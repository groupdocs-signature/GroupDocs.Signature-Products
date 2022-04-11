---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:24+03:00
draft: false

############################# Head ############################
head_title: "Sign J2C files with Image Signatures in Java"
head_description: "Add image signatures to digitally sign J2C documents in Java - add customized electronic signatures to popular business documents and image file formats."

############################# Header ############################
title: "Add Image Signatures to J2C Files In Java"
description: "Add digital signatures to your J2C files using popular image signature types. Securely add customized image signatures by manipulating the signature properties - set up advance signing options within documents that suit your needs."
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
        [GroupDocs.Signature for Java](/signature/java/) is a native Java API to electronically sign digital documents using various signature types such as text, image, barcode, stamp, form-field, QR-code and metadata. Users can add, update, validate, remove and search digital signatures within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, OpenDocument, metafiles and image file formats with additional support for customizing signature properties as needed.

############################# Steps ############################
steps:
    enable: true
    title_left: "How to Add Image Signatures to J2C"
    content_left: |
        [GroupDocs.Signature](/signature/java/) makes it easy for Java developers to add image signatures to J2C files within their applications by implementing a few easy steps.

        *   Create new instance of Signature class and pass source document path as a constructor parameter.
        *   Instantiate the ImageSignOptions object according to your requirements and specify Image signature options.
        *   Call Sign method of Signature class instance and pass ImageSignOptions to it.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for Java APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: NetBeans, IntelliJ IDEA, Eclipse
        *   Frameworks: Java 7 (1.7) and above
        *   Download the latest version of GroupDocs.Signature for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
        
    code: |
        ```cs
        Signature signature = new Signature("sample.j2c"))
        
        ImageSignOptions options = new ImageSignOptions("signature.jpg") ;
        
        // set signature position
        options.setLeft(100);
        options.setTop(100);

        // set page numbers
        options.setPageNumber(1);

        // sign document to file
        signature.sign("SampleSigned.j2c", options);
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Live Demos - Online App to Add Digital Signatures"
    content: |
        Add e-signatures to J2C files right now by visiting [GroupDocs.Signature Live Demos](https://products.groupdocs.app/signature/family) website.  
        The live demo has the following benefits
        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-image-o"
          title: "About J2C File Format"
          content: |
            A file with .j2c extension is a variant of JPEG file format and is compressed with the wavelet compression. It has nearly identical system of markers and segments to JPEG 2000 file format. The J2C file format is as defined in the Part 1 of the JPEG 2000 stand that supports both lossy and lossless compression. The JPEG 2000 codestream was designed to be embedded in JP2 or another file format, although it may appear in a file by itself. A J2C file can be opened using Adobe Photoshop 2020, Adobe Illustrator 2020, and Corel Paintshop Pro.

          link: "https://docs.fileformat.com/image/j2c/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Signing Other Digital Document Formats"
    content: |
        Java digital signatures management API for documents and images. Add image signatures to some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Add image signatures to PDF"
          link: "/signature/java/add/image/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Add image signatures to DOC"
          link: "/signature/java/add/image/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Add image signatures to DOCM"
          link: "/signature/java/add/image/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Add image signatures to DOCX"
          link: "/signature/java/add/image/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Add image signatures to DOT"
          link: "/signature/java/add/image/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Add image signatures to DOTX"
          link: "/signature/java/add/image/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Add image signatures to DOTM"
          link: "/signature/java/add/image/dotm/"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Add image signatures to RTF"
          link: "/signature/java/add/image/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Add image signatures to ODT"
          link: "/signature/java/add/image/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Add image signatures to OTT"
          link: "/signature/java/add/image/ott/"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Add image signatures to XLS"
          link: "/signature/java/add/image/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Add image signatures to XLSX"
          link: "/signature/java/add/image/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Add image signatures to XLSM"
          link: "/signature/java/add/image/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Add image signatures to XLSM"
          link: "/signature/java/add/image/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Add image signatures to XLSB"
          link: "/signature/java/add/image/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Add image signatures to XLTX"
          link: "/signature/java/add/image/xltx/"
          description: "Microsoft Excel template"

        # format loop
        - name: "Add image signatures to XLTM"
          link: "/signature/java/add/image/xltm/"
          description: "Microsoft Excel macro-enabled template"

        # format loop
        - name: "Add image signatures to ODS"
          link: "/signature/java/add/image/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Add image signatures to OTS"
          link: "/signature/java/add/image/ots/"
          description: "OpenDocument Spreadsheet Template"

        # format loop
        - name: "Add image signatures to PPT"
          link: "/signature/java/add/image/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Add image signatures to PPTX"
          link: "/signature/java/add/image/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Add image signatures to PPS"
          link: "/signature/java/add/image/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Add image signatures to PPSX"
          link: "/signature/java/add/image/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Add image signatures to POTM"
          link: "/signature/java/add/image/potm/"
          description: "Microsoft PowerPoint Macro-Enabled Template"

        # format loop
        - name: "Add image signatures to POTX"
          link: "/signature/java/add/image/potx/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Add image signatures to PPTM"
          link: "/signature/java/add/image/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Add image signatures to ODP"
          link: "/signature/java/add/image/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Add image signatures to OTP"
          link: "/signature/java/add/image/otp/"
          description: "OpenDocument Presentation Template"

        # format loop
        - name: "Add image signatures to WEBP"
          link: "/signature/java/add/image/webp/"
          description: "WebP Image"

        # format loop
        - name: "Add image signatures to TIFF"
          link: "/signature/java/add/image/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Add image signatures to JPEG"
          link: "/signature/java/add/image/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Add image signatures to GIF"
          link: "/signature/java/add/image/gif/"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Add image signatures to PNG"
          link: "/signature/java/add/image/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Add image signatures to BMP"
          link: "/signature/java/add/image/bmp/"
          description: "Bitmap File Format"

        # format loop
        - name: "Add image signatures to CDR"
          link: "/signature/java/add/image/cdr/"
          description: "CorelDraw Vector Graphic Drawing"

        # format loop
        - name: "Add image signatures to SVG"
          link: "/signature/java/add/image/svg/"
          description: "Scalable Vector Graphics"

        # format loop
        - name: "Add image signatures to PSD"
          link: "/signature/java/add/image/psd/"
          description: "Adobe Photoshop Document"

        # format loop
        - name: "Add image signatures to WMF"
          link: "/signature/java/add/image/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Add image signatures to EMF"
          link: "/signature/java/add/image/emf/"
          description: "Enhanced Metafile Format"

        # format loop
        - name: "Add image signatures to CMX"
          link: "/signature/java/add/image/cmx/"
          description: "Corel Metafile eXchange Image"

        # format loop
        - name: "Add image signatures to DJVU"
          link: "/signature/java/add/image/djvu/"
          description: "Deja Vu"

        # format loop
        - name: "Add image signatures to PPSM"
          link: "/signature/java/add/image/ppsm/"
          description: "Microsoft PowerPoint Macro-Enabled Slide Show"

        # format loop
        - name: "Add image signatures to DCM"
          link: "/signature/java/add/image/dcm/"
          description: "Digital Imaging and Communications in Medicine"


############################# Back to top ###############################
back_to_top:
    enable: true
---
