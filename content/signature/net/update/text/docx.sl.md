---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Text
fileformat: Docx
productName: .NET
lang: sl
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Docx for C#

############################# Head ############################
head_title: "Posodobite podpise Text v datotekah Docx z C#"
head_description: "Uporabite preprosto in razumljivo kodo .NET za posodobitev podpisov Text v podpisanih dokumentih Docx."

############################# Header ############################
title: "Uredite in posodobite podpise Text v datotekah Docx"
description: "API za .NET zagotavlja funkcionalnost za posodabljanje podpisov Text v dokumentih Docx. Hitro in enostavno posodobite e-podpise v svojih dokumentih Docx z nekaj vrsticami kode C#."
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
    title: "Več o funkcijah API-ja GroupDocs.Signature for .NET"
    content: |
        Funkcionalnost API-ja [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) vsebuje širok izbor sredstev za obdelavo v formatih dokumentov na zahtevo z uporabo elektronskih podpisov. Podprt je širok spekter e-podpisov, kot so besedila, slike, digitalna potrdila, črtne kode, QR-kode, žigi ali metapodatki. Stranke lahko dodajajo, odstranjujejo, urejajo, preverjajo ali iščejo digitalne podpise v PDF-jih, dokumentih MS Word, delovnih zvezkih MS Excel, predstavitvah MS PowerPoint, datotekah Adobe Photoshop in različnih formatih slik. Na voljo so številne uporabne funkcije in nastavitve.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kako spremeniti podpise Text v dokumentu Docx"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) vključuje uporabne funkcije, kot je posodobitev podpisov Text v dokumentih Docx. Omogoča spreminjanje funkcij podpisov brez dodatne kode.
        
        * Za začetek ustvarite predmet podpisa, ki bo kot pot parametra konstruktorja posredoval dokumentu, ki naj bi bil posodobljen.
        * Nato ustvarite primerek ustreznega določenega predmeta podpisa in nastavite njegov identifikator in lastnosti, ki jih je treba spremeniti.
        * Na koncu pokličite metodo posodobitve podpisa, ki posreduje določen predmet podpisa.
        * Postopek posodabljanja rezultatov na vaše obvestilo.

    title_right: "Sistemske zahteve"
    content_right: |
        GroupDocs.Signature for .NET so podprti na vseh glavnih platformah in operacijskih sistemih. Preden izvedete spodnjo kodo, se prepričajte, da imate v sistemu nameščene naslednje predpogoje.

        * Operacijski sistemi: Microsoft Windows, Linux, MacOS
        * Razvojna okolja: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Prenesite najnovejšo različico GroupDocs.Signature for .NET iz [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Docx file
        string filePath = "input.docx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to update
                // set up particular signature id
                TextSignature signatureToUpdate = new TextSignature(id)
                {
                    // specify signature width
                    Width = 130,
                    // specify signature height
                    Height = 20,
                    // set left position
                    Left = 40,
                    // set top position
                    Top = 50,
                    // set up new text
                    Text = "Mr. John Smith"
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
    title: "Posodabljanje podpisov Text na straneh dokumenta – predstavitev v živo"
    content: |
       Takoj zdaj uredite različne elektronske podpise dokumenta Docx tako, da obiščete spletno mesto [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Posodobite različne podpise Text prek C#"
    content: |
        "Urejanje digitalnih podpisov, ki se nahajajo v različnih formatih dokumentov. Posodobite podatke o podpisih brez dodatne kode."
    format: 
       
       
back_to_top:
    enable: true
---