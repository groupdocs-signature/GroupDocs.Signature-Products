---
############################# Static ############################
layout: "landing"
date: 2023-09-13T10:36:50
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: en
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: ".NET, Java, Cloud APIs & Online Document Signature Apps"
head_description: "Get all-in-one document e-signature solution for .NET, Java and cloud-based applications. Sign common document formats online using simple drag and drop feature"

############################# Header ############################
title: "Sign documents<br>via Java API"
description: "Sign digital documents and images on any platform using our flexible APIs and app based solutions for programmers and end-users."
words:
  for: "for"

actions:
  main: "Free Maven Download"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Licensing"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Ready to get started?"
  description: "Try GroupDocs.Signature features for free or request a license"

release:
  title: "Version {0} released"
  notes: "See what’s new"
  downloads: "Downloads"

code:
  title: "Sign PDF files in Java"
  more: "More examples"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Select PDF document
    Signature signature = new Signature("sample.pdf");
    
    // Provide text
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Sign document and save to file
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Overview"
  description: "API for performing document signing and related operations in Java applications"
  features:
    # feature loop
    - title: "Improved business documents with digital signatures in Java"
      content: "Swift and customizable signing: GroupDocs.Signature for Java offers a wide range of digital signature options for PDFs, images, and Office documents. You can use text, barcodes, QR-codes, digital certificates, pictures, or hidden metadata. The document processing is fast and efficient."

    # feature loop
    - title: "Manipulating signed documents"
      content: "Advanced document processing involves powerful operations on signed documents using GroupDocs.Signature for Java. You can search for and validate signatures that have been added to business documents using various useful criteria. Additionally, you can access detailed information about the document or obtain preview images of its pages."

    # feature loop
    - title: "Variety of output choices"
      content: "Robust signing options allow you to customize the output for documents signed with GroupDocs.Signature for Java. You can precisely position any signature on any document page and configure its appearance in various ways. The Java API supports saving signed business documents in numerous supported formats and provides options for securing them with passwords."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform independence"
  description: "GroupDocs.Signature for Java supports the following operating systems, frameworks and package managers"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Supported file formats"
  description: |
    GroupDocs.Signature for Java supports operations with the following [file formats](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office formats
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Images & Other Formats
        * **Portable:** PDF
        * **Images:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Other office formats:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Other formats
        * **Web:** HTML, MHTML
        * **Archives:** ZIP, TAR, 7Z
        * **Certificates:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Signature features"
  description: "Signing PDFs, Office Documents, and images with digital signatures"

  items:
    # feature loop
    - icon: "merge"
      title: "Adding Signatures"
      content: "Sign a document using various supported signature types by placing a digital signature precisely at any position on any page."

    # feature loop
    - icon: "split"
      title: "Customizing results"
      content: "Customize the signature appearance by adjusting color, font, border, rotation, and other features to achieve the desired result."

    # feature loop
    - icon: "move"
      title: "Securing documents with password"
      content: "For many supported document types, you can protect the signed document with a password."

    # feature loop
    - icon: "remove"
      title: "Preventing unauthorized changes"
      content: "Protect important business documents signed with a digital certificate from unauthorized modifications."

    # feature loop
    - icon: "rotate"
      title: "Obtaining results in desired formats"
      content: "Easily obtain signed result files in any supported format. You can also convert MS Word documents to PDF effortlessly."

    # feature loop
    - icon: "swap"
      title: "Document preview"
      content: "Save any page of a document as an image for future processing."

    # feature loop
    - icon: "extract"
      title: "Searching for signatures"
      content: "It is possible to get information about previously added signatures in specific documents."

    # feature loop
    - icon: "orientation"
      title: "Validating documents"
      content: "Validate the correctness of signatures on any signed document."

    # feature loop
    - icon: "preview"
      title: "Managing signatures"
      content: "Once a signature is placed on a document page, it can be deleted, moved, or updated as needed."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Code samples"
  description: "Some use cases of typical GroupDocs.Signature for Java operations"
  items:
    # code sample loop
    - title: "Enchance PDF document with QR-code"
      content: |
        Enhancing business processes by adding [QR-codes](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) to specific pages of PDF documents can be valuable. There is an example of how to add a QR code using GroupDocs.Signature for Java.
        {{< landing/code title="Enchance PDF document with QR-code">}}
        ```java {style=abap}
        // Load the document to sign
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Create QR code options with predefined text
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Configure QR code encoding type and position on the page
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Sign the document and save it as the result file
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Use digital signature to protect a DOCX"
      content: |
        You can [Safeguard a Document](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) using personal or corporate signatures stored as digital certificates. Documents secured with certificate cannot be altered without invalidating the signature.
        {{< landing/code title="Use digital signature to protect a DOCX">}}
        ```java {style=abap}   
        // Load the document to be digitally signed
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Specify digital signing options and provide the path to the certificate file
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Set the certificate password
        options.setPassword("1234567890");

        // Sign the document and save it to the desired path
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

############################# Reviews ############################
# reviews:
# enable: true
# title: "{reviews.title}"
# description: "{reviews.description}"

# items:
#   # review loop
#   - title: "GroupDocs.Viewer"
#     content: "{reviews.review_1.content}"
#     author: "{reviews.review_1.author}"
#     company: "{reviews.review_1.company}"

#   # review loop
#   - title: "GroupDocs.Viewer"
#     content: "{reviews.review_2.content}"
#     author: "{reviews.review_2.author}"
#     company: "{reviews.review_2.company}"
---
