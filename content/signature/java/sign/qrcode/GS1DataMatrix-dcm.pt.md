---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Qrcode
codetype: G S1 Data Matrix
fileformat: Dcm
productName: Java
lang: pt
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Qrcode signature on Dcm for Java

############################# Head ############################
head_title: "eSign Dcm documento com G S1 Data Matrix QR Code em Java"
head_description: "Crie G S1 Data Matrix QR Code e coloque-o no arquivo Dcm usando Java com um pequeno pedaço de código Java. Use a API de assinatura de documentos do GroupDocs para assinar seus documentos e arquivos comerciais com QR Code."

############################# Header ############################
title: "Gere G S1 Data Matrix assinatura de QR Code para Dcm documento em Java"
description: "Assine seus documentos e contratos Dcm com G S1 Data Matrix QR Code. Gere assinatura de QR Code de forma rápida e fácil."
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
    title: "Sobre a API de assinaturas de código QR do GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) é uma API madura para criar e gerar assinaturas de QR Code para os documentos. Os usuários podem gerar assinaturas de QR Code fornecendo texto para baixá-lo ou compartilhar nas mídias sociais como imagem. O documento assinado pode ser digitalizado com API ou simplesmente pela câmera do celular! Assine eletronicamente seus contratos comerciais e documentos oficiais adicionando a assinatura do QR Code e manipule-o. Qualquer assinatura de QR Code conterá informações personalizadas exclusivas para identificar o signatário ou autorizar o documento. Além disso, o conteúdo do QR Code pode ser criptografado e descriptografado com chaves pessoais de forma programática. Isso abre muitas habilidades para compartilhar dados confidenciais dentro dos documentos públicos. Após a assinatura, o usuário pode atualizar, verificar, excluir, visualizar ou pesquisar os QR Codes em PDFs, documentos do MS Word, pastas de trabalho do MS Excel, apresentações do MS PowerPoint, arquivos do Adobe Photoshop e vários formatos de imagem. Códigos QR podem ser personalizados adicionalmente.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Etapas para assinar Dcm com Qrcode em Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) permite assinar documentos Dcm com assinaturas Qrcode de forma rápida e fácil.
        
        * Crie uma instância da classe Signature fornecendo o arquivo Dcm para assinar como caminho ou fluxo de memória
        * Instancie a classe SignOptions e defina todos os dados exigidos.
        * Invoque o método Signature.Sign() passando o arquivo de saída Dcm ou fluxo de memória

    title_right: " Requisitos de sistema"
    content_right: |
        GroupDocs.Signature for Java são compatíveis com todas as principais plataformas e sistemas operacionais. Antes de executar o código abaixo, certifique-se de ter os seguintes pré-requisitos instalados em seu sistema.

        * Sistemas operacionais: Microsoft Windows, Linux, MacOS
        * Ambientes de desenvolvimento: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obtenha o GroupDocs.Signature for Java mais recente de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dcm file
        String filePath = "input.dcm";
        // Set up output file
        String outputFilePath = "output.dcm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(QrCodeTypes.G S1 Data Matrix);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Dcm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Assinando Dcm documentos com Qrcode Demonstração ao vivo"
    content: |
       Assine o arquivo Dcm com várias assinaturas agora mesmo visitando o site [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demonstração online gratuita esperando por você.

              
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About G S1 Data Matrix QrCode"
          content: |
            GS1 Data Matrix é uma variante do Data Matrix que está em conformidade com as especificações GS1. Use o GS1 DataMatrix para codificar as informações como, mas não se limitando a: AI(01) Global Trade Item Number (GTIN), AI(17) Expiration Date, AI(10) Batch Number, AI(21) Serial Number .
          characterset: |
             Conjunto de caracteres: letras maiúsculas e minúsculas e caracteres especiais $@%*+-./:=<>;&*_,'! todos com Identificadores de Aplicativos corretos.
          textcapacity: |
             Capacidade de texto de código: até 3116 dígitos numéricos ou 2335 caracteres alfanuméricos.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Outras assinaturas Qrcode suportadas para Java"
    content: |
        "Você também pode assinar Dcm com outros tipos de assinatura. Por favor, veja a lista abaixo."
    format: 
        
       
back_to_top:
    enable: true
---