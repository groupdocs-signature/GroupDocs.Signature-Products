---
############################# Static ############################
layout: "landing"
date: 2023-09-13T10:36:51
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
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, जावा, क्लाउड एपीआई और ऑनलाइन दस्तावेज़ हस्ताक्षर ऐप्स"
head_description: ".NET, Java और क्लाउड-आधारित अनुप्रयोगों के लिए सभी में एक दस्तावेज़ ई-हस्ताक्षर समाधान प्राप्त करें। सरल ड्रैग एंड ड्रॉप सुविधा का उपयोग करके सामान्य दस्तावेज़ स्वरूपों पर ऑनलाइन हस्ताक्षर करें"

############################# Header ############################
title: "दस्तावेज़ों पर हस्ताक्षर करें<br>.NET एपीआई के माध्यम से"
description: "प्रोग्रामर और अंतिम उपयोगकर्ताओं के लिए हमारे लचीले एपीआई और ऐप आधारित समाधानों का उपयोग करके किसी भी प्लेटफ़ॉर्म पर डिजिटल दस्तावेज़ों और छवियों पर हस्ताक्षर करें।"
words:
  for: "के लिए"

actions:
  main: "नि:शुल्क नुगेट डाउनलोड"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "लाइसेंसिंग"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "आरंभ करने के लिए तैयार हैं?"
  description: "GroupDocs.Signature सुविधाओं को निःशुल्क आज़माएँ या लाइसेंस का अनुरोध करें"

release:
  title: "संस्करण {0} जारी किया गया"
  notes: "देखें, क्या नया है"
  downloads: "डाउनलोड"

code:
  title: "सी# में पीडीएफ फाइलों पर हस्ताक्षर करें"
  more: "और ज्यादा उदाहरण"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // पीडीएफ दस्तावेज़ का चयन करें
    using (Signature signature = new Signature("sample.pdf"))
    {
        // पाठ प्रदान करें
        var options = new TextSignOptions("John Smith")
        {
            // रंग सेट करें
            ForeColor = Color.Red
        };
        // दस्तावेज़ पर हस्ताक्षर करें और फ़ाइल में सहेजें
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.हस्ताक्षर अवलोकन"
  description: ".NET अनुप्रयोगों में दस्तावेज़ पर हस्ताक्षर करने और संबंधित संचालन करने के लिए एपीआई"
  features:
    # feature loop
    - title: "C# में व्यावसायिक दस्तावेज़ों में हस्ताक्षर जोड़ना"
      content: "दस्तावेज़ों पर हस्ताक्षर: .NET के लिए GroupDocs.Signature के साथ, आप PDF और Office दस्तावेज़ों में विभिन्न प्रकार के हस्ताक्षर, जैसे टेक्स्ट, चित्र, बारकोड और डिजिटल प्रमाणपत्र जोड़ सकते हैं। यह एपीआई आपको छिपे हुए मेटाडेटा सहित लगभग किसी भी डेटा प्रकार के साथ अपने दस्तावेज़ों पर हस्ताक्षर करने की अनुमति देता है।"

    # feature loop
    - title: "हस्ताक्षरित दस्तावेज़ों का प्रसंस्करण"
      content: "अतिरिक्त प्रसंस्करण: आप GroupDocs.Signature का उपयोग करके हस्ताक्षरित दस्तावेज़ों पर शक्तिशाली संचालन कर सकते हैं। इसमें व्यावसायिक दस्तावेज़ों में मौजूदा हस्ताक्षरों की खोज करना और विशिष्ट मानदंडों का उपयोग करके उन्हें सत्यापित करना शामिल है। इसके अतिरिक्त, आप इस .NET API के माध्यम से दस्तावेज़ जानकारी और पूर्वावलोकन पृष्ठों को पुनः प्राप्त कर सकते हैं।"

    # feature loop
    - title: "परिणामों को अनुकूलित करना"
      content: ".NET के लिए GroupDocs.Signature व्यापक अनुकूलन विकल्प प्रदान करता है। आप दस्तावेज़ पृष्ठ पर कहीं भी हस्ताक्षरों को सटीक रूप से रख सकते हैं और विभिन्न सेटिंग्स का उपयोग करके उनके स्वरूप को समायोजित कर सकते हैं। इसके अलावा, यह एपीआई संसाधित दस्तावेज़ों को समर्थित प्रारूपों की एक विस्तृत श्रृंखला में सहेजने का समर्थन करता है।"

############################# Platforms ############################
platforms:
  enable: true
  title: "मंच की स्वतंत्रता"
  description: ".NET के लिए GroupDocs.Signature निम्नलिखित ऑपरेटिंग सिस्टम, फ्रेमवर्क और पैकेज मैनेजर का समर्थन करता है"
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
    .NET के लिए GroupDocs.Signature निम्नलिखित [फ़ाइल स्वरूपों] (https://docs.groupdocs.com/signature/net/supported-document-formats/) के साथ संचालन का समर्थन करता है।
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
  description: "पीडीएफ़, कार्यालय दस्तावेज़ों और छवियों पर तेज़ी से और सटीकता से हस्ताक्षर करना"

  items:
    # feature loop
    - icon: "merge"
      title: "दस्तावेज़ पर हस्ताक्षर"
      content: "व्यावसायिक दस्तावेज़ों पर किसी भी निर्दिष्ट स्थान पर एक या एकाधिक समर्थित प्रकार के हस्ताक्षर सटीक रूप से जोड़ें।"

    # feature loop
    - icon: "split"
      title: "हस्ताक्षर अनुकूलित करें"
      content: "हस्ताक्षरों की उपस्थिति को कॉन्फ़िगर करने के लिए रंग, फ़ॉन्ट, बॉर्डर, रोटेशन इत्यादि जैसी सुविधाओं का उपयोग करें।"

    # feature loop
    - icon: "move"
      title: "दस्तावेज़ पासवर्ड सुरक्षा"
      content: "हस्ताक्षर करने के बाद पासवर्ड सेट करके कुछ दस्तावेज़ प्रकारों को सुरक्षित करें।"

    # feature loop
    - icon: "remove"
      title: "परिवर्तनों से सुरक्षा"
      content: "डिजिटल प्रमाणपत्र के साथ हस्ताक्षर जोड़ने के बाद महत्वपूर्ण व्यावसायिक दस्तावेज़ों में परिवर्तन रोकें।"

    # feature loop
    - icon: "rotate"
      title: "हस्ताक्षरित फ़ाइलों को अन्य प्रारूपों में कनवर्ट करें"
      content: "हस्ताक्षरित फ़ाइलों को वांछित प्रारूपों में परिवर्तित करें, जैसे किसी Word दस्तावेज़ को PDF के रूप में सहेजना।"

    # feature loop
    - icon: "swap"
      title: "पृष्ठ पूर्वावलोकन निकालें"
      content: "भविष्य के प्रसंस्करण के लिए हस्ताक्षरित दस्तावेज़ों से अलग-अलग छवियों के रूप में पृष्ठ निकालें।"

    # feature loop
    - icon: "extract"
      title: "दस्तावेजों में हस्ताक्षर खोज"
      content: "विशिष्ट दस्तावेज़ों में पहले जोड़े गए हस्ताक्षरों के बारे में जानकारी प्राप्त करें।"

    # feature loop
    - icon: "orientation"
      title: "हस्ताक्षरित दस्तावेज़ों को मान्य करें"
      content: "सत्यापन सुविधाओं का उपयोग करके दस्तावेज़ों पर उचित हस्ताक्षर की पुष्टि करें।"

    # feature loop
    - icon: "preview"
      title: "हस्ताक्षर अद्यतन करें या हटाएँ"
      content: "किसी पृष्ठ पर आसानी से विशिष्ट हस्ताक्षरों का स्थान बदलें, उनके पाठ को संशोधित करें, या बिना किसी समस्या के उन्हें हटा दें।"

############################# Code samples ############################
code_samples:
  enable: true
  title: "कोड नमूने"
  description: "कुछ लोग .NET संचालन के लिए विशिष्ट GroupDocs.Signature के मामलों का उपयोग करते हैं"
  items:
    # code sample loop
    - title: "पीडीएफ में क्यूआर-कोड जोड़ें"
      content: |
        पीडीएफ दस्तावेज़ों के विशिष्ट पृष्ठों में [क्यूआर-कोड](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) जोड़ने से व्यावसायिक प्रक्रियाओं में सुधार हो सकता है। नीचे GroupDocs.Signature का उपयोग करके QR कोड जोड़ने का एक उदाहरण दिया गया है।
        {{< landing/code title="पीडीएफ में क्यूआर कोड कैसे डालें।">}}
        ```csharp {style=abap}
        // हस्ताक्षर करने के लिए दस्तावेज़ लोड करें
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // पूर्वनिर्धारित पाठ के साथ QR कोड विकल्प बनाएं
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // पृष्ठ पर क्यूआर कोड एन्कोडिंग प्रकार और स्थिति कॉन्फ़िगर करें
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // दस्तावेज़ पर हस्ताक्षर करें और इसे परिणाम फ़ाइल के रूप में सहेजें
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "डिजिटल प्रमाणपत्र का उपयोग करके DOCX दस्तावेज़ की सुरक्षा करना"
      content: |
        आप डिजिटल प्रमाणपत्र के रूप में संग्रहीत व्यक्तिगत या कॉर्पोरेट हस्ताक्षरों का उपयोग करके [दस्तावेज़ को सुरक्षित रखें](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) कर सकते हैं। ऐसे संरक्षित दस्तावेजों को हस्ताक्षर को अमान्य किए बिना संशोधित नहीं किया जा सकता है।
        {{< landing/code title="यहां दस्तावेज़ की अखंडता सुनिश्चित करने का तरीका बताया गया है।">}}
        ```csharp {style=abap}   
        // दस्तावेज़ को डिजिटल रूप से हस्ताक्षरित करने के लिए लोड करें
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // डिजिटल हस्ताक्षर विकल्प निर्दिष्ट करें और प्रमाणपत्र फ़ाइल का पथ प्रदान करें
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // प्रमाणपत्र पासवर्ड सेट करें
                Password = "1234567890"
            };
            // दस्तावेज़ पर हस्ताक्षर करें और इसे वांछित पथ पर सहेजें
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
