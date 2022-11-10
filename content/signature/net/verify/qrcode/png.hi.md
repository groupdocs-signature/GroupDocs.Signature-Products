---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Png
productName: .NET
lang: hi
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Png for C#

############################# Head ############################
head_title: "C# के माध्यम से Png फ़ाइलों के लिए Qrcode हस्ताक्षरों का सत्यापन"
head_description: "Png दस्तावेज़ों और उनके Qrcode हस्ताक्षरों को सत्यापित करने के लिए .NET कोड की केवल कुछ पंक्तियों का उपयोग करें।"

############################# Header ############################
title: "Qrcode Png फाइलों के लिए हस्ताक्षर सत्यापन"
description: ".NET के लिए API Qrcode हस्ताक्षरों को Png दस्तावेज़ों पर सत्यापित करने का अवसर प्रदान करता है। आपके Png दस्तावेज़ों के अंदर ई-हस्ताक्षर का सत्यापन जल्दी और आसानी से किया जा सकता है।"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "नई GroupDocs.Signature for .NET API सुविधाएं खोजें"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API इलेक्ट्रॉनिक हस्ताक्षरों का उपयोग करके कई दस्तावेज़ प्रारूपों को संसाधित करने के व्यापक तरीके प्रदान करता है। टेक्स्ट, इमेज, डिजिटल सर्टिफिकेट, बारकोड, क्यूआर-कोड, स्टैम्प या मेटाडेटा जैसे कई प्रकार के डिजिटल हस्ताक्षर समर्थित हैं। ग्राहक PDF, MS Word दस्तावेज़, MS Excel कार्यपुस्तिका, MS PowerPoint प्रस्तुतियों, Adobe Photoshop फ़ाइलों और विभिन्न छवि प्रारूपों में डिजिटल हस्ताक्षर जोड़, हटा, संपादित, मान्य या खोज सकते हैं। अतिरिक्त सुविधाओं और सेटिंग्स की आश्चर्यजनक संख्या उपलब्ध है।
    

############################# Steps ############################
steps:
    enable: true
    title_left: "अपने Png दस्तावेज़ में Qrcode हस्ताक्षरों की पुष्टि कैसे करें"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) में Qrcode Png दस्तावेज़ों पर रखे गए हस्ताक्षरों के सत्यापन जैसी उपयोगी सुविधाएं शामिल हैं। अतिरिक्त कोड लागू किए बिना इस अवसर का उपयोग करें।
        
        * सबसे पहले, सिग्नेचर क्लास को एक दस्तावेज़ के लिए एक कंस्ट्रक्टर पैरामीटर पथ के रूप में प्रदान करना, जिसे सत्यापित किया जाना है।
        * दूसरे, एक नया VerifyOptions ऑब्जेक्ट बनाएं और सभी आवश्यक गुण सेट करें।
        * अंत में, सिग्नेचर के ऑब्जेक्ट वेरिफाई मेथड को VerifyOptions इंस्टेंस पास करने का आह्वान करें।
        * फिर सत्यापन परिणामों की प्रक्रिया करें।

    title_right: "सिस्टम आवश्यकताएं"
    content_right: |
        GroupDocs.Signature for .NET सभी प्रमुख प्लेटफॉर्म और ऑपरेटिंग सिस्टम पर समर्थित हैं। नीचे दिए गए कोड को निष्पादित करने से पहले, कृपया सुनिश्चित करें कि आपके सिस्टम पर निम्नलिखित पूर्वापेक्षाएँ स्थापित हैं।

        * ऑपरेटिंग सिस्टम: माइक्रोसॉफ्ट विंडोज, लिनक्स, मैकओएस
        * विकास परिवेश: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature) से GroupDocs.Signature for .NET का नवीनतम संस्करण डाउनलोड करें
         
    code: |
        ```csharp    
                
        // Set up input Png file
        string filePath = "input.png";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                QrCodeVerifyOptions options = new QrCodeVerifyOptions()
                {
                    // process only first page
                    PagesSetup = new PagesSetup() { FirstPage = true },
                    AllPages = false,
                    // set up text match type
                    MatchType = TextMatchType.StartsWith,
                    // specify text pattern to search
                    Text = "QrCode text",
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Qrcode सिग्नेचर लाइव डेमो के साथ साइन करना"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) वेबसाइट पर जाकर अभी Png फ़ाइल में विभिन्न इलेक्ट्रॉनिक हस्ताक्षर जोड़ें।          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# का उपयोग करके अन्य Qrcode हस्ताक्षर सत्यापित करें"
    content: |
        "विभिन्न दस्तावेजों में रखे गए इलेक्ट्रॉनिक हस्ताक्षरों का सत्यापन। नीचे बताए अनुसार लोकप्रिय फ़ाइल स्वरूपों में हस्ताक्षरों की गुणवत्ता की जाँच करें।"
    format: 
       
       
back_to_top:
    enable: true
---