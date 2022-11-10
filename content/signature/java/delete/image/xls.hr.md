---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Image
fileformat: Xls
productName: Java
lang: hr
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Xls for Java

############################# Head ############################
head_title: "Izbriši Image potpise iz Xls datoteka putem Java"
head_description: "Brisanje specifičnih Image potpisa iz potpisanih Xls dokumenata može se lako izvesti s kratkim Java kodom."

############################# Header ############################
title: "Uklonite potpise Image koji se nalaze u datotekama Xls"
description: "Izbrišite razne Image potpise iz Xls dokumenata. Uklanjanje Image potpisa zahtijeva jednostavan Java kod."
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
    title: "Dobijte informacije o GroupDocs.Signature for Java API značajkama"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API pruža mnogo načina za obradu vaših dokumenata korištenjem elektroničkih potpisa. Dostupni su digitalni potpisi kao što su tekstovi, slike, digitalni certifikati, crtični kodovi, QR kodovi, pečati ili metapodaci. Korisnici imaju mogućnost dodavanja, brisanja, ažuriranja, provjere ili pretraživanja digitalnih potpisa u PDF-ovima, MS Word dokumentima, MS Excel radnim knjigama, MS PowerPoint prezentacijama, Adobe Photoshop datotekama i raznim formatima slika. Omogućen je velik broj korisnih značajki i postavki.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kako ukloniti Image potpise iz vašeg Xls dokumenta"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) pruža korisnu značajku za brisanje Xls dokumenata od Image potpisa s nekoliko redaka koda.
        
        * Prvo, instancirajte putanju prolaza objekta Signature do vašeg dokumenta kao parametar konstruktora.
        * Zatim stvorite odgovarajući objekt potpisa i postavite njegov jedinstveni identifikator.
        * Nakon toga pozovite metodu Delete prosljeđujući objekt potpisa koji se mora izbrisati.
        * Na kraju, obradite rezultate operacije.

    title_right: "Zahtjevi sustava"
    content_right: |
        GroupDocs.Signature for Java podržani su na svim glavnim platformama i operativnim sustavima. Prije izvršavanja koda u nastavku, provjerite imate li sljedeće preduvjete instalirane na vašem sustavu.

        * Operativni sustavi: Microsoft Windows, Linux, MacOS
        * Razvojna okruženja: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Preuzmite najnoviju verziju GroupDocs.Signature for Java s [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xls file
        String filePath = "input.xls";
        // Set up output file
        String outputFilePath = "output.xls";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "e3ad0ec7-9abf-426d-b9aa-b3328f3f1470";

        // provide signature features to delete
        ImageSignature signatureToDelete = new ImageSignature(id);

        // delete signature
        Boolean deleteResult = signature.delete(outputFilePath, signatureToDelete);

        // process deletion result
        if (deleteResult)
        {
                System.out.println("Signature was deleted successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Potpisivanje s Image potpisima Demo uživo"
    content: |
       Odmah dodajte različite elektroničke potpise u datoteku Xls tako da posjetite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web mjesto.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Izbrišite svoje Image potpise s Java"
    content: |
        "Brisanje e-potpisa koji su dodani različitim formatima dokumenata. Brzo uklonite potpise bez dodatnog koda."
    format: 
       
       
back_to_top:
    enable: true
---