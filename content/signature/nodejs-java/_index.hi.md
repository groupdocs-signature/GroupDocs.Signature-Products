---
############################# Static ############################
layout: "landing"
date: 2024-03-04T17:52:03
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: hi
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
head_title: ".NET, जावा, क्लाउड एपीआई और ऑनलाइन दस्तावेज़ हस्ताक्षर ऐप्स"
head_description: ".NET, Java और क्लाउड-आधारित अनुप्रयोगों के लिए सभी में एक दस्तावेज़ ई-हस्ताक्षर समाधान प्राप्त करें। सरल ड्रैग एंड ड्रॉप सुविधा का उपयोग करके सामान्य दस्तावेज़ स्वरूपों पर ऑनलाइन हस्ताक्षर करें"

############################# Header ############################
title: "दस्तावेज़ों पर हस्ताक्षर करें<br>Node.js एपीआई के साथ"
description: "प्रोग्रामर और अंतिम उपयोगकर्ताओं के लिए हमारे लचीले एपीआई और ऐप आधारित समाधानों का उपयोग करके किसी भी प्लेटफ़ॉर्म पर डिजिटल दस्तावेज़ों और छवियों पर हस्ताक्षर करें।"
words:
  for: "के लिए"

actions:
  main: "एनपीएम से डाउनलोड करें"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "लाइसेंसिंग"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "आरंभ करने के लिए तैयार हैं?"
  description: "GroupDocs.Signature सुविधाओं को निःशुल्क आज़माएँ या लाइसेंस का अनुरोध करें"

release:
  title: "संस्करण {0} जारी किया गया"
  notes: "देखें, क्या नया है"
  downloads: "डाउनलोड"

code:
  title: "Node.js द्वारा PDF पर हस्ताक्षर करना"
  more: "और ज्यादा उदाहरण"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```javascript {style=abap}   
    // पीडीएफ दस्तावेज़ का चयन करें
    let signature = new Signature("sample.pdf");
    
    // पाठ प्रदान करें
    let options = new TextSignOptions("John Smith");
    
    // रंग सेट करें
    options.ForeColor = Color.Red;
    
    // दस्तावेज़ पर हस्ताक्षर करें और फ़ाइल में सहेजें
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.हस्ताक्षर अवलोकन"
  description: "दस्तावेज़ हस्ताक्षरित लाइब्रेरी जो Node.js अनुप्रयोगों में उपयोग के लिए तैयार है"
  features:
    # feature loop
    - title: "Node.js के साथ व्यावसायिक दस्तावेज़ों के लिए डिजिटल हस्ताक्षर समाधान"
      content: "GroupDocs.Signature for Node.js via Java पीडीएफ, कार्यालय दस्तावेजों और छवियों के लिए डिजिटल हस्ताक्षर विकल्पों का एक व्यापक सेट प्रदान करता है। टेक्स्ट, बारकोड, चित्र, डिजिटल प्रमाणपत्र और मेटाडेटा उपलब्ध हैं। सुव्यवस्थित दस्तावेज़ प्रसंस्करण दक्षता सुनिश्चित करता है।"

    # feature loop
    - title: "हस्ताक्षरित दस्तावेज़ों का उन्नत हेरफेर"
      content: "GroupDocs.Signature आपको हस्ताक्षरित दस्तावेज़ों को संसाधित करने का अधिकार देता है। विभिन्न मानदंडों का उपयोग करके हस्ताक्षर खोजें और मान्य करें। इसके अतिरिक्त, विस्तृत दस्तावेज़ जानकारी निकालें या पृष्ठों की पूर्वावलोकन छवियां बनाएं।"

    # feature loop
    - title: "विविध आउटपुट प्रारूप"
      content: "हमारा समाधान हस्ताक्षरित दस्तावेज़ों के आउटपुट स्वरूप पर व्यापक नियंत्रण प्रदान करता है। किसी भी पृष्ठ पर हस्ताक्षरों को सटीक रूप से रखें और उनके स्वरूप को अनुकूलित करें। हस्ताक्षरित दस्तावेज़ों को अनेक समर्थित प्रारूपों में सहेजें और वैकल्पिक रूप से उन्हें पासवर्ड से सुरक्षित करें।"

############################# Platforms ############################
platforms:
  enable: true
  title: "मंच की स्वतंत्रता"
  description: "GroupDocs.Signature for Node.js via Java विभिन्न ऑपरेटिंग सिस्टम के साथ दस्तावेज़ प्रसंस्करण करता है"
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
  title: "समर्थित फ़ाइल स्वरूप"
  description: |
    GroupDocs.Signature for Node.js via Java [लोकप्रिय फ़ाइल स्वरूपों](https://docs.groupdocs.com/signature/java/supported-document-formats/) के लिए संचालन की सुविधा प्रदान करता है।
  groups:
    # group loop
    - color: "green"
      content: |
        ### माइक्रोसॉफ्ट ऑफिस प्रारूप
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### छवियाँ एवं अन्य प्रारूप
        * **पोर्टेबल:** PDF
        * **इमेजिस:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **अन्य कार्यालय प्रारूप:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### अन्य प्रारूप
        * **वेब:** HTML, MHTML
        * **अभिलेखागार:** ZIP, TAR, 7Z
        * **प्रमाण पत्र:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Signature की विशेषताएं"
  description: "डिजिटल हस्ताक्षर के साथ पीडीएफ, कार्यालय दस्तावेजों और छवियों पर हस्ताक्षर करें"

  items:
    # feature loop
    - icon: "sign"
      title: "व्यावसायिक हस्ताक्षर"
      content: "दस्तावेज़ों पर हस्ताक्षर करने के लिए विभिन्न प्रकार के हस्ताक्षर नियोजित करें। किसी भी पृष्ठ स्थान पर सटीक रूप से डिजिटल हस्ताक्षर रखें।"

    # feature loop
    - icon: "custom"
      title: "हस्ताक्षर उपस्थिति को अनुकूलित करना"
      content: "अपने वांछित परिणाम प्राप्त करने के लिए रंग, फ़ॉन्ट, बॉर्डर, रोटेशन और बहुत कुछ समायोजित करके हस्ताक्षर के दृश्य पहलुओं को तैयार करें।"

    # feature loop
    - icon: "password"
      title: "पासवर्ड से सुरक्षित दस्तावेज़"
      content: "कई समर्थित दस्तावेज़ प्रारूपों के लिए, अतिरिक्त सुरक्षा के लिए हस्ताक्षरित दस्तावेज़ों को पासवर्ड से सुरक्षित रखें।"

    # feature loop
    - icon: "protect"
      title: "अनधिकृत संशोधनों को रोकना"
      content: "डिजिटल प्रमाणपत्रों से हस्ताक्षरित महत्वपूर्ण व्यावसायिक दस्तावेज़ों को अनधिकृत परिवर्तनों से सुरक्षित रखें।"

    # feature loop
    - icon: "convert"
      title: "वांछित आउटपुट प्रारूप"
      content: "किसी भी समर्थित प्रारूप में हस्ताक्षरित दस्तावेज़ आसानी से प्राप्त करें। एमएस वर्ड दस्तावेजों को आसानी से पीडीएफ प्रारूप में बदलें।"

    # feature loop
    - icon: "preview"
      title: "दस्तावेज़ पूर्वावलोकन"
      content: "भविष्य की ज़रूरतों के लिए अलग-अलग दस्तावेज़ पृष्ठों को छवियों के रूप में सहेजें।"

    # feature loop
    - icon: "search"
      title: "हस्ताक्षर खोज"
      content: "अपने दस्तावेज़ों में पहले जोड़े गए हस्ताक्षरों के बारे में जानकारी प्राप्त करें।"

    # feature loop
    - icon: "validate"
      title: "दस्तावेज़ सत्यापन"
      content: "किसी भी दस्तावेज़ में प्रस्तुत हस्ताक्षरों की प्रामाणिकता सत्यापित करें।"

    # feature loop
    - icon: "update"
      title: "हस्ताक्षर प्रबंधन"
      content: "किसी भी दस्तावेज़ पृष्ठ पर रखे गए किसी भी हस्ताक्षर को हटाएं, स्थानांतरित करें या संशोधित करें।"

############################# Code samples ############################
code_samples:
  enable: true
  title: "कोड नमूने"
  description: "विशिष्ट GroupDocs.Signature for Node.js via Java परिचालनों को दर्शाने वाले उदाहरणात्मक उदाहरण"
  items:
    # code sample loop
    - title: "पीडीएफ को क्यूआर कोड से चिह्नित करें"
      content: |
        [बारकोड](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) को विशिष्ट पीडीएफ दस्तावेज़ पृष्ठों में शामिल करने से व्यावसायिक प्रक्रियाओं को सुव्यवस्थित किया जा सकता है। यह अनुभाग GroupDocs.Signature for Node.js via Java का उपयोग करके QR कोड जोड़ने का एक उदाहरण प्रदान करता है।
        {{< landing/code title="पीडीएफ में क्यूआर कोड कैसे डालें।">}}
        ```javascript {style=abap}
        // हस्ताक्षर करने के लिए दस्तावेज़ लोड करें
        let signature = new Signature("file_to_sign.pdf");
        
        // पूर्वनिर्धारित पाठ के साथ QR कोड विकल्प बनाएं
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // पृष्ठ पर क्यूआर कोड एन्कोडिंग प्रकार और स्थिति कॉन्फ़िगर करें
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // दस्तावेज़ पर हस्ताक्षर करें और इसे परिणाम फ़ाइल के रूप में सहेजें
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "डिजिटल हस्ताक्षर के साथ DOCX की सुरक्षा करना"
      content: |
        [अपने दस्तावेज़ों को सुरक्षित रखें](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) डिजिटल प्रमाणपत्रों के आधार पर हस्ताक्षर द्वारा। डिजिटल हस्ताक्षर आपके व्यावसायिक दस्तावेज़ों को सामग्री बदलने से बचाते हैं।
        {{< landing/code title="यहां दस्तावेज़ की अखंडता सुनिश्चित करने का तरीका बताया गया है।">}}
        ```javascript {style=abap}   
        // दस्तावेज़ को डिजिटल रूप से हस्ताक्षरित करने के लिए लोड करें
        let signature = new Signature("file_to_sign.pdf");
        
        // डिजिटल हस्ताक्षर विकल्प निर्दिष्ट करें और प्रमाणपत्र फ़ाइल का पथ प्रदान करें
        let options = new DigitalSignOptions("certificate.pfx");

        // प्रमाणपत्र पासवर्ड सेट करें
        options.Password = "1234567890";

        // दस्तावेज़ पर हस्ताक्षर करें और इसे वांछित पथ पर सहेजें
        signature.Sign("digitally_signed.pdf", options);

        ```
        {{< /landing/code >}}

---
