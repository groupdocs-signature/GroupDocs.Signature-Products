---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Codabar
fileformat: Webp
productName: Java
lang: ku
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Webp for Java

############################# Head ############################
head_title: "eSign Webp belgeya bi Codabar Barcode di Java"
head_description: "Îmzeya barkodê ya Codabar biafirîne û bi çend rêzikên kodê bi Java li ser belgeya Webp biafirîne. Ji bo îmzekirina cûrbecûr formatên pelan API-ya Îmzekirina Belgeya GroupDocs bikar bînin."

############################# Header ############################
title: "Di Java de ji bo belgeya Codabar îmzeya barkodê çêbike"
description: "Belgeyên karsaziya xwe yên {{Pelformat}} bi Codabar Barkodê îmze bikin. Bi çend rêzikên kodê re zû û bi hêsanî îmzeya Barkodê biafirînin da ku vebijarkên îmzekirinê saz bikin."
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
    title: "Derbarê GroupDocs.Signature for Java API-ya îmzeyên barkodê."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) APIyek bilez û hêsan e ku ji bo birêvebirina e-îmzakirina belgeyên dîjîtal bi karanîna cûreyên barkodê yên wekî UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN. , ITF14 û gelekên din. Xerîdar dikarin bi hêsanî Barkodên ku nivîsa pêwîst peyda dikin biafirînin û wan bixin ser PDF, Belgeyên Microsoft Office Words, pirtûkên xebatê yên Microsoft Office Excel, pêşandanên MS PowerPoint, pelên Adobe Photoshop û formên cûda yên wêneyê. Barkodên ku di belgeyan de têne danîn dikarin bêne nûve kirin, lêgerîn, verastkirin, jêbirin an pêşdîtin. Digel vê yekê, xwerûkirina barkodê tê piştgirî kirin.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Gavên îmzekirina Webp bi Barcode di Java de"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) îmzakirina belgeyên Webp bi îmzeyên Barcode zû û bi hêsanî peyda dike.
        
        * Nimûneyek ji çîna îmzayê biafirîne ku pelê {{Pelformat}} pêşkêş dike ku divê wekî rêyek an herikîna bîranînê were îmzekirin
        * Dersa SignOptions destnîşan bikin û hemî daneyên daxwazkirî bicîh bikin.
        * Rêbaza Signature.Sign() vexwend ku derana pelê {{Pelformat}} an jî herikîna bîrê derbas dike

    title_right: " Pêdiviyên Sîstemê"
    content_right: |
        GroupDocs.Signature for Java li ser hemî platform û pergalên xebitandinê yên sereke têne piştgirî kirin. Berî ku hûn koda jêrîn bicîh bikin, ji kerema xwe pê ewle bibin ku we şertên jêrîn li ser pergala we hatine saz kirin.

        * Pergalên xebitandinê: Microsoft Windows, Linux, MacOS
        * Jîngehên pêşkeftinê: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Nûtirîn GroupDocs.Signature for Java ji [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) bistînin
         
    code: |
        ```java    
                
        // Set up input Webp file
        String filePath = "input.webp";
        // Set up output file
        String outputFilePath = "output.webp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Codabar);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Webp document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Îmzekirina belgeyên {{Pelformat}} bi Barcode Demoya Zindî"
    content: |
       Naha bi serdana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) pelê Webp bi îmzeyên cihêreng îmze bikin. Demoya serhêl a belaş li benda we ye.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Codabar Barcode"
          content: |
            Codabar sembolek barkodê ya xêzkirî ye ku ji bo formên pir-beş ên wekî FedEx hewayê û forma banka xwînê jî dema ku li ser çapkerên xal-matrixê tê çap kirin jî bi duristî were xwendin hatî çêkirin.
          characterset: |
             Reqemên hejmarî (0-9) û tîpên taybetî $/-:+.
          textcapacity: |
             Ne sînorkirinên taybetî.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAD0AAABGCAYAAAB/h5zrAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAK2SURBVHhe7c9BagQBDAPB/f+nNxDQpUCOfc1MQx8khMGf7wN5n34K79NP4X36KYxPfz6fX0OyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2svfi3/I+/RTeJ9+Cg98+vv9AViQgD/8yuhqAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Îmzeyên din ên piştgirî yên Barcode ji bo Java"
    content: |
        "Her weha hûn dikarin {{Pelformat}} bi celebên din ên îmzayê re îmze bikin. Ji kerema xwe lîsteya jêrîn bibînin."
    format: 
        
       
back_to_top:
    enable: true
---