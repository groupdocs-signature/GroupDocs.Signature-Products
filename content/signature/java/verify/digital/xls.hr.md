---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Xls
productName: Java
lang: hr
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xls for Java

############################# Head ############################
head_title: "Provjera Digital potpisa za Xls datoteke putem Java"
head_description: "Upotrijebite samo nekoliko redaka Java koda za provjeru Xls dokumenata i njihovih Digital potpisa."

############################# Header ############################
title: "Provjera potpisa Digital za Xls datoteke"
description: "API za Java pruža priliku za provjeru potpisa Digital u dokumentima Xls. Provjera e-potpisa unutar vaših Xls dokumenata može se izvršiti brzo i jednostavno."
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
    title: "Otkrijte nove GroupDocs.Signature for Java API značajke"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API pruža širok raspon načina za obradu brojnih formata dokumenata korištenjem elektroničkih potpisa. Podržane su mnoge vrste digitalnih potpisa kao što su tekstovi, slike, digitalni certifikati, crtični kodovi, QR kodovi, pečati ili metapodaci. Korisnici mogu dodavati, uklanjati, uređivati, potvrđivati ​​ili pretraživati ​​digitalne potpise u PDF-ovima, MS Word dokumentima, MS Excel radnim knjigama, MS PowerPoint prezentacijama, Adobe Photoshop datotekama i raznim formatima slika. Dostupan je nevjerojatan broj dodatnih značajki i postavki.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kako provjeriti valjanost potpisa Digital u vašem Xls dokumentu"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) uključuje korisne značajke kao što je provjera potpisa Digital postavljenih na dokumente Xls. Iskoristite ovu priliku bez implementacije dodatnog koda.
        
        * Prvo, instancirajte klasu potpisa koja kao parametar konstruktora daje put do dokumenta koji bi trebao biti verificiran.
        * Drugo, stvorite novi objekt VerifyOptions i postavite sva potrebna svojstva.
        * Na kraju, pozovite metodu Verify objekta Signature prolazeći instancu VerifyOptions.
        * Zatim obradite rezultate provjere.

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

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        DigitalVerifyOptions options = new DigitalVerifyOptions();

        // Digital signature comment
        options.setComments("Approved");

        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2020, 12, 12));
        options.setSignDateTimeTo(new Date(2022, 12, 12));
                            
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
    title: "Potpisivanje s Digital potpisima Demo uživo"
    content: |
       Odmah dodajte različite elektroničke potpise u datoteku Xls tako da posjetite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web mjesto.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Provjerite druge Digital potpise koristeći Java"
    content: |
        "Provjera elektroničkih potpisa postavljenih u različite dokumente. Provjerite kvalitetu potpisa u popularnim formatima datoteka kao što je otkriveno u nastavku."
    format: 
       
       
back_to_top:
    enable: true
---