---
############################# Static ############################
layout: "landing"
date: 2024-03-04T17:52:03
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: ga
#productCode: nodejs-java
#otherformats: 
#breadcrumb: Put  signature on  for JavaScript
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: ".NET, Java, Cloud APIs & Aipeanna Sínithe Doiciméad Ar Líne"
head_description: "Faigh réiteach ríomhshínithe doiciméad uile-i-amháin le haghaidh .NET, Java agus feidhmchláir scamall-bhunaithe. Sínigh formáidí coiteanna doiciméad ar líne ag baint úsáide as gné simplí tarraing agus scaoil"

############################# Header ############################
title: "Doiciméid a shíniú<br>le Node.js API"
description: "Sínigh doiciméid agus íomhánna digiteacha ar aon ardán ag baint úsáide as ár n-APIanna solúbtha agus ár réitigh app-bhunaithe do ríomhchláraitheoirí agus úsáideoirí deiridh."
words:
  for: "le haghaidh"

actions:
  main: "Íosluchtaigh ceol ó NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Ceadúnú"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Réidh le tosú?"
  description: "Bain triail as gnéithe GroupDocs.Signature saor in aisce nó iarr ceadúnas"

release:
  title: "Leagan {0} eisithe"
  notes: "Féach cad atá nua"
  downloads: "Íoslódálacha"

code:
  title: "PDFs á síniú ag Node.js"
  more: "Tuilleadh samplaí"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```javascript {style=abap}   
    // Roghnaigh doiciméad PDF
    let signature = new Signature("sample.pdf");
    
    // Cuir téacs ar fáil
    let options = new TextSignOptions("John Smith");
    
    // Socraigh dath
    options.ForeColor = Color.Red;
    
    // Sínigh an doiciméad agus sábháil i gcomhad
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Forbhreathnú GroupDocs.Signature"
  description: "Leabharlann sínithe doiciméad atá réidh le húsáid in feidhmchláir Node.js"
  features:
    # feature loop
    - title: "Réiteach Sínithe Digiteacha do Dhoiciméid Ghnó le Node.js"
      content: "Tairgeann GroupDocs.Signature for Node.js via Java sraith chuimsitheach de roghanna sínithe digiteacha do PDF, doiciméid Office agus íomhánna. Tá téacs, barrachóid, íomhánna, deimhnithe digiteacha agus meiteashonraí ar fáil. Cinntíonn próiseáil shruthlínithe doiciméad éifeachtúlacht."

    # feature loop
    - title: "Ard-ionramháil ar Dhoiciméid Sínithe"
      content: "Ligeann GroupDocs.Signature duit doiciméid sínithe a phróiseáil. Cuardaigh agus bailíochtaigh sínithe ag baint úsáide as critéir éagsúla. Ina theannta sin, bain eolas mionsonraithe doiciméad nó gin íomhánna réamhamhairc de leathanaigh."

    # feature loop
    - title: "Formáidí Aschuir Éagsúla"
      content: "Soláthraíonn ár réiteach rialú fairsing ar fhormáid aschuir doiciméad sínithe. Cuir sínithe go beacht ar aon leathanach agus saincheapadh a gcuma. Sábháil doiciméid sínithe i bhformáidí iomadúla a dtacaítear leo agus déan iad a dhaingniú go roghnach le pasfhocail."

############################# Platforms ############################
platforms:
  enable: true
  title: "Neamhspleáchas ardán"
  description: "Déanann GroupDocs.Signature for Node.js via Java próiseáil doiciméad le córais oibriúcháin éagsúla"
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
  title: "Formáidí comhaid tacaithe"
  description: |
    Éascaíonn GroupDocs.Signature for Node.js via Java oibríochtaí do na [formáidí comhaid coitianta](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formáidí microsoft office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Íomhánna & Formáidí Eile
        * **Inaistrithe:** PDF
        * **Íomhánna:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Formáidí oifige eile:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Formáidí eile
        * **Gréasán:** HTML, MHTML
        * **Cartlanna:** ZIP, TAR, 7Z
        * **Deimhnithe:** PFX

############################# Features ############################
features:
  enable: true
  title: "Gnéithe de GroupDocs.Signature"
  description: "Sínigh PDFs, doiciméid Oifige, agus íomhánna le sínithe digiteacha"

  items:
    # feature loop
    - icon: "sign"
      title: "Sínithe Gnó"
      content: "Fostú cineálacha sínithe éagsúla chun doiciméid a shíniú. Cuir sínithe digiteacha go beacht ar shuíomh leathanach ar bith."

    # feature loop
    - icon: "custom"
      title: "Cuma Síniú a shaincheapadh"
      content: "Cuir gnéithe amhairc na sínithe in oiriúint trí dhath, cló, teorainneacha, rothlú, agus níos mó a choigeartú chun an toradh inmhianaithe a bhaint amach."

    # feature loop
    - icon: "password"
      title: "Doiciméid Pasfhocal-Chosanta"
      content: "I gcás go leor formáidí doiciméad tacaithe, déan doiciméid sínithe a chosaint le pasfhocal le haghaidh slándála breise."

    # feature loop
    - icon: "protect"
      title: "Modhnuithe Neamhúdaraithe a Chosc"
      content: "Doiciméid ghnó ríthábhachtacha atá sínithe le deimhnithe digiteacha a chosaint ó athruithe neamhúdaraithe."

    # feature loop
    - icon: "convert"
      title: "Formáidí Aschuir Inmhianaithe"
      content: "Faigh doiciméid sínithe gan stró i bhformáid ar bith a dtacaítear léi. Tiontaigh doiciméid MS Word go formáid PDF gan stró."

    # feature loop
    - icon: "preview"
      title: "Réamhamharc ar Dhoiciméid"
      content: "Sábháil leathanaigh aonair doiciméad mar íomhánna do riachtanais sa todhchaí."

    # feature loop
    - icon: "search"
      title: "Cuardach Síniú"
      content: "Aisghabh faisnéis faoi shínithe a cuireadh leis roimhe seo laistigh de do dhoiciméid."

    # feature loop
    - icon: "validate"
      title: "Bailíochtú Doiciméad"
      content: "Fíoraigh barántúlacht na sínithe a chuirtear i láthair in aon doiciméad."

    # feature loop
    - icon: "update"
      title: "Bainistíocht Síniú"
      content: "Scrios, athlonnaigh, nó modhnaigh aon sínithe a chuirtear ar aon leathanach doiciméid."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Cóid samplaí"
  description: "Samplaí léiriúcháin a thaispeánann oibríochtaí tipiciúla GroupDocs.Signature for Node.js via Java"
  items:
    # code sample loop
    - title: "Marcáil pdf le cóid QR"
      content: |
        Má ionchorpraítear [barrachóid](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) i leathanaigh ar leith doiciméad PDF, féadtar próisis ghnó a shruthlíniú. Soláthraíonn an rannán seo sampla de chód QR a chur leis trí úsáid a bhaint as GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Conas a cuir an cód QR i bhformáid pdf.">}}
        ```javascript {style=abap}
        // Íoslódáil an doiciméad le síniú
        let signature = new Signature("file_to_sign.pdf");
        
        // Cruthaigh roghanna cód QR le téacs réamhshainithe
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Cumraigh cineál ionchódaithe cód QR agus suíomh ar an leathanach
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Sínigh an doiciméad agus sábháil é mar chomhad toraidh
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX a chosaint le Síniú Digiteach"
      content: |
        [Cosain do Dhoiciméid](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) trí shínithe bunaithe ar theastais dhigiteacha. Cosnaíonn síniú digiteach do dhoiciméid ghnó in aghaidh athrú ábhair.
        {{< landing/code title="Seo conas sláine doiciméad a chinntiú.">}}
        ```javascript {style=abap}   
        // Íoslódáil an doiciméad le síniú digiteach
        let signature = new Signature("file_to_sign.pdf");
        
        // Sonraigh roghanna sínithe digiteacha agus cuir an cosán chuig an gcomhad teastais ar fáil
        let options = new DigitalSignOptions("certificate.pfx");

        // Socraigh focal faire an teastais
        options.Password = "1234567890";

        // Sínigh an doiciméad agus é a shábháil ar an cosán atá ag teastáil
        signature.Sign("digitally_signed.pdf", options);

        ```
        {{< /landing/code >}}

---
