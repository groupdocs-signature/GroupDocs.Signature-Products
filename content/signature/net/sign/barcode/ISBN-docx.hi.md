---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: ISBN
fileformat: Docx
productName: .NET
lang: hi
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Docx for C#

############################# Head ############################
head_title: "C# में ISBN बारकोड के साथ eSign Docx दस्तावेज़"
head_description: "ISBN बारकोड सिग्नेचर बनाएं और इसे Docx डॉक्यूमेंट पर .NET के साथ कोड की दो पंक्तियों का उपयोग करके लगाएं। विभिन्न फ़ाइल स्वरूपों पर हस्ताक्षर करने के लिए GroupDocs दस्तावेज़ हस्ताक्षर API का उपयोग करें।"

############################# Header ############################
title: "C# में Docx दस्तावेज़ के लिए ISBN बारकोड हस्ताक्षर जेनरेट करें"
description: "ISBN बारकोड के साथ अपने Docx व्यावसायिक दस्तावेज़ों पर ई-हस्ताक्षर करें। हस्ताक्षर विकल्प सेट करने के लिए कोड की कुछ पंक्तियों के साथ जल्दी और आसानी से बारकोड हस्ताक्षर उत्पन्न करें।"
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
    title: "GroupDocs.Signature for .NET बारकोड सिग्नेचर API के बारे में।"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN जैसे बारकोड प्रकारों का उपयोग करके डिजिटल दस्तावेज़ ई-हस्ताक्षर को प्रबंधित करने के लिए एक त्वरित और आसान एपीआई है। , ITF14 और कई अन्य। ग्राहक आवश्यक टेक्स्ट प्रदान करके आसानी से बारकोड बना सकते हैं और उन्हें PDF, Microsoft Office Words Documents, Microsoft Office Excel कार्यपुस्तिकाओं, MS PowerPoint प्रस्तुतियों, Adobe Photoshop फ़ाइलों और विभिन्न छवि प्रारूपों में डाल सकते हैं। दस्तावेज़ों में रखे गए बारकोड को अद्यतन, खोजा, सत्यापित, हटाया या पूर्वावलोकन किया जा सकता है। इसके अलावा, बारकोड अनुकूलन समर्थित है।
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C# में Barcode के साथ Docx पर हस्ताक्षर करने के चरण"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) जल्दी और आसानी से Barcode हस्ताक्षर के साथ Docx दस्तावेज़ों पर हस्ताक्षर करने की क्षमता प्रदान करता है।
        
        * सिग्नेचर क्लास का एक इंस्टेंस बनाएं जो Barcode फाइल को पाथ या मेमोरी स्ट्रीम के रूप में साइन करने वाली फाइल प्रदान करता है
        * साइनऑप्शन क्लास को इंस्टेंट करें और सभी मांगे गए डेटा को सेट करें।
        * Signature.Sign() मेथड पासिंग आउटपुट Docx फाइल या मेमोरी स्ट्रीम को आमंत्रित करें

    title_right: " सिस्टम आवश्यकताएं"
    content_right: |
        GroupDocs.Signature for .NET सभी प्रमुख प्लेटफॉर्म और ऑपरेटिंग सिस्टम पर समर्थित हैं। नीचे दिए गए कोड को निष्पादित करने से पहले, कृपया सुनिश्चित करें कि आपके सिस्टम पर निम्नलिखित पूर्वापेक्षाएँ स्थापित हैं।

        * ऑपरेटिंग सिस्टम: माइक्रोसॉफ्ट विंडोज, लिनक्स, मैकओएस
        * विकास परिवेश: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature) से नवीनतम GroupDocs.Signature for .NET प्राप्त करें
         
    code: |
        ```csharp    
        
        // Set up input Docx file
        string filePath = "input.docx";
        // Set up output file
        string outputFilePath = "output.docx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.ISBN,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Docx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Barcode लाइव डेमो के साथ Docx दस्तावेज़ों पर हस्ताक्षर करना"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) वेबसाइट पर जाकर अभी विभिन्न हस्ताक्षरों के साथ Docx फ़ाइल पर हस्ताक्षर करें। मुफ्त ऑनलाइन डेमो आपका इंतजार कर रहा है।

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About ISBN Barcode"
          content: |
            इंटरनेशनल स्टैंडर्ड बुक नंबर (आईएसबीएन) एक संख्यात्मक वाणिज्यिक पुस्तक पहचानकर्ता है जिसका उद्देश्य अद्वितीय होना है। [ए] [बी] प्रकाशक अंतरराष्ट्रीय आईएसबीएन एजेंसी के एक सहयोगी से आईएसबीएन खरीदते हैं।
          characterset: |
             संख्यात्मक अंक (0-9)।
          textcapacity: |
             बिल्कुल 9 अंक + 1 चेक अंक।
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# के लिए अन्य समर्थित Barcode हस्ताक्षर"
    content: |
        "आप अन्य हस्ताक्षर प्रकारों के साथ Docx पर भी हस्ताक्षर कर सकते हैं। कृपया नीचे दी गई सूची देखें।"
    format: 
        
       
back_to_top:
    enable: true
---