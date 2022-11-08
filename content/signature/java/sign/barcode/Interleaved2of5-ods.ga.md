---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Interleaved2of5
fileformat: Ods
productName: Java
lang: ga
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Ods for Java

############################# Head ############################
head_title: "eSign Ods doiciméad le Interleaved2of5 Barcode in Java"
head_description: "Cruthaigh Interleaved2of5 Síniú Barrachóid agus cuir ar Ods doiciméad le Java ag baint úsáide as cúpla líne de chód. Bain úsáid as an GroupDocs Document Signature API chun formáidí éagsúla comhaid a shíniú."

############################# Header ############################
title: "Gin síniú barrachóid Interleaved2of5 don doiciméad Ods in Java"
description: "eSínigh do dhoiciméid ghnó Ods le Barrachóid Interleaved2of5. Gin síniú Barrachóid go tapa agus go héasca le cúpla líne de chód chun roghanna sínithe a shocrú."
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
    title: "Maidir le GroupDocs.Signature for Java sínithe barcode API."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) is API tapa agus éasca é chun ríomhshíniú doiciméad digiteach a bhainistiú ag baint úsáide as cineálacha Barrachóid amhail UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 agus go leor eile. Is féidir le custaiméirí barrachóid a chruthú go héasca ag soláthar an téacs riachtanach agus iad a chur ar PDF, Doiciméid Microsoft Office Words, leabhair oibre Microsoft Office Excel, láithreoireachtaí MS PowerPoint, comhaid Adobe Photoshop agus formáidí éagsúla íomhá. Is féidir barrachóid a chuirtear i ndoiciméid a nuashonrú, a chuardach, a fhíorú, a scriosadh nó a réamhamharc. Ina theannta sin, tacaítear le saincheaptha barrachóid.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Céimeanna chun Ods a shíniú le Barcode in Java"
    content_left: |
        Soláthraíonn [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) cumas chun doiciméid Ods a shíniú le sínithe Barcode go tapa agus go héasca.
        
        * Cruthaigh sampla d'aicme Sínithe ag soláthar Ods comhad atá ceaptha a shíniú mar chonair nó mar shruth cuimhne
        * Cuir rang SignOptions ar bun agus socraigh na sonraí go léir a éilítear.
        * Iarr ar an modh Signature.Sign() aschuir {{ Fileformat}} comhad nó sruth cuimhne a rith

    title_right: " Riachtanais Chórais"
    content_right: |
        Tacaítear le GroupDocs.Signature for Java ar gach mór-ardán agus córas oibriúcháin. Sula ndéanann tú an cód thíos, déan cinnte go bhfuil na réamhriachtanais seo a leanas suiteáilte ar do chóras.

        * Córais oibriúcháin: Microsoft Windows, Linux, MacOS
        * Timpeallachtaí forbartha: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Faigh an GroupDocs.Signature for Java is déanaí ó [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ods file
        String filePath = "input.ods";
        // Set up output file
        String outputFilePath = "output.ods";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Interleaved2of5);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Ods document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ag síniú Ods doiciméad le {{ Signaturetype}} Taispeántas Beo"
    content: |
       Sínigh Ods comhad le sínithe éagsúla faoi láthair trí chuairt a thabhairt ar an suíomh Gréasáin [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Saor in aisce taispeána ar líne ag fanacht leat.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Interleaved2of5 Barcode"
          content: |
            Idirdhuilleogach 2 de 5 (ITF) is ea digití leanúnacha ionchódaithe siombaile cód barra dhá leithead. Úsáidtear é go tráchtála ar 135 scannán, le haghaidh barrachóid ITF-14, agus ar cartáin roinnt táirgí, agus tá na táirgí taobh istigh lipéadaithe le UPC nó EAN.
          characterset: |
             digití uimhriúla (0-9).
          textcapacity: |
             Fad athraitheach.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAB8AAACGCAYAAAAlx1GyAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAFdSURBVHhe7Y0xCkJRAMPe/S/9BSFLqHaSN9hAhyzNeS6y+BUWv8LX+DnnPfjkHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3X+K9Z/Ar/Gn+eF5E2tt5Q4JATAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Sínithe Barcode eile a dtacaítear leo le haghaidh Java"
    content: |
        "Is féidir leat Ods a shíniú le cineálacha sínithe eile freisin. Féach ar an liosta thíos le do thoil."
    format: 
        
       
back_to_top:
    enable: true
---