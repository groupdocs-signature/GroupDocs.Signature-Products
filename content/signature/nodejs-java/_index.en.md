---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:02
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: en
#productCode: nodejs-java
#otherformats: 
#breadcrumb: Put  signature on  for JavaScript
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: ".NET, Java, Cloud APIs & Online Document Signature Apps"
head_description: "Get all-in-one document e-signature solution for .NET, Java and cloud-based applications. Sign common document formats online using simple drag and drop feature"

############################# Header ############################
title: "Sign documents<br>with Node.js API"
description: "Sign digital documents and images on any platform using our flexible APIs and app based solutions for programmers and end-users."
words:
  for: "for"

actions:
  main: "Download from NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Licensing"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Ready to get started?"
  description: "Try GroupDocs.Signature features for free or request a license"

release:
  title: "Version {0} released"
  notes: "See what’s new"
  downloads: "Downloads"

code:
  title: "Signing PDFs by Node.js"
  more: "More examples"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Select PDF document
    let signature = new Signature("sample.pdf");
    
    // Provide text
    let options = new TextSignOptions("John Smith");
    
    // Set color
    options.ForeColor = Color.Red;
    
    // Sign document and save to file
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Overview"
  description: "Documents signing library that ready to be used in Node.js applications"
  features:
    # feature loop
    - title: "Digital Signatures Solution for Business Documents with Node.js"
      content: "GroupDocs.Signature for Node.js via Java offers a comprehensive set of digital signature options for PDF, Office documents and images. Text, barcodes, images, digital certificates and metadata are available. Streamlined document processing ensures efficiency."

    # feature loop
    - title: "Advanced Manipulation of Signed Documents"
      content: "GroupDocs.Signature empowers you to process signed documents. Search and validate signatures using various criteria. Additionally, extract detailed document information or generate preview images of pages."

    # feature loop
    - title: "Diverse Output Formats"
      content: "Our solution provides extensive control over the output format of signed documents. Precisely position signatures on any page and customize their appearance. Save signed documents in numerous supported formats and optionally secure them with passwords."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform independence"
  description: "GroupDocs.Signature for Node.js via Java performs document processing with various operating systems"
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
    GroupDocs.Signature for Node.js via Java facilitates operations for the [popular file formats](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  title: "Features of GroupDocs.Signature"
  description: "Sign PDFs, Office documents, and images with digital signatures"

  items:
    # feature loop
    - icon: "sign"
      title: "Business Signatures"
      content: "Employ various signature types to sign documents. Place digital signatures precisely on any page location."

    # feature loop
    - icon: "custom"
      title: "Customizing Signature Appearance"
      content: "Tailor the visual aspects of signatures by adjusting color, font, borders, rotation, and more to achieve your desired outcome."

    # feature loop
    - icon: "password"
      title: "Password-Protected Documents"
      content: "For many supported document formats, safeguard signed documents with a password for added security."

    # feature loop
    - icon: "protect"
      title: "Preventing Unauthorized Modifications"
      content: "Protect crucial business documents signed with digital certificates from unauthorized alterations."

    # feature loop
    - icon: "convert"
      title: "Desired Output Formats"
      content: "Effortlessly get signed documents in any supported format. Convert MS Word documents to PDF format with ease."

    # feature loop
    - icon: "preview"
      title: "Documents Previewing"
      content: "Save individual document pages as images for future needs."

    # feature loop
    - icon: "search"
      title: "Signature Search"
      content: "Retrieve information about previously added signatures within your documents."

    # feature loop
    - icon: "validate"
      title: "Document Validation"
      content: "Verify the authenticity of signatures presented in any document."

    # feature loop
    - icon: "update"
      title: "Signature Management"
      content: "Delete, relocate, or modify any signatures placed on any document page."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Code samples"
  description: "Illustrative examples showcasing typical GroupDocs.Signature for Node.js via Java operations"
  items:
    # code sample loop
    - title: "Mark PDF with QR Codes"
      content: |
        Incorporating [barcodes](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) into specific PDF document pages can streamline business processes. This section provides an example of adding a QR code using GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="How to put QR code to PDF.">}}
        ```javascript {style=abap}
        // Load the document to sign
        let signature = new Signature("file_to_sign.pdf");
        
        // Create QR code options with predefined text
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Configure QR code encoding type and position on the page
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Sign the document and save it as the result file
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Protecting a DOCX with a Digital Signature"
      content: |
        [Protect your Documents](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) by signatures based on digital certificates. Digital signature protect your business documents against content changing.
        {{< landing/code title="Here is how to ensure document integrity.">}}
        ```javascript {style=abap}   
        // Load the document to be digitally signed
        let signature = new Signature("file_to_sign.docx");
        
        // Specify digital signing options and provide the path to the certificate file
        let options = new DigitalSignOptions("certificate.pfx");

        // Set the certificate password
        options.Password = "1234567890";

        // Sign the document and save it to the desired path
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
