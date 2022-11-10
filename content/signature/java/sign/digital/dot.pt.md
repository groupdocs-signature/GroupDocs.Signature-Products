---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Dot
productName: Java
lang: pt
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Dot for Java

############################# Head ############################
head_title: "Adicionando assinaturas eletrônicas digitais ao arquivo Dot com Java"
head_description: "Coloque a assinatura digital no arquivo Dot para Java usando algumas linhas de código. Use a API de assinatura de documentos do GroupDocs para assinar dezenas de formatos de arquivo."

############################# Header ############################
title: "eSign Dot arquivos com assinaturas Digital em Java"
description: "Como adicionar a assinatura Digital com algumas linhas de código Java"
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
    title: "Sobre a API de assinaturas digitais do GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) é uma API popular para assinar documentos com assinaturas eletrônicas digitais, com certificados digitais. Para a API de assinaturas digitais, usa arquivos de certificado PFX para assinar documentos com chaves privadas e públicas protegidas por senha. As assinaturas digitais podem ser usadas para certificar documentos comerciais com uma página específica do eSign PDF, certificar documentos inteiros do Microsoft Office, como Word, Excel, arquivos do Powerpoint e documentos do Open Office. Os clientes podem manipular facilmente as assinaturas, como editá-las, removê-las ou ajustá-las. A API fornece uma maneira de pesquisar e verificar assinaturas. Além disso, são fornecidas muitas habilidades para personalização de assinaturas.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Etapas para assinar Dot com Digital em Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) permite assinar documentos Dot com assinaturas Digital de forma rápida e fácil.
        
        * Crie uma instância da classe Signature fornecendo o arquivo Dot para assinar como caminho ou fluxo de memória
        * Instancie a classe SignOptions e defina todos os dados exigidos.
        * Invoque o método Signature.Sign() passando o arquivo de saída Dot ou fluxo de memória

    title_right: " Requisitos de sistema"
    content_right: |
        GroupDocs.Signature for Java são compatíveis com todas as principais plataformas e sistemas operacionais. Antes de executar o código abaixo, certifique-se de ter os seguintes pré-requisitos instalados em seu sistema.

        * Sistemas operacionais: Microsoft Windows, Linux, MacOS
        * Ambientes de desenvolvimento: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obtenha o GroupDocs.Signature for Java mais recente de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dot file
        String filePath = "input.dot";
        // Set up output file
        String outputFilePath = "output.dot";
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

        // sign Dot document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Assinando Dot documentos com Digital Demonstração ao vivo"
    content: |
       Assine o arquivo Dot com várias assinaturas agora mesmo visitando o site [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demonstração online gratuita esperando por você.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Outras assinaturas Digital suportadas para Java"
    content: |
        "Você também pode assinar Dot com outros tipos de assinatura. Por favor, veja a lista abaixo."
    format: 
       
       
back_to_top:
    enable: true
---