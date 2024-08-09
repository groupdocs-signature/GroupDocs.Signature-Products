---
############################# Static ############################
layout: "family"
date:  2024-07-25T14:25:12
draft: false

product: "Signature"
product_tag: "signature"

lang: en

############################# Head ############################
head_title: "C# .NET, Java, Node.js Digital Signature Apps"
head_description: "Integrate e-signatures in .NET, Java, or Node.js applications with GroupDocs.Signature. Sign popular business document formats."

############################# Header ############################
title: "Document e-Signing Solution"
description:  |
  Sign digital documents and images on any platform using our flexible APIs and app-based solutions for programmers and end-users.

  Search and modify previously added signatures using advanced methods.

  Protect documents from changes with digital certificates and control hidden metadata.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Choose your platform"
  title: "Platform independence"
  description: "GroupDocs.Signature library supports the following operating systems and frameworks:"
  details_link_title: "Learn more"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Signature .NET 
      color: "blue"
      tag: "net"
      link: "/signature/net/"
      features_link: "https://docs.groupdocs.com/signature/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.6.2 or higher <br> .NET Core 3.0 or higher <br> .NET 6.0 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS <br> Microsoft Azure
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Signature Java
      color: "red"
      tag: "java"
      link: "/signature/java/"
      features_link: "https://docs.groupdocs.com/signature/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 8 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Signature Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/signature/nodejs-java/"
      features_link: "https://docs.groupdocs.com/signature/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Any other text editor
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Signature key features"
  description: "Our solution is designed to add various types of signatures to popular document and file formats. Enrich your business processes easily."

  items:
    # items loop
    - icon: "additional"
      title: "Enrich your data with signatures"
      content: "Append text, images, watermarks, etc. to your business documents."

    # items loop
    - icon: "protect"
      title: "Protect documents content"
      content: "Forbid document changes by sealing it with a digital certificate."

    # items loop
    - icon: "search"
      title: "Add hidden data and barcodes"
      content: "Use metadata to store invisible information or put custom barcodes on pages."

    # items loop
    - icon: "manipulate"
      title: "Manipulate signatures"
      content: "Search, update, or delete all signatures that have been added previously."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Protect your files using signatures"
  description: "GroupDocs.Signature code examples"
  items:
    # code sample loop
    - title: "Generate and add QR-code"
      content: |
       GroupDocs.Signature allows us to generate and add QR-codes to documents with supported formats. Provide the path to a document which must be signed and set up desired text and visual options of QR-code. You may put the generated QR-code image on any area of any document page.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Specify the document for signing
            using (Signature signature = new Signature("source.docx"))
            {
                // Create QR-code sign options
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // Set QR-code options
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150,
                };

                // Sign and save processed file
                SignResult result = signature.Sign("result.docx", options);
            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Specify the document for signing
            Signature signature = new Signature("source.docx");

            // Create QR-code sign options
            QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith");

            // Set QR-code options
            options.setEncodeType(QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // Sign and save processed file
            signature.sign("result.docx", options);
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            const signatureLib = require('@groupdocs/groupdocs.signature')

            // Specify the document for signing
            const signature = new signatureLib.Signature('source.docx');

            // Create QR-code sign options
            const options = new signatureLib.QrCodeSignOptions('JohnSmith');

            // Set QR-code options
            options.setEncodeType(signatureLib.QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // Sign and save processed file
            signature.sign('result.docx', options);
            ```

############################# Supported Formats ###############################
formats:
  enable: true
  title: "60+ file formats are supported"
  description: "GroupDocs.Signature supports almost all popular file formats"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Our library statistical data"
  description: "Inspect key product metrics, revealing insights into our achievements, impact, and growth"

  items:
    # items loop
    - number: "50+"
      title: "Supported formats"
      content: "Signing more than 60 of the most popular business file formats."

    # items loop
    - number: "500k"
      title: "NuGet downloads"
      content: "GroupDocs.Signature for .NET is a popular library with over 550,000 downloads on NuGet."

    # items loop
    - number: "15k"
      title: "Maven downloads"
      content: "Java developers have downloaded GroupDocs.Signature on Maven more than 15K times."

    # items loop
    - number: "140+"
      title: "Happy customers"
      content: "Individual developers and top companies worldwide use our products to build innovative solutions."


############################# Customers ###############################
customers:
  enable: true
  title: "Our happy customers"
  description: "GroupDocs libraries are employed by globally renowned and distinguished brands across the world"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Ready to get started?"
  description: "Try GroupDocs.Signature features for free on your platform"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/signature/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/signature/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/signature/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "Frequently asked questions"
  description: "Explore our Frequently Asked Questions"

  items:
    # items loop
    - question: "Does GroupDocs.Signature need any external library for documents signing?"
      answer: "No, GroupDocs.Signature works independently. There are no third-party dependencies like Adobe Acrobat, Microsoft Office, etc."

    # items loop
    - question: "Is it possible to test GroupDocs.Signature features before buying?"
      answer: "Absolutely! GroupDocs.Signature offers a free trial. Install it and explore its features. Note that trial versions add 'trial badges' to your documents and only process the first 3 pages. For the full experience, obtain a free 30-day temporary license to access all functionalities. See details under [temporary license](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "What license types are provided?"
      answer: "Looking for a GroupDocs.Signature license? We offer various options tailored to your needs. Choose based on team size, deployment locations (single office or remote workplaces), and whether end-customer distribution requires sharing the SDK/API with clients. Alternatively, opt for a monthly usage license with metered plans—pay only for what you use. Discover the best fit for you under [pricing](https://purchase.groupdocs.com/pricing/signature/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Signature low code APIs"
  description: "Sign files using your application via our cloud-based REST API."
  
  items:
    # items loop
    - title: "GroupDocs.Signature Cloud for cURL"
      content: "Use cURL RESTful API to put signatures on PDF, Word, Excel, PowerPoint, JPEG, and many other file formats."
      icon: "groupdocs_signature-for-curl"
      link: "https://products.groupdocs.cloud/signature/curl"

    # items loop
    - title: "GroupDocs.Signature Cloud for .NET"
      content: "Enrich your .NET applications with signing documents via Cloud SDK. Protect business documents in your own way."
      icon: "groupdocs_signature-for-net"
      link: "https://products.groupdocs.cloud/signature/net"

    # items loop
    - title: "GroupDocs.Signature Cloud for Java"
      content: "GroupDocs.Signature SDK grants access to various possibilities for your Java applications to sign any files."
      icon: "groupdocs_signature-for-java"
      link: "https://products.groupdocs.cloud/signature/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Signature Web apps"
  description: "GroupDocs.Signature presents a free web application where you can sign documents. More than 60 popular file formats could be signed via your favorite browser FOR FREE."

  items:
    # items loop
    - title: "GroupDocs.Signature Total"
      content: "Online tool to put signatures on documents from any device."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/signature/total"

    # items loop
    - title: "GroupDocs.Signature DOCX"
      content: "Sign MS Word DOCX online."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/signature/docx"

    # items loop
    - title: "GroupDocs.Signature PDF"
      content: "Protect PDF documents online."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/signature/pdf"


      


---