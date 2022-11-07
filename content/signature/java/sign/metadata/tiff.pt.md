---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Tiff
productName: Java
lang: pt
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Tiff for Java

############################# Head ############################
head_title: "Anexar assinaturas eletrônicas de metadados a documentos Tiff via Java"
head_description: "Use metadados como assinaturas eletrônicas ocultas dentro de seus documentos Tiff usando algumas linhas de código Java. Use a API de assinatura de documentos do GroupDocs para assinar seus documentos e arquivos comerciais com informações de metadados."

############################# Header ############################
title: "Assinaturas eletrônicas de metadados para o documento Tiff via Java são simples e fáceis de usar!"
description: "Assine seus documentos e contratos Tiff com entradas de metadados ocultas. Gere metadados para PDFs, documentos do MS Word, pastas de trabalho do MS Excel, apresentações do MS PowerPoint e vários formatos de imagem sem problemas e codificação extra."
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
    title: "Sobre a API de assinaturas de metadados do GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) é uma API popular para assinatura eletrônica de documentos digitais. Assinaturas como textos, imagens, certificados digitais, códigos de barras, códigos QR, carimbos ou metadados estão disponíveis. Assinaturas podem ser colocadas em PDFs, documentos do MS Word, pastas de trabalho do MS Excel, apresentações do MS PowerPoint, arquivos do Adobe Photoshop e vários formatos de imagem. Os clientes podem assinar seu documento e atualizar, pesquisar, verificar, excluir ou visualizar assinaturas eletrônicas que foram colocadas nesses documentos. Além disso, são fornecidas muitas habilidades para personalização de assinaturas.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Etapas para assinar Tiff com Metadata em Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) permite assinar documentos Tiff com assinaturas Metadata de forma rápida e fácil.
        
        * Crie uma instância da classe Signature fornecendo o arquivo Tiff para assinar como caminho ou fluxo de memória
        * Instancie a classe SignOptions e defina todos os dados exigidos.
        * Invoque o método Signature.Sign() passando o arquivo de saída Tiff ou fluxo de memória

    title_right: " Requisitos de sistema"
    content_right: |
        GroupDocs.Signature for Java são compatíveis com todas as principais plataformas e sistemas operacionais. Antes de executar o código abaixo, certifique-se de ter os seguintes pré-requisitos instalados em seu sistema.

        * Sistemas operacionais: Microsoft Windows, Linux, MacOS
        * Ambientes de desenvolvimento: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obtenha o GroupDocs.Signature for Java mais recente de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Tiff file
        String filePath = "input.tiff";
        // Set up output file
        String outputFilePath = "output.tiff";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // Specify different Metadata Signatures and add them to options signature collection
        // set start id
        int imgsMetadataId = 41996;
        // setup int value
        ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
        options.getSignatures().add(mdSign_DocId);
        // setup Author property
        ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
        options.getSignatures().add(mdSign_Author);
        // setup data of sign date
        ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, new Date()); // DateTime
        options.getSignatures().add(mdSign_Date);
        // setup double
        ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456); //decimal value
        options.getSignatures().add(mdSign_Amnt);

        // sign Tiff document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Assinando Tiff documentos com Metadata Demonstração ao vivo"
    content: |
       Assine o arquivo Tiff com várias assinaturas agora mesmo visitando o site [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demonstração online gratuita esperando por você.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Outras assinaturas Metadata suportadas para Java"
    content: |
        "Você também pode assinar Tiff com outros tipos de assinatura. Por favor, veja a lista abaixo."
    format: 
       
       
back_to_top:
    enable: true
---