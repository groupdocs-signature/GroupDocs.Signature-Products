


---
############################# Static ############################
layout: "format"
date:  2024-07-30T15:09:06
draft: false
lang: en
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Add Metadata to DOCX Files in C# Applications"
head_description: "C# metadata processing API to add metadata information to DOCX files. Work with metadata standards XMP, EXIF, IPTC, ID3 etc"

############################# Header ############################
title: "Adding Metadata To DOCX In C#" 
description: "Add custom metadata properties to a wide range of business documents, images, audio & video file formats using GroupDocs.Signature for .NET API"
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download Free Trial"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "About GroupDocs.Signature for .NET API"
    link: "/metadata/net/"
    link_title: "Learn more"
    picture: "about_metadata.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) offers an advanced set of metadata management and manipulation features, allowing .NET programmers to easily view, edit, delete, find, compare, swap and export metadata information from images and document formats without using any external software. Add metadata details to PDF, Microsoft Word, Excel, PowerPoint, Outlook, OneNote, Visio, Project, AutoCAD, Archive and Multimedia file formats with additional support to perform metadata operations on any GroupDocs.Signature-based applications with true flexibility

############################# Steps ############################
steps:
    enable: true
    title: "Steps for adding Metadata to Docx in C#"
    content: |
      [GroupDocs.Signature](/signature/net/) makes it easy for .NET developers to add metadata details to DOCX files from within their applications by implementing a few easy steps.
      
      1. Load the DOCX file to be updated.
      2. Specify a predicate that will be used to add metadata properties.
      3. Pass the predicate to the  method.
      4. Save the changes.
   
    code:
      platform: "net"
      copy_title: "Copy"
      install:
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-metadata</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```java {style=abap}
        // load the file in an instance of  class
        try (Metadata metadata = new Metadata("input.docx"))
        {
            // add a property containing the content author
            int affected = metadata.addProperties(new ContainsTagSpecification(Tags.getTime().getPrinted()), 
                new PropertyValue(new Date()));

            // process operation results
            System.out.println(String.format("Affected properties: %s", affected));

            // save the file with updated metadata
            metadata.save("output.docx");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Document Metadata Management"
  description: "Our robust API simplifies the management of document metadata. Seamlessly access, edit, and manipulate a variety of document properties to enhance organization and searchability."
  image: "/img/metadata/features_add.webp" # 500x500 px
  image_description: "Metadata Manipulation Features"
  features:
    # feature loop
    - title: "Metadata Control"
      content: "Easily retrieve and process metadata from documents. Gain valuable insights into properties such as author, creation date, and more."

    # feature loop
    - title: "Metadata Editing"
      content: "Directly modify document metadata. Update properties to improve organization, boost searchability, and ensure accurate information."

    # feature loop
    - title: "Advanced Metadata Management"
      content: "Execute complex operations on document metadata. Efficiently add custom properties, remove unnecessary data, and maintain data consistency."
      
  code_samples:
    # code sample loop
    - title: "How to Add Custom Metadata to a TIFF Image"
      content: |
        This example demonstrates how to insert a custom tag into an EXIF package.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        try (Metadata metadata = new Metadata("input.tiff")) {
            IExif root = (IExif) metadata.getRootPackage();

            //  Assign the EXIF package if it is missing.
            if (root.getExifPackage() == null) {
                root.setExifPackage(new ExifPackage());
            }

            //  Insert a recognized property.
            root.getExifPackage().set(new TiffAsciiTag(TiffTagID.Artist, "Artist's name"));

            //  Include a fully custom property that is not part of the EXIF specification.
            //  Be aware that the chosen ID may conflict with IDs used by some third-party tools.
            root.getExifPackage().set(new TiffAsciiTag(TiffTagID.getByRawValue(65523), "Hidden data"));

            metadata.save("output.tiff");
        }
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Ready to get started?"
  description: "Try GroupDocs.Signature features for free or request a license"
  items:
    #  loop
    - title: "Nuget download"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Adding Metadata Properties To Other File Formats"
    exclude: "DOCX"
    description: "Multi format documents and images metadata addition API for GroupDocs.Signature. Retrieve metadata of some of the popular file formats as stated below."
    items: 
        # format loop 1
        - name: "{common-content.format-formats.avi.name}"
          format: "AVI"
          link: "/metadata/net//avi/"
          description: "{common-content.format-formats.avi.description}"
          
        # format loop 2
        - name: "{common-content.format-formats.djvu.name}"
          format: "DJVU"
          link: "/metadata/net//djvu/"
          description: "{common-content.format-formats.djvu.description}"
          
        # format loop 3
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/metadata/net//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 4
        - name: "{common-content.format-formats.epub.name}"
          format: "EPUB"
          link: "/metadata/net//epub/"
          description: "{common-content.format-formats.epub.description}"
          
        # format loop 5
        - name: "{common-content.format-formats.heic.name}"
          format: "HEIC"
          link: "/metadata/net//heic/"
          description: "{common-content.format-formats.heic.description}"
          
        # format loop 6
        - name: "Watermark JPEG"
          format: "JPEG"
          link: "/metadata/net//jpeg/"
          description: "JPEG Image"
          
        # format loop 7
        - name: "{common-content.format-formats.mov.name}"
          format: "MOV"
          link: "/metadata/net//mov/"
          description: "{common-content.format-formats.mov.description}"
          
        # format loop 8
        - name: "{common-content.format-formats.mp3.name}"
          format: "MP3"
          link: "/metadata/net//mp3/"
          description: "{common-content.format-formats.mp3.description}"
          
        # format loop 9
        - name: "{common-content.format-formats.msg.name}"
          format: "MSG"
          link: "/metadata/net//msg/"
          description: "{common-content.format-formats.msg.description}"
          
        # format loop 10
        - name: "{common-content.format-formats.ods.name}"
          format: "ODS"
          link: "/metadata/net//ods/"
          description: "{common-content.format-formats.ods.description}"
          
        # format loop 11
        - name: "{common-content.format-formats.odt.name}"
          format: "ODT"
          link: "/metadata/net//odt/"
          description: "{common-content.format-formats.odt.description}"
          
        # format loop 12
        - name: "Watermark PDF"
          format: "PDF"
          link: "/metadata/net//pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 13
        - name: "Watermark PNG"
          format: "PNG"
          link: "/metadata/net//png/"
          description: "Portable Network Graphic"
          
        # format loop 14
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/metadata/net//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 15
        - name: "Watermark TIFF"
          format: "TIFF"
          link: "/metadata/net//tiff/"
          description: "Tag Image File Format"
          
        # format loop 16
        - name: "{common-content.format-formats.torrent.name}"
          format: "TORRENT"
          link: "/metadata/net//torrent/"
          description: "{common-content.format-formats.torrent.description}"
          
        # format loop 17
        - name: "{common-content.format-formats.vsdx.name}"
          format: "VSDX"
          link: "/metadata/net//vsdx/"
          description: "{common-content.format-formats.vsdx.description}"
          
        # format loop 18
        - name: "{common-content.format-formats.wav.name}"
          format: "WAV"
          link: "/metadata/net//wav/"
          description: "{common-content.format-formats.wav.description}"
          
        # format loop 19
        - name: "Watermark WEBP"
          format: "WEBP"
          link: "/metadata/net//webp/"
          description: "WEB Picture"
          
        # format loop 20
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/metadata/net//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
          
        # format loop 21
        - name: "{common-content.format-formats.zip.name}"
          format: "ZIP"
          link: "/metadata/net//zip/"
          description: "{common-content.format-formats.zip.description}"
          

---