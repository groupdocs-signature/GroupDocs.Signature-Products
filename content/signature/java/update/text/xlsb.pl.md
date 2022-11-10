---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Text
fileformat: Xlsb
productName: Java
lang: pl
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Xlsb for Java

############################# Head ############################
head_title: "Zaktualizuj podpisy Text umieszczone w plikach Xlsb za pomocą Java"
head_description: "Użyj prostego i łatwego do zrozumienia kodu Java do aktualizacji podpisów Text w podpisanych dokumentach Xlsb."

############################# Header ############################
title: "Edytuj i aktualizuj podpisy Text umieszczone w plikach Xlsb"
description: "Interfejs API dla Java zapewnia funkcjonalność aktualizacji podpisów Text w dokumentach Xlsb. Zaktualizuj podpisy elektroniczne w swoich dokumentach Xlsb za pomocą kilku linijek kodu Java szybko i łatwo."
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
    title: "Dowiedz się więcej o funkcjach interfejsu API GroupDocs.Signature for Java"
    content: |
        Funkcjonalność interfejsu API [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) obejmuje szeroki wybór środków do przetwarzania na żądanie formatów dokumentów przy użyciu podpisów elektronicznych. Obsługiwane jest szerokie spektrum podpisów elektronicznych, takich jak teksty, obrazy, certyfikaty cyfrowe, kody kreskowe, kody QR, pieczątki czy metadane. Klienci mogą dodawać, usuwać, edytować, sprawdzać lub wyszukiwać podpisy cyfrowe w plikach PDF, dokumentach MS Word, skoroszytach MS Excel, prezentacjach MS PowerPoint, plikach Adobe Photoshop i różnych formatach graficznych. Dostępnych jest wiele przydatnych funkcji i ustawień.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Jak zmienić podpisy Text w dokumencie Xlsb?"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) zawiera przydatne funkcje, takie jak aktualizacja podpisów Text umieszczonych w dokumentach Xlsb. Umożliwia zmianę funkcji podpisów bez dodatkowego kodu.
        
        * Na początek utwórz obiekt Signature przekazujący jako ścieżkę parametru konstruktora do dokumentu, który ma zostać zaktualizowany.
        * Następnie utwórz instancję odpowiedniego konkretnego obiektu podpisu i ustaw jego identyfikator oraz właściwości, które należy zmienić.
        * Na koniec wywołaj metodę Update Signature, przekazując konkretny obiekt podpisu.
        * Przeprowadź aktualizację wyników do Twojego powiadomienia.

    title_right: "wymagania systemowe"
    content_right: |
        GroupDocs.Signature for Java są obsługiwane na wszystkich głównych platformach i systemach operacyjnych. Przed wykonaniem poniższego kodu upewnij się, że masz zainstalowane w systemie następujące wymagania wstępne.

        * Systemy operacyjne: Microsoft Windows, Linux, MacOS
        * Środowiska programistyczne: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Pobierz najnowszą wersję GroupDocs.Signature for Java z [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsb file
        String filePath = "input.xlsb";
        // Set up output file
        String outputFilePath = "output.xlsb";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to update
        // set up particular signature id
        TextSignature signatureToUpdate = new TextSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(130);
        // specify signature height
        signatureToUpdate.setHeight(20);
        // set left position
        signatureToUpdate.setLeft(40);
        // set top position
        signatureToUpdate.setTop(50);
        // set up new text
        signatureToUpdate.setText("Mr. John Smith");

        // update signature
        Boolean updateResult = signature.update(outputFilePath, signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Aktualizacja podpisów Text na stronach dokumentu - Demo na żywo"
    content: |
       Edytuj różne podpisy elektroniczne dokumentu Xlsb już teraz, odwiedzając witrynę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Zaktualizuj różne podpisy Text przez Java"
    content: |
        "Edycja podpisów cyfrowych, które są umieszczane w różnych formatach dokumentów. Zaktualizuj dane podpisów bez dodatkowego kodu."
    format: 
       
       
back_to_top:
    enable: true
---