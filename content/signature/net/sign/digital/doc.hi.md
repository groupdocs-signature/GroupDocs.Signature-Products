---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Doc
productName: .NET
lang: hi
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Doc for C#

############################# Head ############################
head_title: "C# के साथ Doc फ़ाइल में डिजिटल इलेक्ट्रॉनिक हस्ताक्षर जोड़ना"
head_description: "कोड की कुछ पंक्तियों का उपयोग करके .NET के लिए Doc फ़ाइल पर डिजिटल हस्ताक्षर लगाएं। दर्जनों फ़ाइल स्वरूपों पर हस्ताक्षर करने के लिए GroupDocs दस्तावेज़ हस्ताक्षर API का उपयोग करें।"

############################# Header ############################
title: "C# में Digital हस्ताक्षर वाली Doc फ़ाइलें eSign करें"
description: ".NET कोड की कुछ पंक्तियों के साथ Digital हस्ताक्षर कैसे जोड़ें"
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
    title: "GroupDocs.Signature for .NET डिजिटल सिग्नेचर API के बारे में"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) डिजिटल प्रमाणपत्रों के साथ डिजिटल इलेक्ट्रॉनिक हस्ताक्षर के साथ दस्तावेज़ तैयार करने के लिए एक लोकप्रिय एपीआई है। डिजिटल हस्ताक्षर के लिए एपीआई पासवर्ड से सुरक्षित निजी और सार्वजनिक कुंजी के साथ दस्तावेज़ तैयार करने के लिए पीएफएक्स प्रमाणपत्र फाइलों का उपयोग करता है। डिजिटल हस्ताक्षर का उपयोग ई-साइन पीडीएफ विशेष पृष्ठ के साथ व्यावसायिक दस्तावेजों को प्रमाणित करने, वर्ड्स, एक्सेल, पावरपॉइंट फाइलों और ओपन ऑफिस दस्तावेजों जैसे संपूर्ण माइक्रोसॉफ्ट ऑफिस दस्तावेजों को प्रमाणित करने के लिए किया जा सकता है। ग्राहक आसानी से हस्ताक्षर में हेरफेर कर सकते हैं जैसे उन्हें संपादित करना, हटाना या समायोजित करना। एपीआई हस्ताक्षर खोजने और सत्यापित करने का एक तरीका प्रदान करता है। इसके अलावा, हस्ताक्षर अनुकूलन के लिए बहुत सारी क्षमताएं प्रदान की जाती हैं।
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C# में Digital के साथ Doc पर हस्ताक्षर करने के चरण"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) जल्दी और आसानी से Digital हस्ताक्षर के साथ Doc दस्तावेज़ों पर हस्ताक्षर करने की क्षमता प्रदान करता है।
        
        * सिग्नेचर क्लास का एक इंस्टेंस बनाएं जो {{फाइलफॉर्मेट}} फाइल को पाथ या मेमोरी स्ट्रीम के रूप में साइन करने वाली फाइल प्रदान करता है
        * साइनऑप्शन क्लास को इंस्टेंट करें और सभी मांगे गए डेटा को सेट करें।
        * Signature.Sign() मेथड पासिंग आउटपुट Doc फाइल या मेमोरी स्ट्रीम को आमंत्रित करें

    title_right: " सिस्टम आवश्यकताएं"
    content_right: |
        GroupDocs.Signature for .NET सभी प्रमुख प्लेटफॉर्म और ऑपरेटिंग सिस्टम पर समर्थित हैं। नीचे दिए गए कोड को निष्पादित करने से पहले, कृपया सुनिश्चित करें कि आपके सिस्टम पर निम्नलिखित पूर्वापेक्षाएँ स्थापित हैं।

        * ऑपरेटिंग सिस्टम: माइक्रोसॉफ्ट विंडोज, लिनक्स, मैकओएस
        * विकास परिवेश: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature) से नवीनतम GroupDocs.Signature for .NET प्राप्त करें
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";
        // Set up output file
        string outputFilePath = "output.doc";
        // Provide digital certificate
        string certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                DigitalSignOptions options = new DigitalSignOptions(certificateFilePath)
                {
                    // set certificate password
                    Password = "1234567890",
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Doc document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Digital लाइव डेमो के साथ Doc दस्तावेज़ों पर हस्ताक्षर करना"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) वेबसाइट पर जाकर अभी विभिन्न हस्ताक्षरों के साथ Doc फ़ाइल पर हस्ताक्षर करें। मुफ्त ऑनलाइन डेमो आपका इंतजार कर रहा है।          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# के लिए अन्य समर्थित Digital हस्ताक्षर"
    content: |
        "आप अन्य हस्ताक्षर प्रकारों के साथ Doc पर भी हस्ताक्षर कर सकते हैं। कृपया नीचे दी गई सूची देखें।"
    format: 
       
       
back_to_top:
    enable: true
---