---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Xlsm
productName: .NET
lang: et
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xlsm for C#

############################# Head ############################
head_title: "Digitaalsete elektrooniliste allkirjade lisamine failile Xlsm rakendusega C#"
head_description: "Sisestage digitaalallkiri toote .NET failile Xlsm, kasutades mõnda koodirida. Kasutage GroupDocs Document Signature API-t kümnete failivormingute allkirjastamiseks."

############################# Header ############################
title: "eSign Xlsm failid Digital allkirjaga rakenduses C#"
description: "Kuidas lisada allkirja Digital mõne reaga .NET koodiga"
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
    title: "Teave GroupDocs.Signature for .NET digitaalallkirjade API kohta"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) on populaarne API dokumentide allkirjastamiseks digitaalsete elektrooniliste allkirjadega ja digitaalsete sertifikaatidega. Digitaalallkirjade jaoks kasutab API parooliga kaitstud privaatsete ja avalike võtmetega dokumendi allkirjastamiseks PFX-sertifikaadi faile. Digitaalallkirju võib kasutada äridokumentide sertifitseerimiseks eSign PDF-i konkreetse lehe abil, tervete Microsoft Office'i dokumentide, näiteks Wordsi, Exceli, Powerpointi failide ja Open Office'i dokumentide sertifitseerimiseks. Kliendid saavad allkirjadega hõlpsalt manipuleerida, näiteks neid redigeerida, eemaldada või kohandada. API pakub võimalust allkirjade otsimiseks ja kinnitamiseks. Lisaks pakutakse palju allkirjade kohandamise võimalusi.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Toimingud Xlsm allkirjastamiseks rakendusega Digital rakenduses C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) võimaldab kiiresti ja lihtsalt allkirjastada Xlsm dokumente Digital allkirjaga.
        
        * Looge allkirjaklassi eksemplar, mis sisaldab faili Xlsm, mis peaks allkirjastama tee või mäluvoona
        * Käivitage klass SignOptions ja määrake kõik nõutavad andmed.
        * Käivitage meetod Signature.Sign(), mis edastab väljundfaili Xlsm või mäluvoo

    title_right: " Nõuded süsteemile"
    content_right: |
        Toodet GroupDocs.Signature for .NET toetavad kõik suuremad platvormid ja operatsioonisüsteemid. Enne alloleva koodi käivitamist veenduge, et teie süsteemi on installitud järgmised eeltingimused.

        * Operatsioonisüsteemid: Microsoft Windows, Linux, MacOS
        * Arenduskeskkonnad: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Hankige uusim GroupDocs.Signature for .NET kasutajalt [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xlsm file
        string filePath = "input.xlsm";
        // Set up output file
        string outputFilePath = "output.xlsm";
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

                // sign Xlsm document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dokumentide Xlsm allkirjastamine Digital reaalajas demoga"
    content: |
       Allkirjastage fail Xlsm erinevate allkirjadega kohe, külastades veebisaiti [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Tasuta online demo ootab teid.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Muud toetatud Digital allkirjad C# jaoks"
    content: |
        "Saate allkirjastada faili Xlsm ka muude allkirjatüüpidega. Vaadake allolevat loendit."
    format: 
       
       
back_to_top:
    enable: true
---