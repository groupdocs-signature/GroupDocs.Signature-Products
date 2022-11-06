---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Ots
productName: Java
lang: am
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Ots with Java

############################# Head ############################
head_title: "በJava ውስጥ በOts ፋይል ውስጥ የ{{Signturetype}} ፊርማዎችን ይፈልጉ"
head_description: "ጥቂት የኮድ መስመሮችን በመጠቀም በOts ፋይሎች ውስጥ የImage ፊርማዎችን ለመፈለግ Javaን ይጠቀሙ።"

############################# Header ############################
title: "በOts ፋይል ውስጥ የ{{Signturetype}} ፊርማዎችን ይፈልጉ"
description: "Java ቤተኛ ኤፒአይ አስቀድሞ በተፈረሙ Ots ፋይሎች ውስጥ የImage ፊርማዎችን ለመፈለግ ይፈቅዳል። ጥቂት የኮድ መስመሮችን በመጠቀም በOts ሰነዶችዎ ውስጥ የላቀ የኢ-ፊርማ ፍለጋን ያድርጉ።"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "ስለ GroupDocs.Signature for Java ኤፒአይ"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) እንደ ጽሁፎች፣ ምስሎች፣ ዲጂታል ሰርተፊኬቶች፣ ባርኮዶች፣ QR-ኮዶች፣ ማህተሞች ወይም ሜታዳታ ያሉ የተለያዩ የፊርማ አይነቶችን በመጠቀም ሰነዶችን ለመስራት Java ኤፒአይን ያቀርባል። ተጠቃሚዎች እንደ አስፈላጊነቱ የፊርማ ንብረቶችን ለማበጀት ተጨማሪ ድጋፍ በፒዲኤፍ፣ MS Word ሰነዶች፣ MS ኤክሴል የስራ ደብተሮች፣ MS PowerPoint አቀራረቦች፣ አዶቤ ፎቶሾፕ ፋይሎች እና የተለያዩ የምስል ቅርጸቶች ውስጥ የኤሌክትሮኒክ ፊርማዎችን ማከል፣ መሰረዝ፣ ማዘመን፣ ማረጋገጥ ወይም መፈለግ ይችላሉ።
    

############################# Steps ############################
steps:
    enable: true
    title_left: "በOts ውስጥ የ{{Signturetype}} ፊርማዎችን እንዴት መፈለግ እንደሚቻል"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ለJava ገንቢዎች ጥቂት ቀላል ደረጃዎችን በመተግበር በOts ፋይሎች ውስጥ ፊርማዎችን መፈለግ ቀላል ያደርገዋል።
        
        * አዲስ የፊርማ ክፍል ይፍጠሩ እና የምንጭ ሰነድ መንገድን እንደ ግንበኛ መለኪያ ይለፉ።
        * እንደ ፍላጎቶችዎ የፍለጋ አማራጮችን ነገር ያፋጥኑ እና የፍለጋ አማራጮችን ይጥቀሱ።
        * ለፊርማ ክፍል ምሳሌ የፍለጋ ዘዴን ይደውሉ እና የፍለጋ አማራጮችን ወደ እሱ ያስተላልፉ።
        * በጥያቄዎችዎ መሰረት የፍለጋ ውጤቶችን ያስኬዱ።

    title_right: "የስርዓት መስፈርቶች"
    content_right: |
        GroupDocs.Signature for Java በሁሉም ዋና መድረኮች እና ስርዓተ ክወናዎች ላይ ይደገፋሉ። ከዚህ በታች ያለውን ኮድ ከመተግበሩ በፊት፣ እባክዎ በስርዓትዎ ላይ የሚከተሉት ቅድመ ሁኔታዎች እንዳሉዎት ያረጋግጡ።

        * ስርዓተ ክወናዎች-ማይክሮሶፍት ዊንዶውስ ፣ ሊኑክስ ፣ ማክኦኤስ
        * የልማት አካባቢዎች፡ NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * የቅርብ ጊዜውን የGroupDocs.Signature for Java ስሪት ከ[Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) ያውርዱ
         
    code: |
        ```java    
                
        // Set up input Ots file
        String filePath = "input.ots";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        ImageSearchOptions options = new ImageSearchOptions();

        // set minimum size if needed 
        options.setMinContentSize(100);
        // set maximum image size if needed
        options.setMaxContentSize(2000);
        // return images for processing
        options.setReturnContent(true);
        // set up type of returned images
        options.setReturnContentType(FileType.PNG);

        // search for Image signatures in Ots document
        List<ImageSignature> signatures = signature.search(ImageSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "የ{{Signturetype}} ኤሌክትሮኒክ ፊርማዎችን የቀጥታ ማሳያን ይፈልጉ"
    content: |
       የ[GroupDocs.signature መተግበሪያ](https://products.groupdocs.app/signature/family) ድህረ ገጽን በመጎብኘት ሰነዱን አሁን በOts ፋይሎች ላይ የተለያዩ የኤሌክትሮኒክ ፊርማዎችን ይፈልጉ።

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Javaን በመጠቀም ሌሎች {{የፊርማ አይነት}} ፊርማዎችን ይፈልጉ"
    content: |
        "የኤሌክትሮኒክ ፊርማዎች በተለያዩ ሰነዶች ውስጥ ይፈልጉ. ከታች እንደሚታየው ከታዋቂው የፋይል ቅርጸቶች ፊርማዎችን ያግኙ።"
    format: 
           
       
back_to_top:
    enable: true
---