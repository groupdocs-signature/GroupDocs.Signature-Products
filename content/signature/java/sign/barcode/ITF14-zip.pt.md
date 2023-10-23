---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: I T F14
fileformat: Zip
productName: Java
lang: pt
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Zip for Java

############################# Head ############################
head_title: "eSign Zip documento com I T F14 Código de barras em Java"
head_description: "Crie uma assinatura de código de barras I T F14 e coloque-a no documento Zip com Java usando algumas linhas de código. Use a API de assinatura de documento do GroupDocs para assinar vários formatos de arquivo."

############################# Header ############################
title: "Gere assinatura de código de barras I T F14 para Zip documento em Java"
description: "Assine seus documentos comerciais Zip com o código de barras I T F14. Gere assinatura de código de barras de forma rápida e fácil com algumas linhas de código para configurar as opções de assinatura."
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
    title_left: "Etapas para assinar Zip com Barcode em Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) permite assinar documentos Zip com assinaturas Barcode de forma rápida e fácil.
        
        * Crie uma instância da classe Signature fornecendo o arquivo Zip para assinar como caminho ou fluxo de memória
        * Instancie a classe SignOptions e defina todos os dados exigidos.
        * Invoque o método Signature.Sign() passando o arquivo de saída Zip ou fluxo de memória

    title_right: " Requisitos de sistema"
    content_right: |
        GroupDocs.Signature for Java são compatíveis com todas as principais plataformas e sistemas operacionais. Antes de executar o código abaixo, certifique-se de ter os seguintes pré-requisitos instalados em seu sistema.

        * Sistemas operacionais: Microsoft Windows, Linux, MacOS
        * Ambientes de desenvolvimento: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obtenha o GroupDocs.Signature for Java mais recente de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Zip file
        String filePath = "input.zip";
        // Set up output file
        String outputFilePath = "output.zip";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.I T F14);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Zip document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Assinando Zip documentos com Barcode Demonstração ao vivo"
    content: |
       Assine o arquivo Zip com várias assinaturas agora mesmo visitando o site [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demonstração online gratuita esperando por você.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About I T F14 Barcode"
          content: |
            ITF-14 é a implementação GS1 de um código de barras Interleaved 2 of 5 (ITF) para codificar um Número Global de Item Comercial.
          characterset: |
             Dígitos numéricos (0-9).
          textcapacity: |
             13 dígitos + 1 dígito verificador.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Outras assinaturas Barcode suportadas para Java"
    content: |
        "Você também pode assinar Zip com outros tipos de assinatura. Por favor, veja a lista abaixo."
    format: 
        
       
back_to_top:
    enable: true
---