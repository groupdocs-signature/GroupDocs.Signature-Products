---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Xlsb
productName: Java
lang: hi
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Xlsb for Java

############################# Head ############################
head_title: "Java के माध्यम से Xlsb दस्तावेज़ों में मेटाडेटा इलेक्ट्रॉनिक हस्ताक्षर संलग्न करें"
head_description: "Java कोड की दो पंक्तियों का उपयोग करके अपने Xlsb दस्तावेज़ों के अंदर छिपे हुए इलेक्ट्रॉनिक हस्ताक्षर के रूप में मेटाडेटा का उपयोग करें। मेटाडेटा जानकारी के साथ अपने व्यावसायिक दस्तावेज़ों और फ़ाइलों पर ई-हस्ताक्षर करने के लिए GroupDocs दस्तावेज़ हस्ताक्षर API का उपयोग करें।"

############################# Header ############################
title: "Xlsb दस्तावेज़ के लिए Java के माध्यम से मेटाडेटा इलेक्ट्रॉनिक हस्ताक्षर सरल और उपयोग में आसान हैं!"
description: "छिपे हुए मेटाडेटा प्रविष्टियों के साथ अपने Xlsb दस्तावेज़ों और अनुबंधों पर ई-हस्ताक्षर करें। PDF, MS Word दस्तावेज़, MS Excel कार्यपुस्तिकाएँ, MS PowerPoint प्रस्तुतियाँ और बिना किसी समस्या और अतिरिक्त कोडिंग के विभिन्न छवि प्रारूपों के लिए मेटाडेटा उत्पन्न करें।"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Java मेटाडेटा हस्ताक्षर API के बारे में"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) डिजिटल दस्तावेज़ ई-हस्ताक्षर के लिए एक लोकप्रिय एपीआई है। पाठ, चित्र, डिजिटल प्रमाणपत्र, बारकोड, क्यूआर-कोड, टिकट या मेटाडेटा जैसे हस्ताक्षर उपलब्ध हैं। हस्ताक्षर PDF, MS Word दस्तावेज़, MS Excel कार्यपुस्तिकाएँ, MS PowerPoint प्रस्तुतियाँ, Adobe Photoshop फ़ाइलें और विभिन्न छवि प्रारूपों पर रखे जा सकते हैं। ग्राहक अपने दस्तावेज़ पर हस्ताक्षर कर सकते हैं और उन दस्तावेज़ों पर रखे गए ई-हस्ताक्षरों को अपडेट, खोज, सत्यापित, हटा या पूर्वावलोकन कर सकते हैं। इसके अलावा, हस्ताक्षर अनुकूलन के लिए बहुत सारी क्षमताएं प्रदान की जाती हैं।
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Java में Metadata के साथ Xlsb पर हस्ताक्षर करने के चरण"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) जल्दी और आसानी से Metadata हस्ताक्षर के साथ Xlsb दस्तावेज़ों पर हस्ताक्षर करने की क्षमता प्रदान करता है।
        
        * सिग्नेचर क्लास का एक इंस्टेंस बनाएं जो Metadata फाइल को पाथ या मेमोरी स्ट्रीम के रूप में साइन करने वाली फाइल प्रदान करता है
        * साइनऑप्शन क्लास को इंस्टेंट करें और सभी मांगे गए डेटा को सेट करें।
        * Signature.Sign() मेथड पासिंग आउटपुट Xlsb फाइल या मेमोरी स्ट्रीम को आमंत्रित करें

    title_right: " सिस्टम आवश्यकताएं"
    content_right: |
        GroupDocs.Signature for Java सभी प्रमुख प्लेटफॉर्म और ऑपरेटिंग सिस्टम पर समर्थित हैं। नीचे दिए गए कोड को निष्पादित करने से पहले, कृपया सुनिश्चित करें कि आपके सिस्टम पर निम्नलिखित पूर्वापेक्षाएँ स्थापित हैं।

        * ऑपरेटिंग सिस्टम: माइक्रोसॉफ्ट विंडोज, लिनक्स, मैकओएस
        * विकास परिवेश: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) से नवीनतम GroupDocs.Signature for Java प्राप्त करें
         
    code: |
        ```java    
                
        // Set up input Xlsb file
        String filePath = "input.xlsb";
        // Set up output file
        String outputFilePath = "output.xlsb";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        SpreadsheetMetadataSignature mdSign_Author = new SpreadsheetMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        SpreadsheetMetadataSignature mdSign_DocData = new SpreadsheetMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        SpreadsheetMetadataSignature mdSign_DocId = new SpreadsheetMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Xlsb document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Metadata लाइव डेमो के साथ Xlsb दस्तावेज़ों पर हस्ताक्षर करना"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) वेबसाइट पर जाकर अभी विभिन्न हस्ताक्षरों के साथ Xlsb फ़ाइल पर हस्ताक्षर करें। मुफ्त ऑनलाइन डेमो आपका इंतजार कर रहा है।          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java के लिए अन्य समर्थित Metadata हस्ताक्षर"
    content: |
        "आप अन्य हस्ताक्षर प्रकारों के साथ Xlsb पर भी हस्ताक्षर कर सकते हैं। कृपया नीचे दी गई सूची देखें।"
    format: 
       
       
back_to_top:
    enable: true
---