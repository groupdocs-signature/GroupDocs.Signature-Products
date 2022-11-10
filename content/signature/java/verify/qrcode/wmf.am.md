---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Wmf
productName: Java
lang: am
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Wmf for Java

############################# Head ############################
head_title: "የQrcode ፊርማዎች ለWmf ፋይሎች በJava በኩል ማረጋገጫ"
head_description: "Wmf ሰነዶችን እና Qrcode ፊርማቸውን ለማረጋገጥ ጥቂት የJava ኮድ መስመሮችን ብቻ ይጠቀሙ።"

############################# Header ############################
title: "ለWmf ፋይሎች የQrcode ፊርማ ማረጋገጫ"
description: "ኤፒአይ ለJava የQrcode ፊርማዎችን በWmf ሰነዶች ለማረጋገጥ እድል ይሰጣል። በእርስዎ Wmf ሰነዶች ውስጥ ያሉ የኢ-ፊርማዎች ማረጋገጫ በፍጥነት እና በቀላሉ ሊከናወን ይችላል።"
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
    title: "አዲስ የGroupDocs.Signature for Java API ባህሪያትን ያግኙ"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ኤፒአይ የኤሌክትሮኒክ ፊርማዎችን በመጠቀም ብዙ የሰነድ ቅርጸቶችን ለማስኬድ ሰፊ መንገዶችን ይሰጣል። ብዙ አይነት ዲጂታል ፊርማዎች እንደ ጽሑፎች፣ ምስሎች፣ ዲጂታል ሰርተፊኬቶች፣ ባርኮዶች፣ QR-codes፣ ማህተሞች ወይም ሜታዳታ ይደገፋሉ። ደንበኞች ዲጂታል ፊርማዎችን በፒዲኤፍ፣ MS Word ሰነዶች፣ በኤምኤስ ኤክሴል የስራ ደብተሮች፣ MS PowerPoint ማቅረቢያዎች፣ አዶቤ ፎቶሾፕ ፋይሎች እና የተለያዩ የምስል ቅርጸቶችን ማከል፣ ማስወገድ፣ ማረም፣ ማረጋገጥ ወይም መፈለግ ይችላሉ። የሚገርሙ የተጨማሪ ባህሪያት እና ቅንብሮች ይገኛሉ።
    

############################# Steps ############################
steps:
    enable: true
    title_left: "በእርስዎ Wmf ሰነድ ውስጥ የQrcode ፊርማዎችን እንዴት ማረጋገጥ እንደሚቻል"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) በWmf ሰነዶች ላይ የተቀመጡ የQrcode ፊርማዎችን ማረጋገጥ ያሉ ጠቃሚ ባህሪያትን ያካትታል። ተጨማሪ ኮድ ሳይተገብሩ ይህንን እድል ይጠቀሙ።
        
        * በመጀመሪያ፣ የፈጣን ፊርማ ክፍል መረጋገጥ አለበት ወደተባለው ሰነድ እንደ ግንበኛ መለኪያ መንገድ ያቀርባል።
        * በሁለተኛ ደረጃ አዲስ የVerifyOptions ነገር ይፍጠሩ እና ሁሉንም አስፈላጊ ንብረቶች ያዘጋጁ።
        * በመጨረሻም፣ የፊርማ ነገርን ጥራ የVerifyOptions ምሳሌን የሚያልፍበትን ዘዴ ያረጋግጡ።
        * ከዚያ የማረጋገጫ ውጤቶችን ያስኬዱ.

    title_right: "የስርዓት መስፈርቶች"
    content_right: |
        GroupDocs.Signature for Java በሁሉም ዋና መድረኮች እና ስርዓተ ክወናዎች ላይ ይደገፋሉ። ከዚህ በታች ያለውን ኮድ ከመተግበሩ በፊት፣ እባክዎ በስርዓትዎ ላይ የሚከተሉት ቅድመ ሁኔታዎች እንዳሉዎት ያረጋግጡ።

        * ስርዓተ ክወናዎች-ማይክሮሶፍት ዊንዶውስ ፣ ሊኑክስ ፣ ማክኦኤስ
        * የልማት አካባቢዎች፡ NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * የቅርብ ጊዜውን የGroupDocs.Signature for Java ስሪት ከ[Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) ያውርዱ
         
    code: |
        ```java    
                
        // Set up input Wmf file
        String filePath = "input.wmf";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        QrCodeVerifyOptions options = new QrCodeVerifyOptions();

        // process only first page
        options.setPagesSetup(new PagesSetup());
        options.setPageNumber(1);
        options.setAllPages(false);
        // specify text match type
        options.setMatchType(TextMatchType.StartsWith);
        // specify text pattern to search
        options.setText("QrCode text");
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "በQrcode ፊርማዎች ቀጥታ ማሳያ መፈረም"
    content: |
       የ[GroupDocs.signature መተግበሪያ](https://products.groupdocs.app/signature/family) ድህረ ገጽን በመጎብኘት የተለያዩ ኤሌክትሮኒክ ፊርማዎችን ወደ Wmf ፋይል አሁኑኑ ያክሉ።          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Javaን በመጠቀም ሌሎች የQrcode ፊርማዎችን ያረጋግጡ"
    content: |
        "በተለያዩ ሰነዶች ውስጥ የተቀመጡ የኤሌክትሮኒክ ፊርማዎችን ማረጋገጥ. ከታች እንደተገለጸው የፊርማዎችን ጥራት በታዋቂው የፋይል ቅርጸቶች ያረጋግጡ።"
    format: 
       
       
back_to_top:
    enable: true
---