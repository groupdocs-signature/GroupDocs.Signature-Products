---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Interleaved2of5
fileformat: Png
productName: .NET
lang: hi
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Png for C#

############################# Head ############################
head_title: "C# में Interleaved2of5 बारकोड के साथ eSign Png दस्तावेज़"
head_description: "Interleaved2of5 बारकोड सिग्नेचर बनाएं और इसे Png डॉक्यूमेंट पर .NET के साथ कोड की दो पंक्तियों का उपयोग करके लगाएं। विभिन्न फ़ाइल स्वरूपों पर हस्ताक्षर करने के लिए GroupDocs दस्तावेज़ हस्ताक्षर API का उपयोग करें।"

############################# Header ############################
title: "C# में Png दस्तावेज़ के लिए Interleaved2of5 बारकोड हस्ताक्षर जेनरेट करें"
description: "Interleaved2of5 बारकोड के साथ अपने Png व्यावसायिक दस्तावेज़ों पर ई-हस्ताक्षर करें। हस्ताक्षर विकल्प सेट करने के लिए कोड की कुछ पंक्तियों के साथ जल्दी और आसानी से बारकोड हस्ताक्षर उत्पन्न करें।"
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
    title_left: "C# में Barcode के साथ Png पर हस्ताक्षर करने के चरण"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) जल्दी और आसानी से Barcode हस्ताक्षर के साथ Png दस्तावेज़ों पर हस्ताक्षर करने की क्षमता प्रदान करता है।
        
        * सिग्नेचर क्लास का एक इंस्टेंस बनाएं जो {{फाइलफॉर्मेट}} फाइल को पाथ या मेमोरी स्ट्रीम के रूप में साइन करने वाली फाइल प्रदान करता है
        * साइनऑप्शन क्लास को इंस्टेंट करें और सभी मांगे गए डेटा को सेट करें।
        * Signature.Sign() मेथड पासिंग आउटपुट Png फाइल या मेमोरी स्ट्रीम को आमंत्रित करें

    title_right: " सिस्टम आवश्यकताएं"
    content_right: |
        GroupDocs.Signature for .NET सभी प्रमुख प्लेटफॉर्म और ऑपरेटिंग सिस्टम पर समर्थित हैं। नीचे दिए गए कोड को निष्पादित करने से पहले, कृपया सुनिश्चित करें कि आपके सिस्टम पर निम्नलिखित पूर्वापेक्षाएँ स्थापित हैं।

        * ऑपरेटिंग सिस्टम: माइक्रोसॉफ्ट विंडोज, लिनक्स, मैकओएस
        * विकास परिवेश: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature) से नवीनतम GroupDocs.Signature for .NET प्राप्त करें
         
    code: |
        ```csharp    
        
        // Set up input Png file
        string filePath = "input.png";
        // Set up output file
        string outputFilePath = "output.png";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Interleaved2of5,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Png document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Barcode लाइव डेमो के साथ Png दस्तावेज़ों पर हस्ताक्षर करना"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) वेबसाइट पर जाकर अभी विभिन्न हस्ताक्षरों के साथ Png फ़ाइल पर हस्ताक्षर करें। मुफ्त ऑनलाइन डेमो आपका इंतजार कर रहा है।

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Interleaved2of5 Barcode"
          content: |
            5 का इंटरलीव्ड 2 (आईटीएफ) एक सतत दो-चौड़ाई वाला बारकोड सिम्बॉलॉजी एन्कोडिंग अंक है। यह 135 फिल्म पर, आईटीएफ -14 बारकोड के लिए और कुछ उत्पादों के डिब्बों पर व्यावसायिक रूप से उपयोग किया जाता है, जबकि अंदर के उत्पादों को यूपीसी या ईएएन के साथ लेबल किया जाता है।
          characterset: |
             संख्यात्मक अंक (0-9)।
          textcapacity: |
             चर लंबाई।
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAB8AAACGCAYAAAAlx1GyAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAFdSURBVHhe7Y0xCkJRAMPe/S/9BSFLqHaSN9hAhyzNeS6y+BUWv8LX+DnnPfjkHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3X+K9Z/Ar/Gn+eF5E2tt5Q4JATAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# के लिए अन्य समर्थित Barcode हस्ताक्षर"
    content: |
        "आप अन्य हस्ताक्षर प्रकारों के साथ Png पर भी हस्ताक्षर कर सकते हैं। कृपया नीचे दी गई सूची देखें।"
    format: 
        
       
back_to_top:
    enable: true
---