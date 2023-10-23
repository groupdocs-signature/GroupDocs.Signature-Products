---
############################# Static ############################
layout: "landing"
date: 2023-10-23T14:58:10
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: pt
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, Java, APIs de nuvem e aplicativos de assinatura de documentos on-line"
head_description: "Obtenha uma solução completa de assinatura eletrônica de documentos para aplicativos .NET, Java e baseados em nuvem. Assine formatos de documentos comuns online usando o recurso simples de arrastar e soltar"

############################# Header ############################
title: "Assinar documentos<br>através da API .NET"
description: "Assine documentos e imagens digitais em qualquer plataforma usando nossas APIs flexíveis e soluções baseadas em aplicativos para programadores e usuários finais."
words:
  for: "para"

actions:
  main: "Download grátis do NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Licenciamento"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Pronto para começar?"
  description: "Experimente os recursos do GroupDocs.Signature gratuitamente ou solicite uma licença"

release:
  title: "Versão {0} lançada"
  notes: "Veja o que é novo"
  downloads: "Transferências"

code:
  title: "Assinar arquivos PDF em C#"
  more: "Mais exemplos"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Selecione o documento PDF
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Fornecer texto
        var options = new TextSignOptions("John Smith")
        {
            // Definir cor
            ForeColor = Color.Red
        };
        // Assine o documento e salve em arquivo
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Visão geral do GroupDocs.Signature"
  description: "API para executar assinatura de documentos e operações relacionadas em aplicativos .NET"
  features:
    # feature loop
    - title: "Adicionando assinaturas a documentos comerciais em C#"
      content: "Assinatura de documentos: Com GroupDocs.Signature for .NET, você pode adicionar vários tipos de assinaturas, como texto, imagens, códigos de barras e certificados digitais, a documentos PDF e Office. Esta API permite que você assine seus documentos com praticamente qualquer tipo de dados, incluindo metadados ocultos."

    # feature loop
    - title: "Processando documentos assinados"
      content: "Processamento adicional: você pode executar operações poderosas em documentos assinados usando GroupDocs.Signature. Isso inclui a busca de assinaturas existentes em documentos comerciais e sua verificação usando critérios específicos. Além disso, você pode recuperar informações de documentos e visualizar páginas por meio desta API .NET."

    # feature loop
    - title: "Personalizando resultados"
      content: "GroupDocs.Signature for .NET oferece amplas opções de personalização. Você pode posicionar assinaturas com precisão em qualquer lugar da página de um documento e ajustar sua aparência usando diversas configurações. Além disso, esta API suporta o salvamento de documentos processados ​​em uma ampla variedade de formatos suportados."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independência de plataforma"
  description: "GroupDocs.Signature for .NET oferece suporte aos seguintes sistemas operacionais, estruturas e gerenciadores de pacotes"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de arquivo suportados"
  description: |
    GroupDocs.Signature for .NET oferece suporte a operações com os seguintes [formatos de arquivo](https://docs.groupdocs.com/signature/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formatos do Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Imagens e outros formatos
        * **Portátil:** PDF
        * **Imagens:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Outros formatos de escritório:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Outros formatos
        * **Rede:** HTML, MHTML
        * **Arquivos:** ZIP, TAR, 7Z
        * **Certificados:** PFX

############################# Features ############################
features:
  enable: true
  title: "Recursos do GroupDocs.Signature"
  description: "Assine PDFs, documentos do Office e imagens com rapidez e precisão"

  items:
    # feature loop
    - icon: "sign"
      title: "Assinatura de documento"
      content: "Adicione um ou vários tipos de assinaturas compatíveis com precisão em qualquer posição especificada em documentos comerciais."

    # feature loop
    - icon: "custom"
      title: "Personalize assinaturas"
      content: "Utilize recursos como cor, fonte, borda, rotação, etc., para configurar a aparência das assinaturas."

    # feature loop
    - icon: "password"
      title: "Proteção por senha de documento"
      content: "Proteja determinados tipos de documentos definindo uma senha após a assinatura."

    # feature loop
    - icon: "protect"
      title: "Proteção contra mudanças"
      content: "Evite alterações em documentos comerciais importantes após anexar uma assinatura com um certificado digital."

    # feature loop
    - icon: "convert"
      title: "Converta arquivos assinados para outros formatos"
      content: "Converta arquivos assinados nos formatos desejados, como salvar um documento do Word como PDF."

    # feature loop
    - icon: "preview"
      title: "Extraia visualizações de páginas"
      content: "Extraia páginas de documentos assinados como imagens individuais para processamento futuro."

    # feature loop
    - icon: "search"
      title: "Pesquisa de assinatura em documentos"
      content: "Recuperar informações sobre assinaturas adicionadas anteriormente em documentos específicos."

    # feature loop
    - icon: "validate"
      title: "Validar documentos assinados"
      content: "Verifique a assinatura adequada dos documentos usando recursos de validação."

    # feature loop
    - icon: "update"
      title: "Atualizar ou excluir assinaturas"
      content: "Reposicione facilmente assinaturas específicas em uma página, modifique seu texto ou exclua-as sem problemas."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Amostras de código"
  description: "Alguns casos de uso de operações típicas de GroupDocs.Signature para .NET"
  items:
    # code sample loop
    - title: "Adicionar código QR ao PDF"
      content: |
        Adicionar [códigos QR](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) a páginas específicas de documentos PDF pode aprimorar os processos de negócios. Abaixo está um exemplo de como adicionar um código QR usando GroupDocs.Signature.
        {{< landing/code title="Como colocar código QR em PDF.">}}
        ```csharp {style=abap}
        // Carregue o documento para assinar
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Crie opções de código QR com texto predefinido
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Configure o tipo de codificação do código QR e a posição na página
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Assine o documento e salve-o como arquivo de resultado
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Protegendo um documento DOCX usando um certificado digital"
      content: |
        Você pode [proteger um documento](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) usando assinaturas pessoais ou corporativas armazenadas como certificados digitais. Tais documentos protegidos não podem ser modificados sem invalidar a assinatura.
        {{< landing/code title="Veja como garantir a integridade do documento.">}}
        ```csharp {style=abap}   
        // Carregue o documento a ser assinado digitalmente
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Especifique as opções de assinatura digital e forneça o caminho para o arquivo do certificado
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Defina a senha do certificado
                Password = "1234567890"
            };
            // Assine o documento e salve-o no caminho desejado
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
