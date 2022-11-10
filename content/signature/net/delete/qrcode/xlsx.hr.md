---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Xlsx
productName: .NET
lang: hr
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Xlsx for C#

############################# Head ############################
head_title: "Izbriši Qrcode potpise iz Xlsx datoteka putem C#"
head_description: "Brisanje specifičnih Qrcode potpisa iz potpisanih Xlsx dokumenata može se lako izvesti s kratkim .NET kodom."

############################# Header ############################
title: "Uklonite potpise Qrcode koji se nalaze u datotekama Xlsx"
description: "Izbrišite razne Qrcode potpise iz Xlsx dokumenata. Uklanjanje Qrcode potpisa zahtijeva jednostavan C# kod."
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
    title: "Dobijte informacije o GroupDocs.Signature for .NET API značajkama"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API pruža mnogo načina za obradu vaših dokumenata korištenjem elektroničkih potpisa. Dostupni su digitalni potpisi kao što su tekstovi, slike, digitalni certifikati, crtični kodovi, QR kodovi, pečati ili metapodaci. Korisnici imaju mogućnost dodavanja, brisanja, ažuriranja, provjere ili pretraživanja digitalnih potpisa u PDF-ovima, MS Word dokumentima, MS Excel radnim knjigama, MS PowerPoint prezentacijama, Adobe Photoshop datotekama i raznim formatima slika. Omogućen je velik broj korisnih značajki i postavki.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kako ukloniti Qrcode potpise iz vašeg Xlsx dokumenta"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) pruža korisnu značajku za brisanje Xlsx dokumenata od Qrcode potpisa s nekoliko redaka koda.
        
        * Prvo, instancirajte putanju prolaza objekta Signature do vašeg dokumenta kao parametar konstruktora.
        * Zatim stvorite odgovarajući objekt potpisa i postavite njegov jedinstveni identifikator.
        * Nakon toga pozovite metodu Delete prosljeđujući objekt potpisa koji se mora izbrisati.
        * Na kraju, obradite rezultate operacije.

    title_right: "Zahtjevi sustava"
    content_right: |
        GroupDocs.Signature for .NET podržani su na svim glavnim platformama i operativnim sustavima. Prije izvršavanja koda u nastavku, provjerite imate li sljedeće preduvjete instalirane na vašem sustavu.

        * Operativni sustavi: Microsoft Windows, Linux, MacOS
        * Razvojna okruženja: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Preuzmite najnoviju verziju GroupDocs.Signature for .NET s [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xlsx file
        string filePath = "input.xlsx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

                // provide signature features to delete
                // set up particular signature id
                QrCodeSignature signatureToDelete = new QrCodeSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Potpisivanje s Qrcode potpisima Demo uživo"
    content: |
       Odmah dodajte različite elektroničke potpise u datoteku Xlsx tako da posjetite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web mjesto.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Izbrišite svoje Qrcode potpise s C#"
    content: |
        "Brisanje e-potpisa koji su dodani različitim formatima dokumenata. Brzo uklonite potpise bez dodatnog koda."
    format: 
       
       
back_to_top:
    enable: true
---