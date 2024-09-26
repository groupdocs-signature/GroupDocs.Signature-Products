<% configRef "..\\..\\configs\\index\\index.yml" %>
<% include "..\\..\\data\\family_data.md" %>
---
############################# Static ############################
layout: "family"
date:  <% date "utcnow" %>
draft: false

product: "Signature"
product_tag: "signature"

lang: <% lower ( get "lang") %>

############################# Head ############################
head_title: "<% "{index-content.head_title}" %>"
head_description: "<% "{index-content.head_description}" %>"

############################# Header ############################
title: "<% "{index-content.title}" %>"
description:  |
  <% "{index-content.description_1}" %>

  <% "{index-content.description_2}" %>

  <% "{index-content.description_3}" %>

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "<% "{index-content.platforms.head_title}" %>"
  title: "<% "{index-content.platforms.title}" %>"
  description: "<% "{index-content.platforms.description}" %>"
  details_link_title: "<% "{index-content.platforms.learn_more}" %>"

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
      features_link: "https://docs.groupdocs.com/signature/nodejs-java/system-requirements/"
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
                    Atom <br> Visual Studio Code <br> <% "{index-content.platforms.any_other_text_editor}" %>
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

    # items loop
    - title: "Python"
      description: GroupDocs.Signature Python
      color: "yellow"
      tag: "python-net"
      link: "/signature/python-net/"
      features_link: "https://docs.groupdocs.com/signature/python-net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Python 3.9+ and .Net 6+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IDLE <br> PyCharm <br> Visual Studio Code
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

############################# Features ###############################
features:
  enable: true
  title: "<% "{index-content.features.title}" %>"
  description: "<% "{index-content.features.description}" %>"

  items:
    # items loop
    - icon: "additional"
      title: "<% "{index-content.features.feature_1.title}" %>"
      content: "<% "{index-content.features.feature_1.content}" %>"

    # items loop
    - icon: "protect"
      title: "<% "{index-content.features.feature_2.title}" %>"
      content: "<% "{index-content.features.feature_2.content}" %>"

    # items loop
    - icon: "search"
      title: "<% "{index-content.features.feature_3.title}" %>"
      content: "<% "{index-content.features.feature_3.content}" %>"

    # items loop
    - icon: "manipulate"
      title: "<% "{index-content.features.feature_4.title}" %>"
      content: "<% "{index-content.features.feature_4.content}" %>"

############################# Code samples ############################
code_samples:
  enable: true
  title: "<% "{index-content.code_samples.index_title}" %>"
  description: "<% "{index-content.code_samples.index_description}" %>"
  items:
    # code sample loop
    - title: "<% "{index-content.code_samples.sample_index.title}" %>"
      content: |
       <% "{index-content.code_samples.sample_index.content}" %>
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // <% "{index-content.code_samples.sample_index.comment_1}" %>
            using (Signature signature = new Signature("source.docx"))
            {
                // <% "{index-content.code_samples.sample_index.comment_2}" %>
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // <% "{index-content.code_samples.sample_index.comment_3}" %>
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150,
                };

                // <% "{index-content.code_samples.sample_index.comment_4}" %>
                SignResult result = signature.Sign("result.docx", options);
            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // <% "{index-content.code_samples.sample_index.comment_1}" %>
            Signature signature = new Signature("source.docx");

            // <% "{index-content.code_samples.sample_index.comment_2}" %>
            QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith");

            // <% "{index-content.code_samples.sample_index.comment_3}" %>
            options.setEncodeType(QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // <% "{index-content.code_samples.sample_index.comment_4}" %>
            signature.sign("result.docx", options);
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            const signatureLib = require('@groupdocs/groupdocs.signature')

            // <% "{index-content.code_samples.sample_index.comment_1}" %>
            const signature = new signatureLib.Signature('source.docx');

            // <% "{index-content.code_samples.sample_index.comment_2}" %>
            const options = new signatureLib.QrCodeSignOptions('JohnSmith');

            // <% "{index-content.code_samples.sample_index.comment_3}" %>
            options.setEncodeType(signatureLib.QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // <% "{index-content.code_samples.sample_index.comment_4}" %>
            signature.sign('result.docx', options);
            ```
        - language: "Python"
          color: "yellow"
          content: |
            ```python {style=abap}  
            import groupdocs.signature as sg

            def run():

                # <% "{index-content.code_samples.sample_index.comment_1}" %>
                with sg.Signature('source.docx') as signature:

                    # <% "{index-content.code_samples.sample_index.comment_2}" %>
                    options = sg.QrCodeSignOptions('JohnSmith')

                    # <% "{index-content.code_samples.sample_index.comment_3}" %>
                    options.setEncodeType(sg.QrCodeTypes.QR)
                    options.setLeft(50)
                    options.setTop(100)

                    # <% "{index-content.code_samples.sample_index.comment_4}" %>
                    signature.sign('result.docx', options)
            ```

############################# Supported Formats ###############################
formats:
  enable: true
  title: "<% "{index-content.formats.title}" %>"
  description: "<% "{index-content.formats.description}" %>"

############################# Metrics ###############################
metrics:
  enable: true
  title: "<% "{index-content.metrics.title}" %>"
  description: "<% "{index-content.metrics.description}" %>"

  items:
    # items loop
    - number: "50+"
      title: "<% "{index-content.metrics.item_1.title}" %>"
      content: "<% "{index-content.metrics.item_1.description}" %>"

    # items loop
    - number: "500k"
      title: "<% "{index-content.metrics.item_2.title}" %>"
      content: "<% "{index-content.metrics.item_2.description}" %>"

    # items loop
    - number: "15k"
      title: "<% "{index-content.metrics.item_3.title}" %>"
      content: "<% "{index-content.metrics.item_3.description}" %>"

    # items loop
    - number: "140+"
      title: "<% "{index-content.metrics.item_4.title}" %>"
      content: "<% "{index-content.metrics.item_4.description}" %>"


############################# Customers ###############################
customers:
  enable: true
  title: "<% "{index-content.customers.title}" %>"
  description: "<% "{index-content.customers.description}" %>"

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
  title: "<% "{index-content.actions.title}" %>"
  description: "<% "{index-content.actions.description_index}" %>"

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
  title: "<% "{index-content.faq.title}" %>"
  description: "<% "{index-content.faq.description}" %>"

  items:
    # items loop
    - question: "<% "{index-content.faq.item_1.question}" %>"
      answer: "<% "{index-content.faq.item_1.answer}" %>"

    # items loop
    - question: "<% "{index-content.faq.item_2.question}" %>"
      answer: "<% "{index-content.faq.item_2.answer}" %>"

    # items loop
    - question: "<% "{index-content.faq.item_3.question}" %>"
      answer: "<% "{index-content.faq.item_3.answer}" %>"

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "<% "{index-content.cloud_links.title}" %>"
  description: "<% "{index-content.cloud_links.description}" %>"
  
  items:
    # items loop
    - title: "GroupDocs.Signature Cloud for cURL"
      content: "<% "{index-content.cloud_links.item_1.content}" %>"
      icon: "groupdocs_signature-for-curl"
      link: "https://products.groupdocs.cloud/signature/curl"

    # items loop
    - title: "GroupDocs.Signature Cloud for .NET"
      content: "<% "{index-content.cloud_links.item_2.content}" %>"
      icon: "groupdocs_signature-for-net"
      link: "https://products.groupdocs.cloud/signature/net"

    # items loop
    - title: "GroupDocs.Signature Cloud for Java"
      content: "<% "{index-content.cloud_links.item_3.content}" %>"
      icon: "groupdocs_signature-for-java"
      link: "https://products.groupdocs.cloud/signature/java"

############################# App links ###############################
app_links:
  enable: true
  title: "<% "{index-content.app_links.title}" %>"
  description: "<% "{index-content.app_links.description}" %>"

  items:
    # items loop
    - title: "GroupDocs.Signature Total"
      content: "<% "{index-content.app_links.item_1.content}" %>"
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/signature/total"

    # items loop
    - title: "GroupDocs.Signature DOCX"
      content: "<% "{index-content.app_links.item_2.content}" %>"
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/signature/docx"

    # items loop
    - title: "GroupDocs.Signature PDF"
      content: "<% "{index-content.app_links.item_3.content}" %>"
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/signature/pdf"


      


---