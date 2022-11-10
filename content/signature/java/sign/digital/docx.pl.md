---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Docx
productName: Java
lang: pl
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Docx for Java

############################# Head ############################
head_title: "Dodawanie podpisów elektronicznych do pliku Docx za pomocą Java"
head_description: "Umieść podpis cyfrowy w pliku Docx dla Java, używając kilku linijek kodu. Użyj interfejsu GroupDocs Document Signature API, aby podpisać dziesiątki formatów plików."

############################# Header ############################
title: "eSign Docx pliki z podpisami Digital w Java"
description: "Jak dodać podpis Digital za pomocą kilku linijek kodu Java?"
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
    title: "O GroupDocs.Signature for Java API podpisów cyfrowych"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) to popularny interfejs API do podpisywania dokumentów z cyfrowymi podpisami elektronicznymi i certyfikatami cyfrowymi. W przypadku podpisów cyfrowych API wykorzystuje pliki certyfikatów PFX do opisywania dokumentów za pomocą chronionych hasłem kluczy prywatnych i publicznych. Podpisy cyfrowe mogą być używane do poświadczania dokumentów biznesowych za pomocą określonej strony eSign PDF, poświadczania całych dokumentów Microsoft Office, takich jak Words, Excel, pliki Powerpoint i dokumenty Open Office. Klienci mogą łatwo manipulować podpisami, np. edytować je, usuwać lub dostosowywać. API umożliwia wyszukiwanie i weryfikację podpisów. Ponadto zapewniono wiele możliwości dostosowywania podpisów.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroki do podpisania Docx za pomocą Digital w Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) umożliwia szybkie i łatwe podpisywanie dokumentów w formacie Docx za pomocą podpisów Digital.
        
        * Utwórz instancję klasy Signature podając plik Docx do podpisania jako ścieżkę lub strumień pamięci
        * Utwórz wystąpienie klasy SignOptions i ustaw wszystkie wymagane dane.
        * Wywołaj metodę Signature.Sign() przekazującą wyjściowy plik Docx lub strumień pamięci

    title_right: " wymagania systemowe"
    content_right: |
        GroupDocs.Signature for Java są obsługiwane na wszystkich głównych platformach i systemach operacyjnych. Przed wykonaniem poniższego kodu upewnij się, że masz zainstalowane w systemie następujące wymagania wstępne.

        * Systemy operacyjne: Microsoft Windows, Linux, MacOS
        * Środowiska programistyczne: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Pobierz najnowszą wersję GroupDocs.Signature for Java z [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Docx file
        String filePath = "input.docx";
        // Set up output file
        String outputFilePath = "output.docx";
        // Provide digital certificate
        String certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        DigitalSignOptions options = new DigitalSignOptions(certificateFilePath);

        // set certificate password
        options.setPassword("1234567890");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Docx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisywanie dokumentów Docx za pomocą Digital Demo na żywo"
    content: |
       Podpisz teraz plik Docx różnymi podpisami, odwiedzając witrynę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Darmowe demo online czeka na Ciebie.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Inne obsługiwane podpisy Digital dla Java"
    content: |
        "Możesz także podpisać Docx innymi typami podpisów. Zobacz poniższą listę."
    format: 
       
       
back_to_top:
    enable: true
---