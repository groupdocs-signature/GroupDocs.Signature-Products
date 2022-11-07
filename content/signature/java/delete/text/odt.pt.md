---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Text
fileformat: Odt
productName: Java
lang: pt
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Odt for Java

############################# Head ############################
head_title: "Excluir assinaturas Text de arquivos Odt via Java"
head_description: "A exclusão de assinaturas Text específicas de documentos Odt assinados pode ser realizada facilmente com o código curto Java."

############################# Header ############################
title: "Remova as assinaturas Text que são colocadas em arquivos Odt"
description: "Exclua várias assinaturas Text de documentos Odt. A remoção de assinaturas Text requer um código Java simples."
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
    title: "Obtenha informações sobre os recursos da API GroupDocs.Signature for Java"
    content: |
        A API [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) oferece várias maneiras de processar seus documentos usando assinaturas eletrônicas. Assinaturas digitais como textos, imagens, certificados digitais, códigos de barras, códigos QR, carimbos ou metadados estão disponíveis. Os clientes têm a possibilidade de adicionar, excluir, atualizar, verificar ou pesquisar assinaturas digitais em PDFs, documentos MS Word, pastas de trabalho MS Excel, apresentações MS PowerPoint, arquivos Adobe Photoshop e vários formatos de imagem. Um grande número de recursos e configurações úteis são fornecidos.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Como remover assinaturas Text do seu documento Odt"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) fornece um recurso útil para limpar documentos Odt de assinaturas Text com algumas linhas de código.
        
        * Em primeiro lugar, instancie o objeto Signature passando o caminho para o seu documento como um parâmetro do construtor.
        * Em seguida, crie um objeto de assinatura apropriado e configure seu identificador exclusivo.
        * Depois disso, invoque o método Delete passando o objeto de assinatura que deve ser excluído.
        * Finalmente, os resultados da operação do processo.

    title_right: "Requisitos de sistema"
    content_right: |
        GroupDocs.Signature for Java são compatíveis com todas as principais plataformas e sistemas operacionais. Antes de executar o código abaixo, certifique-se de ter os seguintes pré-requisitos instalados em seu sistema.

        * Sistemas operacionais: Microsoft Windows, Linux, MacOS
        * Ambientes de desenvolvimento: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Faça o download da versão mais recente do GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Odt file
        String filePath = "input.odt";
        // Set up output file
        String outputFilePath = "output.odt";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

        // provide signature features to delete
        TextSignature signatureToDelete = new TextSignature(id);

        // delete signature
        Boolean deleteResult = signature.delete(outputFilePath, signatureToDelete);

        // process deletion result
        if (deleteResult)
        {
                System.out.println("Signature was deleted successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Assinar com assinaturas Text Demonstração ao vivo"
    content: |
       Adicione várias assinaturas eletrônicas ao arquivo Odt agora mesmo visitando o site [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Exclua suas assinaturas Text com Java"
    content: |
        "Exclusão de assinaturas eletrônicas que foram adicionadas a vários formatos de documentos. Remova assinaturas rapidamente sem código extra."
    format: 
       
       
back_to_top:
    enable: true
---