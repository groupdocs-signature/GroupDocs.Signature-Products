---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Odt
productName: .NET
lang: ga
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Odt for C#

############################# Head ############################
head_title: "Sínithe leictreonacha digiteacha á gcur le comhad Odt le C#"
head_description: "Cuir Síniú Digiteach ar chomhad Odt le haghaidh .NET ag baint úsáide as cúpla líne de chód. Úsáid an GroupDocs Document Signature API chun mórán formáidí comhaid a shíniú."

############################# Header ############################
title: "eSínigh Odt comhaid le Digital sínithe in C#"
description: "Conas Digital síniú a chur leis le cúpla líne de chód .NET"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Maidir le GroupDocs.Signature for .NET API sínithe digiteacha"
    content: |
        Is API coitianta é [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) chun doiciméid a bhfuil sínithe leictreonacha digiteacha orthu a shíniú, agus teastais dhigiteacha orthu. Le haghaidh sínithe digiteacha úsáideann API comhaid teastais PFX chun doiciméad a shíniú le heochracha príobháideacha agus poiblí cosanta ag pasfhocal. Féadfar na sínithe Digiteacha a úsáid chun doiciméid ghnó a dheimhniú le leathanach áirithe eSign PDF, chun doiciméid iomlána Microsoft Office a dheimhniú mar Words, Excel, comhaid Powerpoint, agus doiciméid Open Office. Is féidir le custaiméirí na sínithe a ionramháil go héasca ar nós eagarthóireacht a dhéanamh orthu, iad a bhaint nó a choigeartú. Soláthraíonn an API bealach chun sínithe a chuardach agus a fhíorú. Thairis sin, soláthraítear go leor cumais le haghaidh saincheapadh sínithe.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Céimeanna chun Odt a shíniú le Digital in C#"
    content_left: |
        Soláthraíonn [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) cumas chun doiciméid Odt a shíniú le sínithe Digital go tapa agus go héasca.
        
        * Cruthaigh sampla d'aicme Sínithe ag soláthar Odt comhad atá ceaptha a shíniú mar chonair nó mar shruth cuimhne
        * Cuir rang SignOptions ar bun agus socraigh na sonraí go léir a éilítear.
        * Iarr ar an modh Signature.Sign() aschuir Odt comhad nó sruth cuimhne a rith

    title_right: " Riachtanais Chórais"
    content_right: |
        Tacaítear le GroupDocs.Signature for .NET ar gach mór-ardán agus córas oibriúcháin. Sula ndéanann tú an cód thíos, déan cinnte go bhfuil na réamhriachtanais seo a leanas suiteáilte ar do chóras.

        * Córais oibriúcháin: Microsoft Windows, Linux, MacOS
        * Timpeallachtaí forbartha: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Faigh an GroupDocs.Signature for .NET is déanaí ó [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Odt file
        string filePath = "input.odt";
        // Set up output file
        string outputFilePath = "output.odt";
        // Provide digital certificate
        string certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                DigitalSignOptions options = new DigitalSignOptions(certificateFilePath)
                {
                    // set certificate password
                    Password = "1234567890",
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Odt document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ag síniú Odt doiciméad le Digital Taispeántas Beo"
    content: |
       Sínigh Odt comhad le sínithe éagsúla faoi láthair trí chuairt a thabhairt ar an suíomh Gréasáin [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Saor in aisce taispeána ar líne ag fanacht leat.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Sínithe Digital eile a dtacaítear leo le haghaidh C#"
    content: |
        "Is féidir leat Odt a shíniú le cineálacha sínithe eile freisin. Féach ar an liosta thíos le do thoil."
    format: 
       
       
back_to_top:
    enable: true
---