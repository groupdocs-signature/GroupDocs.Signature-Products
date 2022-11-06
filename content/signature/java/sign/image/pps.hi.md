---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Pps
productName: Java
lang: hi
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Pps for Java

############################# Head ############################
head_title: "Image हस्ताक्षर को Pps फ़ाइल में Java के साथ जोड़ना"
head_description: "कोड की कुछ पंक्तियों का उपयोग करके Image हस्ताक्षर को Pps फ़ाइल पर Java के लिए रखें। दर्जनों फ़ाइल स्वरूपों पर हस्ताक्षर करने के लिए GroupDocs दस्तावेज़ हस्ताक्षर API का उपयोग करें।"

############################# Header ############################
title: "Java में Pps Image हस्ताक्षर वाली फाइलों पर हस्ताक्षर करें"
description: "Java कोड की कुछ पंक्तियों के साथ Image हस्ताक्षर कैसे जोड़ें"
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
    title: "GroupDocs.Signature for Java इमेज सिग्नेचर API के बारे में"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) डिजिटल दस्तावेज़ ई-हस्ताक्षर के लिए एक लोकप्रिय एपीआई है। पाठ, चित्र, डिजिटल प्रमाणपत्र, बारकोड, क्यूआर-कोड, टिकट या मेटाडेटा जैसे हस्ताक्षर उपलब्ध हैं। हस्ताक्षर PDF, MS Word दस्तावेज़, MS Excel कार्यपुस्तिकाएँ, MS PowerPoint प्रस्तुतियाँ, Adobe Photoshop फ़ाइलें और विभिन्न छवि प्रारूपों पर रखे जा सकते हैं। ग्राहक अपने दस्तावेज़ पर हस्ताक्षर कर सकते हैं और उन दस्तावेज़ों पर रखे गए ई-हस्ताक्षरों को अपडेट, खोज, सत्यापित, हटा या पूर्वावलोकन कर सकते हैं। इसके अलावा, हस्ताक्षर अनुकूलन के लिए बहुत सारी क्षमताएं प्रदान की जाती हैं।
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Java में Image के साथ Pps पर हस्ताक्षर करने के चरण"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) जल्दी और आसानी से Image हस्ताक्षर के साथ Pps दस्तावेज़ों पर हस्ताक्षर करने की क्षमता प्रदान करता है।
        
        * सिग्नेचर क्लास का एक इंस्टेंस बनाएं जो {{फाइलफॉर्मेट}} फाइल को पाथ या मेमोरी स्ट्रीम के रूप में साइन करने वाली फाइल प्रदान करता है
        * साइनऑप्शन क्लास को इंस्टेंट करें और सभी मांगे गए डेटा को सेट करें।
        * Signature.Sign() मेथड पासिंग आउटपुट Pps फाइल या मेमोरी स्ट्रीम को आमंत्रित करें

    title_right: " सिस्टम आवश्यकताएं"
    content_right: |
        GroupDocs.Signature for Java सभी प्रमुख प्लेटफॉर्म और ऑपरेटिंग सिस्टम पर समर्थित हैं। नीचे दिए गए कोड को निष्पादित करने से पहले, कृपया सुनिश्चित करें कि आपके सिस्टम पर निम्नलिखित पूर्वापेक्षाएँ स्थापित हैं।

        * ऑपरेटिंग सिस्टम: माइक्रोसॉफ्ट विंडोज, लिनक्स, मैकओएस
        * विकास परिवेश: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) से नवीनतम GroupDocs.Signature for Java प्राप्त करें
         
    code: |
        ```java    
                
        // Set up input Pps file
        String filePath = "input.pps";
        // Set up output file
        String outputFilePath = "output.pps";
        // Provide image file
        String imageFilePath = "image.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        ImageSignOptions options = new ImageSignOptions(imageFilePath);

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Pps document
        SignResult result = signature.sign(outputFilePath, options);
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Image लाइव डेमो के साथ Pps दस्तावेज़ों पर हस्ताक्षर करना"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) वेबसाइट पर जाकर अभी विभिन्न हस्ताक्षरों के साथ Pps फ़ाइल पर हस्ताक्षर करें। मुफ्त ऑनलाइन डेमो आपका इंतजार कर रहा है।          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java के लिए अन्य समर्थित Image हस्ताक्षर"
    content: |
        "आप अन्य हस्ताक्षर प्रकारों के साथ Pps पर भी हस्ताक्षर कर सकते हैं। कृपया नीचे दी गई सूची देखें।"
    format: 
       
       
back_to_top:
    enable: true
---