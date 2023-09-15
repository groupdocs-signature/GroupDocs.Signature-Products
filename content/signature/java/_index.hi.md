---
############################# Static ############################
layout: "landing"
date: 2023-09-14T19:07:21
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: hi
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: ".NET, जावा, क्लाउड एपीआई और ऑनलाइन दस्तावेज़ हस्ताक्षर ऐप्स"
head_description: ".NET, Java और क्लाउड-आधारित अनुप्रयोगों के लिए सभी में एक दस्तावेज़ ई-हस्ताक्षर समाधान प्राप्त करें। सरल ड्रैग एंड ड्रॉप सुविधा का उपयोग करके सामान्य दस्तावेज़ स्वरूपों पर ऑनलाइन हस्ताक्षर करें"

############################# Header ############################
title: "दस्तावेज़ों पर हस्ताक्षर करें<br>जावा एपीआई के माध्यम से"
description: "प्रोग्रामर और अंतिम उपयोगकर्ताओं के लिए हमारे लचीले एपीआई और ऐप आधारित समाधानों का उपयोग करके किसी भी प्लेटफ़ॉर्म पर डिजिटल दस्तावेज़ों और छवियों पर हस्ताक्षर करें।"
words:
  for: "के लिए"

actions:
  main: "निःशुल्क मेवेन डाउनलोड"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "लाइसेंसिंग"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "आरंभ करने के लिए तैयार हैं?"
  description: "GroupDocs.Signature सुविधाओं को निःशुल्क आज़माएँ या लाइसेंस का अनुरोध करें"

release:
  title: "संस्करण {0} जारी किया गया"
  notes: "देखें, क्या नया है"
  downloads: "डाउनलोड"

code:
  title: "जावा में पीडीएफ फाइलों पर हस्ताक्षर करें"
  more: "और ज्यादा उदाहरण"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // पीडीएफ दस्तावेज़ का चयन करें
    Signature signature = new Signature("sample.pdf");
    
    // पाठ प्रदान करें
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // दस्तावेज़ पर हस्ताक्षर करें और फ़ाइल में सहेजें
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.हस्ताक्षर अवलोकन"
  description: "जावा अनुप्रयोगों में दस्तावेज़ पर हस्ताक्षर और संबंधित संचालन करने के लिए एपीआई"
  features:
    # feature loop
    - title: "जावा में डिजिटल हस्ताक्षर के साथ बेहतर व्यावसायिक दस्तावेज़"
      content: "तीव्र और अनुकूलन योग्य हस्ताक्षर: जावा के लिए GroupDocs.Signature पीडीएफ, छवियों और कार्यालय दस्तावेजों के लिए डिजिटल हस्ताक्षर विकल्पों की एक विस्तृत श्रृंखला प्रदान करता है। आप टेक्स्ट, बारकोड, क्यूआर-कोड, डिजिटल प्रमाणपत्र, चित्र या छिपे हुए मेटाडेटा का उपयोग कर सकते हैं। दस्तावेज़ प्रसंस्करण तेज़ और कुशल है।"

    # feature loop
    - title: "हस्ताक्षरित दस्तावेजों में हेराफेरी करना"
      content: "उन्नत दस्तावेज़ प्रसंस्करण में जावा के लिए GroupDocs.Signature का उपयोग करके हस्ताक्षरित दस्तावेज़ों पर शक्तिशाली संचालन शामिल है। आप विभिन्न उपयोगी मानदंडों का उपयोग करके व्यावसायिक दस्तावेज़ों में जोड़े गए हस्ताक्षरों को खोज और सत्यापित कर सकते हैं। इसके अतिरिक्त, आप दस्तावेज़ के बारे में विस्तृत जानकारी प्राप्त कर सकते हैं या उसके पृष्ठों की पूर्वावलोकन छवियां प्राप्त कर सकते हैं।"

    # feature loop
    - title: "आउटपुट विकल्पों की विविधता"
      content: "मजबूत हस्ताक्षर विकल्प आपको जावा के लिए GroupDocs.Signature के साथ हस्ताक्षरित दस्तावेजों के लिए आउटपुट को अनुकूलित करने की अनुमति देते हैं। आप किसी भी दस्तावेज़ पृष्ठ पर किसी भी हस्ताक्षर को सटीक रूप से रख सकते हैं और उसके स्वरूप को विभिन्न तरीकों से कॉन्फ़िगर कर सकते हैं। जावा एपीआई कई समर्थित प्रारूपों में हस्ताक्षरित व्यावसायिक दस्तावेजों को सहेजने का समर्थन करता है और उन्हें पासवर्ड से सुरक्षित करने के विकल्प प्रदान करता है।"

############################# Platforms ############################
platforms:
  enable: true
  title: "मंच की स्वतंत्रता"
  description: "जावा के लिए GroupDocs.Signature निम्नलिखित ऑपरेटिंग सिस्टम, फ्रेमवर्क और पैकेज प्रबंधकों का समर्थन करता है"
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
  title: "समर्थित फ़ाइल स्वरूप"
  description: |
    जावा के लिए GroupDocs.Signature निम्नलिखित [फ़ाइल स्वरूपों](https://docs.groupdocs.com/signature/java/supported-document-formats/) के साथ संचालन का समर्थन करता है।
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
  title: "GroupDocs.हस्ताक्षर सुविधाएँ"
  description: "डिजिटल हस्ताक्षर के साथ पीडीएफ, कार्यालय दस्तावेज़ और छवियों पर हस्ताक्षर करना"

  items:
    # feature loop
    - icon: "sign"
      title: "हस्ताक्षर जोड़ना"
      content: "किसी भी पृष्ठ पर किसी भी स्थान पर सटीक रूप से डिजिटल हस्ताक्षर रखकर विभिन्न समर्थित हस्ताक्षर प्रकारों का उपयोग करके एक दस्तावेज़ पर हस्ताक्षर करें।"

    # feature loop
    - icon: "custom"
      title: "परिणामों को अनुकूलित करना"
      content: "वांछित परिणाम प्राप्त करने के लिए रंग, फ़ॉन्ट, बॉर्डर, रोटेशन और अन्य सुविधाओं को समायोजित करके हस्ताक्षर उपस्थिति को अनुकूलित करें।"

    # feature loop
    - icon: "password"
      title: "दस्तावेज़ों को पासवर्ड से सुरक्षित करना"
      content: "कई समर्थित दस्तावेज़ प्रकारों के लिए, आप हस्ताक्षरित दस्तावेज़ को पासवर्ड से सुरक्षित कर सकते हैं।"

    # feature loop
    - icon: "protect"
      title: "अनधिकृत परिवर्तनों को रोकना"
      content: "डिजिटल प्रमाणपत्र से हस्ताक्षरित महत्वपूर्ण व्यावसायिक दस्तावेज़ों को अनधिकृत संशोधनों से सुरक्षित रखें।"

    # feature loop
    - icon: "convert"
      title: "वांछित प्रारूपों में परिणाम प्राप्त करना"
      content: "किसी भी समर्थित प्रारूप में हस्ताक्षरित परिणाम फ़ाइलें आसानी से प्राप्त करें। आप एमएस वर्ड दस्तावेज़ों को भी आसानी से पीडीएफ में परिवर्तित कर सकते हैं।"

    # feature loop
    - icon: "preview"
      title: "दस्तावेज़ पूर्वावलोकन"
      content: "भविष्य में प्रसंस्करण के लिए दस्तावेज़ के किसी भी पृष्ठ को एक छवि के रूप में सहेजें।"

    # feature loop
    - icon: "search"
      title: "हस्ताक्षर खोजे जा रहे हैं"
      content: "विशिष्ट दस्तावेज़ों में पहले जोड़े गए हस्ताक्षरों के बारे में जानकारी प्राप्त करना संभव है।"

    # feature loop
    - icon: "validate"
      title: "दस्तावेज़ों का सत्यापन"
      content: "किसी भी हस्ताक्षरित दस्तावेज़ पर हस्ताक्षरों की शुद्धता को सत्यापित करें।"

    # feature loop
    - icon: "update"
      title: "हस्ताक्षर प्रबंधित करना"
      content: "एक बार जब किसी दस्तावेज़ पृष्ठ पर हस्ताक्षर रख दिया जाता है, तो उसे आवश्यकतानुसार हटाया, स्थानांतरित या अद्यतन किया जा सकता है।"

############################# Code samples ############################
code_samples:
  enable: true
  title: "कोड नमूने"
  description: "कुछ लोग जावा संचालन के लिए विशिष्ट GroupDocs.Signature के मामलों का उपयोग करते हैं"
  items:
    # code sample loop
    - title: "क्यूआर-कोड के साथ पीडीएफ दस्तावेज़ को बेहतर बनाएं"
      content: |
        पीडीएफ दस्तावेज़ों के विशिष्ट पृष्ठों में [क्यूआर-कोड](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) जोड़कर व्यावसायिक प्रक्रियाओं को बढ़ाना मूल्यवान हो सकता है। जावा के लिए GroupDocs.Signature का उपयोग करके QR कोड कैसे जोड़ें इसका एक उदाहरण है।
        {{< landing/code title="क्यूआर-कोड के साथ पीडीएफ दस्तावेज़ को बेहतर बनाएं">}}
        ```java {style=abap}
        // हस्ताक्षर करने के लिए दस्तावेज़ लोड करें
        Signature signature = new Signature("file_to_sign.pdf");
        
        // पूर्वनिर्धारित पाठ के साथ QR कोड विकल्प बनाएं
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // पृष्ठ पर क्यूआर कोड एन्कोडिंग प्रकार और स्थिति कॉन्फ़िगर करें
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // दस्तावेज़ पर हस्ताक्षर करें और इसे परिणाम फ़ाइल के रूप में सहेजें
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX की सुरक्षा के लिए डिजिटल हस्ताक्षर का उपयोग करें"
      content: |
        आप डिजिटल प्रमाणपत्र के रूप में संग्रहीत व्यक्तिगत या कॉर्पोरेट हस्ताक्षरों का उपयोग करके [दस्तावेज़ को सुरक्षित रख सकते हैं](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/)। प्रमाणपत्र के साथ सुरक्षित दस्तावेजों में हस्ताक्षर को अमान्य किए बिना बदलाव नहीं किया जा सकता।
        {{< landing/code title="DOCX की सुरक्षा के लिए डिजिटल हस्ताक्षर का उपयोग करें">}}
        ```java {style=abap}   
        // दस्तावेज़ को डिजिटल रूप से हस्ताक्षरित करने के लिए लोड करें
        Signature signature = new Signature("file_to_sign.pdf");
        
        // डिजिटल हस्ताक्षर विकल्प निर्दिष्ट करें और प्रमाणपत्र फ़ाइल का पथ प्रदान करें
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // प्रमाणपत्र पासवर्ड सेट करें
        options.setPassword("1234567890");

        // दस्तावेज़ पर हस्ताक्षर करें और इसे वांछित पथ पर सहेजें
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
