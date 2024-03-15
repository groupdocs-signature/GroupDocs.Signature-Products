---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:49
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: ga
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

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
head_title: "Leabharlann Sínithe Digiteach Java - GroupDocs.Signature"
head_description: "Cumasaigh feidhmchláir Java trí ríomhshínithe le GroupDocs.Signature. Sínigh doiciméid ghnó go tapa agus gan stró."

############################# Header ############################
title: "Doiciméid a shíniú<br>trí Java API"
description: "Sínigh doiciméid agus íomhánna digiteacha ar aon ardán ag baint úsáide as ár n-APIanna solúbtha agus ár réitigh app-bhunaithe do ríomhchláraitheoirí agus úsáideoirí deiridh."
words:
  for: "le haghaidh"

actions:
  main: "Maven saor in aisce, íoslódáil"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Ceadúnú"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Réidh le tosú?"
  description: "Bain triail as gnéithe GroupDocs.Signature saor in aisce nó iarr ceadúnas"

release:
  title: "Leagan {0} eisithe"
  notes: "Féach cad atá nua"
  downloads: "Íoslódálacha"

code:
  title: "Sínigh comhaid pdf i java"
  more: "Tuilleadh samplaí"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Roghnaigh doiciméad PDF
    Signature signature = new Signature("sample.pdf");
    
    // Cuir téacs ar fáil
    TextSignOptions options = 
        new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Sínigh an doiciméad agus sábháil i gcomhad
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Forbhreathnú GroupDocs.Signature"
  description: "API chun síniú doiciméad agus oibríochtaí gaolmhara a dhéanamh i bhfeidhmchláir Java"
  features:
    # feature loop
    - title: "Doiciméid ghnó feabhsaithe le sínithe digiteacha i Java"
      content: "Síniú tapa agus inoiriúnaithe: Tairgeann GroupDocs.Signature do Java raon leathan roghanna sínithe digiteacha do PDFs, íomhánna agus doiciméid Oifige. Is féidir leat téacs, barrachóid, QR-cóid, teastais dhigiteacha, pictiúir, nó meiteashonraí ceilte a úsáid. Tá próiseáil doiciméad tapa agus éifeachtach."

    # feature loop
    - title: "Ag ionramháil doiciméad sínithe"
      content: "Is éard atá i gceist le hardphróiseáil doiciméad ná oibríochtaí cumhachtacha ar dhoiciméid sínithe ag baint úsáide as GroupDocs.Signature do Java. Is féidir leat sínithe a cuireadh le doiciméid ghnó a chuardach agus a bhailíochtú ag baint úsáide as critéir úsáideacha éagsúla. Ina theannta sin, is féidir leat rochtain a fháil ar fhaisnéis mhionsonraithe faoin doiciméad nó íomhánna réamhamhairc dá leathanaigh a fháil."

    # feature loop
    - title: "Éagsúlacht roghanna aschuir"
      content: "Ligeann roghanna sínithe láidre duit an t-aschur a shaincheapadh do dhoiciméid sínithe le GroupDocs.Signature do Java. Is féidir leat aon síniú a shuíomh go beacht ar aon leathanach doiciméid agus a chuma a chumrú ar bhealaí éagsúla. Tacaíonn an Java API le doiciméid ghnó sínithe a shábháil i bhformáidí iomadúla tacaithe agus cuireann sé roghanna ar fáil chun iad a dhaingniú le pasfhocail."

############################# Platforms ############################
platforms:
  enable: true
  title: "Neamhspleáchas ardán"
  description: "Tacaíonn GroupDocs.Signature do Java leis na córais oibriúcháin, creataí agus bainisteoirí pacáiste seo a leanas"
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Formáidí comhaid tacaithe"
  description: |
    Tacaíonn GroupDocs.Signature le haghaidh Java le hoibríochtaí leis na [formáidí comhaid](https://docs.groupdocs.com/signature/java/supported-document-formats/) seo a leanas.
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
  title: "Gnéithe GroupDocs.Signature"
  description: "PDFs, Doiciméid Oifige, agus íomhánna le sínithe digiteacha a shíniú"

  items:
    # feature loop
    - icon: "sign"
      title: "Ag Cur Sínithe"
      content: "Sínigh doiciméad ag baint úsáide as cineálacha éagsúla sínithe tacaithe trí shíniú digiteach a chur go beacht in aon áit ar aon leathanach."

    # feature loop
    - icon: "custom"
      title: "Torthaí a shaincheapadh"
      content: "Saincheap an chuma sínithe trí dath, cló, teorainn, rothlú agus gnéithe eile a choigeartú chun an toradh inmhianaithe a bhaint amach."

    # feature loop
    - icon: "password"
      title: "Doiciméid a dhaingniú le pasfhocal"
      content: "I gcás go leor cineálacha doiciméad tacaithe, is féidir leat an doiciméad sínithe a chosaint le pasfhocal."

    # feature loop
    - icon: "protect"
      title: "Cosc ar athruithe neamhúdaraithe"
      content: "Cosain doiciméid thábhachtacha gnó sínithe le deimhniú digiteach ó mhodhnuithe neamhúdaraithe."

    # feature loop
    - icon: "convert"
      title: "Torthaí a fháil sna formáidí inmhianaithe"
      content: "Faigh comhaid toraidh sínithe go héasca i bhformáid ar bith a dtacaítear léi. Is féidir leat doiciméid MS Word a thiontú go PDF freisin gan stró."

    # feature loop
    - icon: "preview"
      title: "Réamhamharc doiciméad"
      content: "Sábháil aon leathanach de dhoiciméad mar íomhá le próiseáil amach anseo."

    # feature loop
    - icon: "search"
      title: "Ag cuardach sínithe"
      content: "Is féidir faisnéis a fháil faoi shínithe a cuireadh leis roimhe seo i ndoiciméid ar leith."

    # feature loop
    - icon: "validate"
      title: "Doiciméid a bhailíochtú"
      content: "Bailíochtaigh cruinneas na sínithe ar aon doiciméad sínithe."

    # feature loop
    - icon: "update"
      title: "Sínithe a bhainistiú"
      content: "Nuair a chuirtear síniú ar leathanach doiciméid, is féidir é a scriosadh, a bhogadh nó a nuashonrú de réir mar is gá."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Cóid samplaí"
  description: "Úsáideann roinnt cásanna de ghnáth GroupDocs.Signature le haghaidh oibríochtaí Java"
  items:
    # code sample loop
    - title: "Enchance doiciméad PDF le QR-cód"
      content: |
        D’fhéadfadh sé a bheith luachmhar próisis ghnó a fheabhsú trí [QR-codes](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) a chur le leathanaigh ar leith de dhoiciméid PDF. Tá sampla de conas cód QR a chur leis ag baint úsáide as GroupDocs.Signature do Java.
        {{< landing/code title="Enchance doiciméad PDF le QR-cód">}}
        ```java {style=abap}
        // Íoslódáil an doiciméad le síniú
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Cruthaigh roghanna cód QR le téacs réamhshainithe
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Cumraigh cineál ionchódaithe cód QR agus suíomh ar an leathanach
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Sínigh an doiciméad agus sábháil é mar chomhad toraidh
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Úsáid síniú digiteach chun DOCX a chosaint"
      content: |
        Is féidir leat [Doiciméad a Chosaint](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) ag baint úsáide as sínithe pearsanta nó corparáideacha atá stóráilte mar dheimhnithe digiteacha. Ní féidir doiciméid atá daingnithe le teastas a athrú gan an síniú a chur ó bhail.
        {{< landing/code title="Úsáid síniú digiteach chun DOCX a chosaint">}}
        ```java {style=abap}   
        // Íoslódáil an doiciméad le síniú digiteach
        Signature signature = new Signature("file_to_sign.docx");
        
        // Sonraigh roghanna sínithe digiteacha agus cuir an cosán chuig an gcomhad teastais ar fáil
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Socraigh focal faire an teastais
        options.setPassword("1234567890");

        // Sínigh an doiciméad agus é a shábháil ar an cosán atá ag teastáil
        signature.sign("digitally_signed.docx", options);
        ```
        {{< /landing/code >}}

---
