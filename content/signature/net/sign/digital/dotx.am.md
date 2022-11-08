---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Dotx
productName: .NET
lang: am
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Dotx for C#

############################# Head ############################
head_title: "ዲጂታል ኤሌክትሮኒክ ፊርማዎችን ወደ Dotx ፋይል በC# ማከል"
head_description: "ጥቂት የኮድ መስመሮችን በመጠቀም በDotx ፋይል ላይ ለ.NET ዲጂታል ፊርማ ያድርጉ። በደርዘን የሚቆጠሩ የፋይል ቅርጸቶችን ለመፈረም የGroupDocs Document Signature API ይጠቀሙ።"

############################# Header ############################
title: "eSign Dotx ፋይሎች በDigital ፊርማዎች በC#"
description: "የDigital ፊርማ ከጥቂት መስመሮች .NET ኮድ ጋር እንዴት እንደሚታከል"
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
    title: "ስለ GroupDocs.Signature for .NET ዲጂታል ፊርማዎች ኤፒአይ"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ሰነዶችን ከዲጂታል ኤሌክትሮኒክ ፊርማዎች፣ ከዲጂታል የምስክር ወረቀቶች ጋር ለመፈረም ታዋቂ ኤፒአይ ነው። ለዲጂታል ፊርማዎች ኤፒአይ የPFX የምስክር ወረቀት ፋይሎችን በይለፍ ቃል የተጠበቁ የግል እና የህዝብ ቁልፎችን ለመፈረም ይጠቀማል። የዲጂታል ፊርማዎች የንግድ ሰነዶችን በ eSign PDF የተወሰነ ገጽ ለማረጋገጥ፣ እንደ Words፣ Excel፣ Powerpoint ፋይሎች እና የOffice ሰነዶች ያሉ ሙሉ የማይክሮሶፍት ኦፊስ ሰነዶችን ለማረጋገጥ ሊያገለግሉ ይችላሉ። ደንበኞች ፊርማዎችን እንደ ማረም፣ ማስወገድ ወይም ማስተካከል ያሉ በቀላሉ ሊጠቀሙባቸው ይችላሉ። ኤፒአይ ፊርማዎችን ለመፈለግ እና ለማረጋገጥ መንገድ ያቀርባል። ከዚህም በላይ ለፊርማ ማበጀት ብዙ ችሎታዎች ቀርበዋል.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Dotxን በDigital በC# ለመፈረም ደረጃዎች"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) የDotx ሰነዶችን በDigital ፊርማ በፍጥነት እና በቀላሉ የመፈረም ችሎታን ይሰጣል።
        
        * እንደ ዱካ ወይም የማህደረ ትውስታ ዥረት መፈረም ያለበትን Dotx ፋይል የሚያቀርብ የፊርማ ክፍል ምሳሌ ይፍጠሩ
        * ቅጽበታዊ SignOptions ክፍል እና ሁሉንም የተፈለገውን ውሂብ ያዘጋጁ።
        * ውፅዓት Dotx ፋይልን ወይም የማህደረ ትውስታ ዥረቱን የማለፊያ ዘዴ Signature.Sign()ን ጥራ

    title_right: " የስርዓት መስፈርቶች"
    content_right: |
        GroupDocs.Signature for .NET በሁሉም ዋና መድረኮች እና ስርዓተ ክወናዎች ላይ ይደገፋሉ። ከዚህ በታች ያለውን ኮድ ከመተግበሩ በፊት፣ እባክዎ በስርዓትዎ ላይ የሚከተሉት ቅድመ ሁኔታዎች እንዳሉዎት ያረጋግጡ።

        * ስርዓተ ክወናዎች-ማይክሮሶፍት ዊንዶውስ ፣ ሊኑክስ ፣ ማክኦኤስ
        * የልማት አካባቢዎች፡ Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * የቅርብ ጊዜውን GroupDocs.Signature for .NET ከ[Nuget](https://www.nuget.org/packages/groupdocs.signature) ያግኙ
         
    code: |
        ```csharp    
                
        // Set up input Dotx file
        string filePath = "input.dotx";
        // Set up output file
        string outputFilePath = "output.dotx";
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

                // sign Dotx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dotx ሰነዶችን በDigital ቀጥታ ማሳያ በመፈረም ላይ"
    content: |
       የ[GroupDocs.Signature መተግበሪያ](https://products.groupdocs.app/signature/family) ድህረ ገጽን በመጎብኘት የDotx ፋይልን በተለያዩ ፊርማዎች አሁን ይፈርሙ። ነፃ የመስመር ላይ ማሳያ እርስዎን እየጠበቀዎት ነው።          

############################# More Formats ############################
more_formats:
    enable: true
    title: "ሌሎች የሚደገፉ የDigital ፊርማዎች ለC#"
    content: |
        "እንዲሁም Dotxን ከሌሎች የፊርማ አይነቶች ጋር መፈረም ትችላለህ። እባክዎን ከዚህ በታች ያለውን ዝርዝር ይመልከቱ።"
    format: 
       
       
back_to_top:
    enable: true
---