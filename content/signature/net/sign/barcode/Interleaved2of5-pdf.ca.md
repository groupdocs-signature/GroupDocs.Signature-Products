---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Interleaved2of5
fileformat: Pdf
productName: .NET
lang: ca
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Pdf for C#

############################# Head ############################
head_title: "Document electrònic Pdf amb codi de barres Interleaved2of5 a C#"
head_description: "Creeu la signatura de codi de barres Interleaved2of5 i poseu-la al document Pdf amb .NET utilitzant un parell de línies de codi. Utilitzeu l'API de signatura de documents de GroupDocs per signar diversos formats de fitxer."

############################# Header ############################
title: "Genereu Interleaved2of5 signatura de codi de barres per al document Pdf a C#"
description: "eSigne els vostres documents comercials de Pdf amb el codi de barres Interleaved2of5. Genereu la signatura de codi de barres de manera ràpida i senzilla amb unes poques línies de codi per configurar les opcions de signatura."
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
    title: "Sobre l'API de signatures de codi de barres de GroupDocs.Signature for .NET."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) és una API ràpida i senzilla per gestionar la signatura electrònica de documents digitals mitjançant tipus de codi de barres com UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 i molts altres. Els clients poden crear fàcilment codis de barres que proporcionen el text necessari i posar-los en PDF, documents de Microsoft Office Words, llibres de treball de Microsoft Office Excel, presentacions de MS PowerPoint, fitxers Adobe Photoshop i diversos formats d'imatge. Els codis de barres col·locats als documents es poden actualitzar, cercar, verificar, suprimir o visualitzar prèviament. A més, s'admet la personalització de codis de barres.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Passos per signar Pdf amb Barcode a C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ofereix la possibilitat de signar documents Pdf amb signatures Barcode de manera ràpida i senzilla.
        
        * Creeu una instància de la classe Signature que proporcioni el fitxer Pdf que s'ha de signar com a camí o flux de memòria
        * Instancieu la classe SignOptions i configureu totes les dades sol·licitades.
        * Invoqueu el mètode Signature.Sign() passant el fitxer de sortida Pdf o el flux de memòria

    title_right: " Requisits del sistema"
    content_right: |
        GroupDocs.Signature for .NET són compatibles amb totes les plataformes i sistemes operatius principals. Abans d'executar el codi següent, assegureu-vos que teniu els següents requisits previs instal·lats al vostre sistema.

        * Sistemes operatius: Microsoft Windows, Linux, MacOS
        * Entorns de desenvolupament: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Obteniu l'últim GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Pdf file
        string filePath = "input.pdf";
        // Set up output file
        string outputFilePath = "output.pdf";

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
                
                // sign Pdf document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signant documents de Pdf amb Barcode Demostració en directe"
    content: |
       Signa el fitxer Pdf amb diverses signatures ara mateix visitant el lloc web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demostració gratuïta en línia esperant-te.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Interleaved2of5 Barcode"
          content: |
            Interleaved 2 of 5 (ITF) és una simbologia de codi de barres contínua de dues amplades que codifica els dígits. S'utilitza comercialment en pel·lícules 135, per a codis de barres ITF-14 i en cartrons d'alguns productes, mentre que els productes a l'interior estan etiquetats amb UPC o EAN.
          characterset: |
             Dígits numèrics (0-9).
          textcapacity: |
             Longitud variable.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAB8AAACGCAYAAAAlx1GyAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAFdSURBVHhe7Y0xCkJRAMPe/S/9BSFLqHaSN9hAhyzNeS6y+BUWv8LX+DnnPfjkHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3X+K9Z/Ar/Gn+eF5E2tt5Q4JATAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Altres signatures admeses de Barcode per a C#"
    content: |
        "També podeu signar Pdf amb altres tipus de signatura. Si us plau, consulteu la llista a continuació."
    format: 
        
       
back_to_top:
    enable: true
---