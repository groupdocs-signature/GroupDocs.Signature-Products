---
############################# Static ############################
layout: "landing"
date: 2023-09-13T10:36:51
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
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, Java, Cloud APIs & Online Document Signature Apps"
head_description: "Get all-in-one document e-signature solution for .NET, Java and cloud-based applications. Sign common document formats online using simple drag and drop feature"

############################# Header ############################
title: "Sign documents<br>via .NET API"
description: "Sign digital documents and images on any platform using our flexible APIs and app based solutions for programmers and end-users."
words:
  for: "for"

actions:
  main: "Free NuGet Download"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Licensing"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Ready to get started?"
  description: "Try GroupDocs.Signature features for free or request a license"

release:
  title: "Version {0} released"
  notes: "See what’s new"
  downloads: "Downloads"

code:
  title: "Sign PDF files in C#"
  more: "More examples"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Select PDF document
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Provide text
        var options = new TextSignOptions("John Smith")
        {
            // Set color
            ForeColor = Color.Red
        };
        // Sign document and save to file
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Overview"
  description: "API for performing document signing and related operations in .NET applications"
  features:
    # feature loop
    - title: "Adding signatures to business documents in C#"
      content: "Documents signing: With GroupDocs.Signature for .NET, you can add various types of signatures, such as text, images, barcodes, and digital certificates, to PDF and Office documents. This API allows you to sign your documents with nearly any data type, including hidden metadata."

    # feature loop
    - title: "Processing signed documents"
      content: "Additional processing: You can perform powerful operations on signed documents using GroupDocs.Signature. This includes searching for existing signatures within business documents and verifying them using specific criteria. Additionally, you can retrieve document information and preview pages through this .NET API."

    # feature loop
    - title: "Customizing results"
      content: "GroupDocs.Signature for .NET offers extensive customization options. You can precisely position signatures anywhere on a document page and adjust their appearance using a variety of settings. Furthermore, this API supports saving processed documents in a wide range of supported formats."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform independence"
  description: "GroupDocs.Signature for .NET supports the following operating systems, frameworks and package managers"
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Supported file formats"
  description: |
    GroupDocs.Signature for .NET supports operations with the following [file formats](https://docs.groupdocs.com/signature/net/supported-document-formats/).
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
  description: "Signing PDFs, Office Documents, and Images swiftly and accurately"

  items:
    # feature loop
    - icon: "merge"
      title: "Document signing"
      content: "Add one or multiple supported types of signatures accurately at any specified position on business documents."

    # feature loop
    - icon: "split"
      title: "Customize signatures"
      content: "Utilize features such as color, font, border, rotation, etc., to configure the appearance of signatures."

    # feature loop
    - icon: "move"
      title: "Document password protection"
      content: "Secure certain document types by setting a password after signing."

    # feature loop
    - icon: "remove"
      title: "Protection from changes"
      content: "Prevent changes to important business documents after appending a signature with a digital certificate."

    # feature loop
    - icon: "rotate"
      title: "Convert signed files to other formats"
      content: "Convert signed files to desired formats, such as saving a Word document as a PDF."

    # feature loop
    - icon: "swap"
      title: "Extract page previews"
      content: "Extract pages from signed documents as individual images for future processing."

    # feature loop
    - icon: "extract"
      title: "Signature search in documents"
      content: "Retrieve information about previously added signatures in specific documents."

    # feature loop
    - icon: "orientation"
      title: "Validate signed documents"
      content: "Verify the proper signing of documents using validation features."

    # feature loop
    - icon: "preview"
      title: "Update or delete signatures"
      content: "Easily reposition specific signatures on a page, modify their text, or delete them without any issues."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Code samples"
  description: "Some use cases of typical GroupDocs.Signature for .NET operations"
  items:
    # code sample loop
    - title: "Add QR-code to PDF"
      content: |
        Adding [QR-codes](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) to specific pages of PDF documents can enhance business processes. Below is an example of how to add a QR code using GroupDocs.Signature.
        {{< landing/code title="How to put QR code to PDF.">}}
        ```csharp {style=abap}
        // Load the document to sign
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Create QR code options with predefined text
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Configure QR code encoding type and position on the page
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Sign the document and save it as the result file
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Protecting a DOCX document using a digital certificate"
      content: |
        You can [Protect a Document](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) using personal or corporate signatures stored as digital certificates. Such protected documents cannot be modified without invalidating the signature.
        {{< landing/code title="Here is how to ensure document integrity.">}}
        ```csharp {style=abap}   
        // Load the document to be digitally signed
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Specify digital signing options and provide the path to the certificate file
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Set the certificate password
                Password = "1234567890"
            };
            // Sign the document and save it to the desired path
            signature.Sign("digitally_signed.pdf", options);
        }
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
