---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:01
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
platform: "Net"
platform_tag: "net"

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
title: "Doiciméid a shíniú<br>via .NET API"
description: "Sínigh doiciméid agus íomhánna digiteacha ar aon ardán ag baint úsáide as ár n-APIanna solúbtha agus ár réitigh app-bhunaithe do ríomhchláraitheoirí agus úsáideoirí deiridh."
words:
  for: "le haghaidh"

actions:
  main: "Íoslódáil saor in aisce Nuga"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Ceadúnú"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Réidh le tosú?"
  description: "Bain triail as gnéithe GroupDocs.Signature saor in aisce nó iarr ceadúnas"

release:
  title: "Leagan {0} eisithe"
  notes: "Féach cad atá nua"
  downloads: "Íoslódálacha"

code:
  title: "Sínigh comhaid PDF i C #"
  more: "Tuilleadh samplaí"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Roghnaigh doiciméad PDF
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Cuir téacs ar fáil
        var options = new TextSignOptions("John Smith")
        {
            // Socraigh dath
            ForeColor = Color.Red
        };
        // Sínigh an doiciméad agus sábháil i gcomhad
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Forbhreathnú GroupDocs.Signature"
  description: "API chun doiciméid a shíniú agus oibríochtaí gaolmhara a dhéanamh in feidhmchláir .NET"
  features:
    # feature loop
    - title: "Sínithe á gcur le doiciméid ghnó in C#"
      content: "Síniú doiciméad: Le GroupDocs.Signature do .NET, is féidir leat cineálacha éagsúla sínithe, mar shampla téacs, íomhánna, barrachóid, agus deimhnithe digiteacha, a chur le doiciméid PDF agus Oifige. Ligeann an API seo duit do dhoiciméid a shíniú le beagnach aon chineál sonraí, meiteashonraí folaithe san áireamh."

    # feature loop
    - title: "Doiciméid sínithe a phróiseáil"
      content: "Próiseáil bhreise: Is féidir leat oibríochtaí cumhachtacha a dhéanamh ar dhoiciméid sínithe ag baint úsáide as GroupDocs.Signature. Áiríonn sé seo cuardach do shínithe atá ann cheana féin laistigh de dhoiciméid ghnó agus iad a fhíorú ag baint úsáide as critéir shonracha. Ina theannta sin, is féidir leat faisnéis doiciméad agus leathanaigh réamhamharc a aisghabháil tríd an API .NET seo."

    # feature loop
    - title: "Torthaí a shaincheapadh"
      content: "Cuireann GroupDocs.Signature le haghaidh .NET roghanna saincheaptha fairsinge ar fáil. Is féidir leat sínithe a shuíomh go beacht áit ar bith ar leathanach doiciméid agus a gcuma a choigeartú ag baint úsáide as socruithe éagsúla. Ina theannta sin, tacaíonn an API seo le doiciméid phróiseáilte a shábháil i raon leathan formáidí tacaithe."

############################# Platforms ############################
platforms:
  enable: true
  title: "Neamhspleáchas ardán"
  description: "Tacaíonn GroupDocs.Signature le haghaidh .NET leis na córais oibriúcháin, creataí agus bainisteoirí pacáiste seo a leanas"
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
    Tacaíonn GroupDocs.Signature le haghaidh .NET le hoibríochtaí leis na [formáidí comhaid](https://docs.groupdocs.com/signature/net/supported-document-formats/) seo a leanas.
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
  description: "PDFs, Doiciméid Oifige, agus Íomhánna a shíniú go tapa agus go cruinn"

  items:
    # feature loop
    - icon: "sign"
      title: "Síniú doiciméad"
      content: "Cuir síniú tacaithe amháin nó iolrach leis go cruinn ag aon suíomh sonraithe ar dhoiciméid ghnó."

    # feature loop
    - icon: "custom"
      title: "Saincheap sínithe"
      content: "Bain úsáid as gnéithe cosúil le dath, cló, teorainn, rothlú, etc., chun cuma sínithe a chumrú."

    # feature loop
    - icon: "password"
      title: "Cosaint do phasfhocal doiciméad"
      content: "Déan cineálacha áirithe doiciméad a dhaingniú trí phasfhocal a shocrú tar éis duit a shíniú."

    # feature loop
    - icon: "protect"
      title: "Cosaint ar athruithe"
      content: "Cosc a chur ar athruithe ar dhoiciméid ghnó tábhachtacha tar éis síniú a chur i gceangal le deimhniú digiteach."

    # feature loop
    - icon: "convert"
      title: "Tiontaigh comhaid sínithe go formáidí eile"
      content: "Tiontaigh comhaid sínithe go formáidí inmhianaithe, mar shampla doiciméad Word a shábháil mar PDF."

    # feature loop
    - icon: "preview"
      title: "Sliocht réamhamhairc leathanach"
      content: "Sliocht leathanaigh ó dhoiciméid sínithe mar íomhánna aonair le haghaidh próiseála amach anseo."

    # feature loop
    - icon: "search"
      title: "Cuardach sínithe i ndoiciméid"
      content: "Aisghabh faisnéis faoi shínithe a cuireadh leis roimhe seo i ndoiciméid ar leith."

    # feature loop
    - icon: "validate"
      title: "Doiciméid shínithe a bhailíochtú"
      content: "Fíoraigh síniú ceart doiciméad ag baint úsáide as gnéithe bailíochtaithe."

    # feature loop
    - icon: "update"
      title: "Nuashonraigh nó scrios sínithe"
      content: "Déan sínithe sonracha a athshuíomh go héasca ar leathanach, a dtéacs a mhodhnú, nó iad a scriosadh gan aon fhadhbanna."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Cóid samplaí"
  description: "Úsáideann roinnt cásanna de ghnáth GroupDocs.Signature le haghaidh oibríochtaí .NET"
  items:
    # code sample loop
    - title: "Cuir QR-cód le PDF"
      content: |
        Má chuirtear [QR-codes](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) le leathanaigh ar leith de dhoiciméid PDF, féadtar próisis ghnó a fheabhsú. Seo thíos sampla de conas cód QR a chur leis ag baint úsáide as GroupDocs.Signature.
        {{< landing/code title="Conas a cuir an cód QR i bhformáid pdf.">}}
        ```csharp {style=abap}
        // Íoslódáil an doiciméad le síniú
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Cruthaigh roghanna cód QR le téacs réamhshainithe
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Cumraigh cineál ionchódaithe cód QR agus suíomh ar an leathanach
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Sínigh an doiciméad agus sábháil é mar chomhad toraidh
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Doiciméad DOCX a chosaint ag baint úsáide as deimhniú digiteach"
      content: |
        Is féidir leat [Doiciméad a chosaint](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) ag baint úsáide as sínithe pearsanta nó corparáideacha atá stóráilte mar dheimhnithe digiteacha. Ní féidir doiciméid chosanta den sórt sin a mhodhnú gan an síniú a chur ó bhail.
        {{< landing/code title="Seo conas sláine doiciméad a chinntiú.">}}
        ```csharp {style=abap}   
        // Íoslódáil an doiciméad le síniú digiteach
        using (Signature signature = new Signature("file_to_sign.docx"))
        {
            // Sonraigh roghanna sínithe digiteacha agus cuir an cosán chuig an gcomhad teastais ar fáil
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Socraigh focal faire an teastais
                Password = "1234567890"
            };
            // Sínigh an doiciméad agus é a shábháil ar an cosán atá ag teastáil
            signature.Sign("digitally_signed.docx", options);
        }
        ```
        {{< /landing/code >}}

---
