---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Codabar
fileformat: Rtf
productName: Java
lang: pt
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Rtf for Java

############################# Head ############################
head_title: "eSign Rtf documento com Codabar Código de barras em Java"
head_description: "Crie uma assinatura de código de barras Codabar e coloque-a no documento Rtf com Java usando algumas linhas de código. Use a API de assinatura de documento do GroupDocs para assinar vários formatos de arquivo."

############################# Header ############################
title: "Gere assinatura de código de barras Codabar para Rtf documento em Java"
description: "Assine seus documentos comerciais Rtf com o código de barras Codabar. Gere assinatura de código de barras de forma rápida e fácil com algumas linhas de código para configurar as opções de assinatura."
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
    title: "Sobre a API de assinaturas de código de barras do GroupDocs.Signature for Java."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) é uma API rápida e fácil para gerenciar a assinatura eletrônica de documentos digitais usando tipos de código de barras como UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 e muitos outros. Os clientes podem criar facilmente códigos de barras fornecendo o texto necessário e colocá-los em PDF, documentos do Microsoft Office Words, pastas de trabalho do Microsoft Office Excel, apresentações do MS PowerPoint, arquivos do Adobe Photoshop e vários formatos de imagem. Os códigos de barras colocados em documentos podem ser atualizados, pesquisados, verificados, excluídos ou visualizados. Além disso, a personalização de códigos de barras é suportada.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Etapas para assinar Rtf com Barcode em Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) permite assinar documentos Rtf com assinaturas Barcode de forma rápida e fácil.
        
        * Crie uma instância da classe Signature fornecendo o arquivo Rtf para assinar como caminho ou fluxo de memória
        * Instancie a classe SignOptions e defina todos os dados exigidos.
        * Invoque o método Signature.Sign() passando o arquivo de saída Rtf ou fluxo de memória

    title_right: " Requisitos de sistema"
    content_right: |
        GroupDocs.Signature for Java são compatíveis com todas as principais plataformas e sistemas operacionais. Antes de executar o código abaixo, certifique-se de ter os seguintes pré-requisitos instalados em seu sistema.

        * Sistemas operacionais: Microsoft Windows, Linux, MacOS
        * Ambientes de desenvolvimento: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obtenha o GroupDocs.Signature for Java mais recente de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Rtf file
        String filePath = "input.rtf";
        // Set up output file
        String outputFilePath = "output.rtf";

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

        // sign Rtf document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Assinando Rtf documentos com Barcode Demonstração ao vivo"
    content: |
       Assine o arquivo Rtf com várias assinaturas agora mesmo visitando o site [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demonstração online gratuita esperando por você.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Codabar Barcode"
          content: |
            Codabar é uma simbologia de código de barras linear que foi projetada para ser lida com precisão mesmo quando impressa em impressoras matriciais para formulários de várias vias, como contas aéreas da FedEx e formulário de banco de sangue.
          characterset: |
             Dígitos numéricos (0-9) e caracteres especiais $/-:+.
          textcapacity: |
             Sem restrições específicas.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAD0AAABGCAYAAAB/h5zrAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAK2SURBVHhe7c9BagQBDAPB/f+nNxDQpUCOfc1MQx8khMGf7wN5n34K79NP4X36KYxPfz6fX0OyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2svfi3/I+/RTeJ9+Cg98+vv9AViQgD/8yuhqAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Outras assinaturas Barcode suportadas para Java"
    content: |
        "Você também pode assinar Rtf com outros tipos de assinatura. Por favor, veja a lista abaixo."
    format: 
        
       
back_to_top:
    enable: true
---