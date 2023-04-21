---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "API de assinatura digital Java, adicionar assinatura eletrônica a PDF Word Excel Image"
head_description: "API de assinatura digital Java. Biblioteca de assinatura eletrônica para assinar digitalmente PDF, Microsoft Word, planilhas do Excel, apresentações em PowerPoint e formatos de documento de imagem."

############################# Header ############################
title: "API Java para gerenciar assinaturas digitais"
description: "Gerencie a assinatura eletrônica de imagem, código QR, código de barras, metadados, tipos de texto e carimbo em aplicativos Java para imagens de assinatura e formatos de arquivo de documento digital."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Visão geral"

            # button loop
            - link: "#features"
              text: "Características"

            # button loop
            - link: "#support"
              text: "Apoiar"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Demonstração ao vivo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Preços"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature para Java API ajuda você a desenvolver aplicativos Java com funcionalidade de assinaturas eletrônicas para assinar documentos digitais de formatos suportados sem instalar nenhum software externo. Ele suporta a manipulação e gerenciamento de vários tipos de assinaturas eletrônicas, como imagem, código de barras, QR-Code, carimbo, texto, óptica e metadados. Todos os seus documentos comerciais eletrônicos, como o Microsoft Office Word, apresentações em PowerPoint, planilhas do Excel, imagens e arquivos PDF, podem ser assinados digitalmente, personalizando as propriedades da assinatura, por exemplo. sombra, dimensões, alinhamento e muito mais de acordo com suas necessidades. A biblioteca de assinatura digital é simples e leve, consistindo em um único arquivo DLL que pode ser integrado facilmente em um aplicativo Java novo ou existente.  

      Através do GroupDocs.Signature para Java API você pode carregar todos os certificados registrados do sistema, ou localizar assinaturas existentes usando busca simples e avançada. As opções para trabalhar com documentos protegidos por senha, especificando propriedades de assinatura comuns (tamanho do texto, opacidade, rotação, verificação, propriedades de fonte, opções de cores, número de página, largura, superior, esquerdo etc.) Solução de gerenciamento de assinaturas eletrônicas para documentos digitais.  

      GroupDocs.Signature for Java é compatível com todas as versões do Java e oferece suporte a sistemas operacionais populares (Windows, Linux, MacOS) capazes de executar Java runtime
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Esta é uma visão geral dos recursos do GroupDocs.Signature para Java:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Tipos de assinatura"
          content: |
            * Assinatura de texto
            * Assinatura de imagem
            * Assinaturas digitais
            * Assinatura de código QR
            * Assinatura de código de barras
            * Carimbo Assinatura
            * Assinatura do campo de formulário
      
      ## TAB TWO ##
      tab_two:
        description: |
          A API de assinatura eletrônica Java oferece suporte a vários formatos de arquivo de documento, conforme listado abaixo. [Formatos de documentos suportados.](https://docs.groupdocs.com/signature/java/supported-document-formats/)

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM

        right:
          enable: true
          table:
            # table loop
            - title: "Images & Other Formats"
              content: |
                * **Imagens**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **Metarquivos**: EMF, WMF, CMX
                * **Portátil**: PDF
                * **Gráficos vetoriais escalonáveis**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **Outros**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature for Java oferece suporte aos seguintes sistemas operacionais, estruturas e gerenciadores de pacotes:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Sistemas operacionais"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Estruturas suportadas"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Ambientes de Desenvolvimento"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Construir Ferramenta de Automação"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Signature para recursos Java"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Crie, leia, modifique, oculte e exclua assinaturas eletrônicas de formatos de documento suportados"

      # feature loop
      - icon: "fas fa-eye"
        content: "Acesso ao documento assinado a partir do fluxo, caminho relativo ou caminho absoluto"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Aplicar assinatura de texto a documentos, planilhas, apresentações, imagens e arquivos PDF"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Adicione assinatura de texto como anotação, adesivo, imagem a arquivos PDF e também configure estilo e cor"

      # feature loop
      - icon: "fas fa-code"
        content: "Assine documento PDF, arquivo de imagem e obtenha saída em formato de arquivo diferente"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Assine digitalmente imagens com assinatura de texto como marca d'água e adicione transparência, rotação à assinatura eletrônica"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Pesquise certificados e assine documentos do Microsoft Word, Excel e PDF com certificados digitais"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Assinar formatos de documento de processamento de texto com marcas d'água de texto nativo"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Use QR-Code, código de barras para assinar arquivos de palavras, slides, células, PDF e imagens"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Configurar e aplicar assinaturas de carimbo para proteger os formatos de arquivo suportados"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Configurar e atribuir assinaturas de imagem a documentos, planilhas, apresentações, imagens e arquivos PDF"

      # feature loop
      - icon: "fas fa-columns"
        content: "Configure as Propriedades da Assinatura, por exemplo, Aparência, Margens, Alinhamento, etc."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Aplicar assinatura digital ao documento protegido por senha"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Execute a verificação de texto de documentos PDF usando o manipulador de assinatura"

      # feature loop
      - icon: "fas fa-print"
        content: "Verificação digital de documentos Word, Cell e PDF com contêineres de certificados .CER e .PFX"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Especifique diferentes tipos de unidade de medida (por exemplo, milímetros, pixels, etc.) para assinaturas de texto em PDF"

      # feature loop
      - icon: "fas fa-lock"
        content: "Obtenha informações do documento por meio de arquivo ou URL - adicione assinaturas de campo de formulário a documentos PDF"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Adicionar objeto de dados personalizados, VCard incorporado, e-mail, EPC, MeCard ou objeto de evento ao código QR"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Aplique diferentes estilos de pincel às assinaturas, por exemplo, Gradiente, Radial, Sólido e Pincel de textura"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Assinar documento localizado no FTP ou Azure Cloud Storage"

      # feature loop
      - icon: "fas fa-heading"
        content: "Definir alinhamento de texto dentro de formas para documentos, slides, imagens e arquivos PDF"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Pesquise, verifique e assine digitalmente documentos de apresentação do PowerPoint"

      # feature loop
      - icon: "fas fa-cube"
        content: "Colocar assinatura usando pixels em documentos de célula e posicionamento de texto para assinaturas de carimbo"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Implementar assinatura de carimbo retangular com cantos arredondados"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Estenda assinaturas de código de barras e QR-Code com conteúdo de dados de imagem"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Adicionar assinaturas de metadados criptografados ao trabalhar com opções de assinatura e pesquisa"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Incorpore objetos personalizados a assinaturas de metadados no Word, Excel e apresentações"

    more_feature:
      # more_feature_loop
      - title: "Configure e aplique facilmente assinaturas eletrônicas"
        content: |
          GroupDocs.Signature para Java API permite configurar e adicionar assinaturas eletrônicas a formatos de documento suportados. A seguir está um exemplo de código que mostra como é simples aplicar uma assinatura de texto a um arquivo PDF:

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // definir posição de assinatura
          options.setLeft(100);
          options.setTop(100);
          
          // definir retângulo de assinatura
          options.setWidth(100);
          options.setHeight(30);

          // definir a cor do texto e a fonte
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // assinar documento para arquivar
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "Tipos de codificação de código de barras suportados para assinatura eletrônica"
        content: |
          Usando GroupDocs.Signature para Java API, você pode aplicar código de barras e assinaturas de código QR para formatos de arquivo suportados. GroupDocs.Signature for Java oferece suporte a uma grande variedade de tipos de codificação de código de barras para atender à maioria dos requisitos. Os tipos de codificação de código de barras suportados incluem, Code 11, Code 128, Code 16K/32, Databar codes, GS1 Codeblock, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard e Code39 Estendido.

          Da mesma forma, GroupDocs.Signature para Java API permite que você use tipos de código QR, como QR, Aztec e Data Matrix. Os tipos de codificação QR-Code suportados incluem Aztec, DataMatrix, GS1 DataMatrix e GS1 QR.

      # more_feature_loop
      - title: "Pesquisar assinaturas e certificados"
        content: |
          Por meio do GroupDocs.Signature for Java API, você pode pesquisar assinaturas de QR-Code e Barcode em qualquer documento, apresentação, planilha, imagem, bem como arquivo PDF, e obter o resultado da pesquisa. Você também pode pesquisar objetos de dados personalizados de documentos assinados com assinatura de código QR, bem como pesquisar VCard padrão e objeto de e-mail de documentos assinados com código QR. A verificação de texto criptografado de assinaturas de QR-Code, bem como a pesquisa de assinatura de metadados em documentos PDF também são suportadas. Aplique critérios de pesquisa adicionais para assinaturas digitais de documentos Words & Cells.  

          A opção de pesquisa também está disponível para assinatura de metadados para documentos do Word, slides e planilhas, enquanto a pesquisa de campos de formulário está disponível para documentos PDF.

      # more_feature_loop
      - title: "Configurar propriedades de assinatura eletrônica"
        content: |
          Para aprimorar o UX dos usuários finais, o GroupDocs.Signature for Java API fornece várias propriedades que podem ser configuradas com bastante facilidade. Você pode definir as opções de fonte e cor (cor de fundo, cor de primeiro plano, negrito, itálico, sublinhado, família de fontes, tamanho da fonte, etc.), opções de plano de fundo e borda (cor de fundo, transparência de fundo, cor de borda, estilo de traço de borda, espessura de borda, Transparência de borda etc.), Margens de assinatura (esquerda, superior, largura, altura, preenchimento etc.) e Área de assinatura de imagem de configuração e Alinhamento de assinatura (Alinhamento horizontal, Alinhamento vertical etc.).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature oferece APIs de assinatura de documentos para outros ambientes de desenvolvimento populares"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
          product: "GroupDocs.Signature"
          platform: ".NET"
          link: "/signature/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---