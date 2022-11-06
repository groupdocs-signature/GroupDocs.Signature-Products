---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Barcode
fileformat: Pdf
productName: .NET
lang: hi
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Barcode signature on Pdf for C#

############################# Head ############################
head_title: "Barcode Pdf फाइलों पर रखे गए हस्ताक्षरों को C# के साथ अपडेट करें"
head_description: "हस्ताक्षरित Pdf दस्तावेज़ों में Barcode हस्ताक्षर अद्यतन के लिए .NET कोड को समझने के लिए सरल और आसान का उपयोग करें।"

############################# Header ############################
title: "संपादित करें और अपडेट करें Barcode हस्ताक्षर Pdf फाइलों पर रखे गए हैं"
description: ".NET के लिए API Barcode हस्ताक्षरों को Pdf दस्तावेज़ों में अपडेट करने की कार्यक्षमता प्रदान करता है। C# कोड की दो पंक्तियों के साथ अपने Pdf दस्तावेज़ों के अंदर ई-हस्ताक्षर जल्दी और आसानी से अपडेट करें।"
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
    title: "GroupDocs.Signature for .NET API सुविधाओं के बारे में जानें"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API कार्यक्षमता में इलेक्ट्रॉनिक हस्ताक्षरों का उपयोग करके मांग दस्तावेज़ स्वरूपों में संसाधित करने के लिए साधनों का विशाल चयन शामिल है। टेक्स्ट, इमेज, डिजिटल सर्टिफिकेट, बारकोड, क्यूआर-कोड, स्टैम्प या मेटाडेटा जैसे ई-हस्ताक्षर के व्यापक स्पेक्ट्रम समर्थित हैं। ग्राहक PDF, MS Word दस्तावेज़, MS Excel कार्यपुस्तिका, MS PowerPoint प्रस्तुतियों, Adobe Photoshop फ़ाइलों और विभिन्न छवि प्रारूपों में डिजिटल हस्ताक्षर जोड़, हटा, संपादित, मान्य या खोज सकते हैं। कई उपयोगी सुविधाएँ और सेटिंग्स उपलब्ध हैं।
    

############################# Steps ############################
steps:
    enable: true
    title_left: "अपने Pdf दस्तावेज़ में Barcode हस्ताक्षर कैसे बदलें"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) में Barcode दस्तावेज़ों पर रखे गए Barcode हस्ताक्षरों को अपडेट करने जैसी उपयोगी सुविधाएं शामिल हैं। अतिरिक्त कोड के बिना हस्ताक्षर सुविधाओं को बदलना संभव बनाता है।
        
        * आरंभ करने के लिए, एक दस्तावेज़ के लिए एक कंस्ट्रक्टर पैरामीटर पथ के रूप में पासिंग सिग्नेचर ऑब्जेक्ट बनाएं जिसे अपडेट किया जाना चाहिए।
        * फिर, एक उपयुक्त विशेष हस्ताक्षर वस्तु को तुरंत चालू करें और इसके पहचानकर्ता और गुणों को सेट करें जिन्हें बदलने की आवश्यकता है।
        * अंत में, सिग्नेचर की अपडेट विधि को विशेष सिग्नेचर ऑब्जेक्ट पास करते हुए कॉल करें।
        * अपने नोटिस में परिणाम अपडेट करने की प्रक्रिया करें।

    title_right: "सिस्टम आवश्यकताएं"
    content_right: |
        GroupDocs.Signature for .NET सभी प्रमुख प्लेटफॉर्म और ऑपरेटिंग सिस्टम पर समर्थित हैं। नीचे दिए गए कोड को निष्पादित करने से पहले, कृपया सुनिश्चित करें कि आपके सिस्टम पर निम्नलिखित पूर्वापेक्षाएँ स्थापित हैं।

        * ऑपरेटिंग सिस्टम: माइक्रोसॉफ्ट विंडोज, लिनक्स, मैकओएस
        * विकास परिवेश: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature) से GroupDocs.Signature for .NET का नवीनतम संस्करण डाउनलोड करें
         
    code: |
        ```csharp    
                
        // Set up input Pdf file
        string filePath = "input.pdf";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "07f83369-318b-41ad-a843-732417b912c2";

                // provide signature features to update
                // set up particular signature id
                BarcodeSignature signatureToUpdate = new BarcodeSignature(id)
                {
                    // specify signature width
                    Width = 300,
                    // specify signature height
                    Height = 50,
                    // set left position
                    Left = 80,
                    // set top position
                    Top = 100
                };

                // update signature
                bool updateResult = signature.Update(signatureToUpdate);

                // process updation result
                if (updateResult)
                {
                    Console.WriteLine("Signature was updated successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "दस्तावेज़ पृष्ठों पर Barcode हस्ताक्षर अपडेट करना - लाइव डेमो"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) वेबसाइट पर जाकर Pdf दस्तावेज़ के विभिन्न इलेक्ट्रॉनिक हस्ताक्षरों को अभी संपादित करें।          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# के माध्यम से विभिन्न Barcode हस्ताक्षर अपडेट करें"
    content: |
        "विभिन्न दस्तावेज़ स्वरूपों में रखे गए डिजिटल हस्ताक्षरों का संपादन। अतिरिक्त कोड के बिना हस्ताक्षर डेटा अपडेट करें।"
    format: 
       
       
back_to_top:
    enable: true
---