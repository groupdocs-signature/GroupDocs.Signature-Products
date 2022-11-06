---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Metadata
fileformat: Bmp
productName: .NET
lang: hi
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Metadata signatures at Bmp with C#

############################# Head ############################
head_title: "C# में Bmp फ़ाइल में Metadata हस्ताक्षर खोजें"
head_description: "कोड की कुछ पंक्तियों का उपयोग करके Bmp फ़ाइलों में Metadata हस्ताक्षर खोजने के लिए .NET का उपयोग करें।"

############################# Header ############################
title: "Metadata हस्ताक्षर के लिए Bmp फ़ाइल में खोजें"
description: ".NET नेटिव API पहले से हस्ताक्षरित Bmp फाइलों में Metadata हस्ताक्षर खोजने की अनुमति देता है। कोड की कुछ पंक्तियों का उपयोग करके अपने Bmp दस्तावेज़ों में उन्नत ई-हस्ताक्षर खोज करें।"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for .NET API के बारे में"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) विभिन्न प्रकार के हस्ताक्षर जैसे टेक्स्ट, इमेज, डिजिटल सर्टिफिकेट, बारकोड, क्यूआर-कोड, स्टैम्प या मेटाडेटा का उपयोग करके दस्तावेजों को संसाधित करने के लिए .NET एपीआई प्रदान करता है। उपयोगकर्ता आवश्यकतानुसार हस्ताक्षर गुणों को अनुकूलित करने के लिए अतिरिक्त समर्थन के साथ पीडीएफ, एमएस वर्ड दस्तावेज़, एमएस एक्सेल कार्यपुस्तिका, एमएस पावरपॉइंट प्रस्तुतियों, एडोब फोटोशॉप फाइलों और विभिन्न छवि प्रारूपों के भीतर इलेक्ट्रॉनिक हस्ताक्षर जोड़, हटा, अद्यतन, सत्यापित या खोज सकते हैं।
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Metadata हस्ताक्षर को Bmp में कैसे खोजें"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) कुछ आसान चरणों को लागू करके .NET डेवलपर्स के लिए Metadata हस्ताक्षर को Bmp फाइलों में खोजना आसान बनाता है।
        
        * सिग्नेचर क्लास का एक नया इंस्टेंस बनाएं और सोर्स डॉक्यूमेंट पाथ को कंस्ट्रक्टर पैरामीटर के रूप में पास करें।
        * अपनी आवश्यकताओं के अनुसार SearchOptions ऑब्जेक्ट को इंस्टेंट करें और खोज विकल्प निर्दिष्ट करें।
        * सिग्नेचर क्लास इंस्टेंस की सर्च मेथड को कॉल करें और इसमें सर्चऑप्शन पास करें।
        * अपनी मांगों के अनुसार खोज परिणामों की प्रक्रिया करें।

    title_right: "सिस्टम आवश्यकताएं"
    content_right: |
        GroupDocs.Signature for .NET सभी प्रमुख प्लेटफॉर्म और ऑपरेटिंग सिस्टम पर समर्थित हैं। नीचे दिए गए कोड को निष्पादित करने से पहले, कृपया सुनिश्चित करें कि आपके सिस्टम पर निम्नलिखित पूर्वापेक्षाएँ स्थापित हैं।

        * ऑपरेटिंग सिस्टम: माइक्रोसॉफ्ट विंडोज, लिनक्स, मैकओएस
        * विकास परिवेश: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature) से GroupDocs.Signature for .NET का नवीनतम संस्करण डाउनलोड करें
         
    code: |
        ```csharp    
        
        // Set up input Bmp file
        string filePath = "input.bmp";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // search for Metadata signatures in Bmp document
                List<ImageMetadataSignature> signatures = signature.Search<ImageMetadataSignature>(SignatureType.Metadata);

                // process signatures which were found 
                foreach (ImageMetadataSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Metadata इलेक्ट्रॉनिक हस्ताक्षर के लिए खोजें लाइव डेमो"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) वेबसाइट पर जाकर Bmp फाइलों में विभिन्न इलेक्ट्रॉनिक हस्ताक्षरों के लिए दस्तावेज़ खोजें।

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "C# का उपयोग करके अन्य Metadata हस्ताक्षर खोजें"
    content: |
        "इलेक्ट्रॉनिक हस्ताक्षर विभिन्न दस्तावेजों में खोज करते हैं। नीचे दिखाए गए अनुसार लोकप्रिय फ़ाइल स्वरूपों में से एक से हस्ताक्षर प्राप्त करें।"
    format: 
           
       
back_to_top:
    enable: true
---