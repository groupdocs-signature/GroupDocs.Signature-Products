---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Docm
productName: .NET
lang: ca
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Docm for C#

############################# Head ############################
head_title: "Suprimeix les signatures de Digital dels fitxers Docm mitjançant C#"
head_description: "L'eliminació de signatures específiques de Digital dels documents signats Docm es pot dur a terme fàcilment amb un codi .NET curt."

############################# Header ############################
title: "Elimineu les signatures de Digital que es col·loquen als fitxers Docm"
description: "Suprimeix diverses signatures de Digital dels documents Docm. L'eliminació de signatures Digital requereix un codi C# senzill."
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
    title: "Obteniu informació sobre les funcions de l'API de GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API ofereix moltes maneres de processar els vostres documents mitjançant signatures electròniques. Hi ha signatures digitals com textos, imatges, certificats digitals, codis de barres, codis QR, segells o metadades. Els clients tenen la possibilitat d'afegir, esborrar, actualitzar, verificar o cercar signatures digitals en PDF, documents MS Word, llibres de treball MS Excel, presentacions MS PowerPoint, fitxers Adobe Photoshop i diversos formats d'imatge. S'ofereixen un gran nombre de funcions i configuracions útils.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Com eliminar les signatures de Digital del vostre document Docm"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ofereix una funció útil per esborrar documents de Docm de signatures de Digital amb unes poques línies de codi.
        
        * En primer lloc, instanciïu l'objecte Signature passant el camí al vostre document com a paràmetre de constructor.
        * A continuació, creeu un objecte de signatura adequat i configureu el seu identificador únic.
        * Després d'això, invoqueu el mètode Delete passant l'objecte de signatura que s'ha d'eliminar.
        * Finalment, els resultats de l'operació del procés.

    title_right: "Requisits del sistema"
    content_right: |
        GroupDocs.Signature for .NET són compatibles amb totes les plataformes i sistemes operatius principals. Abans d'executar el codi següent, assegureu-vos que teniu els següents requisits previs instal·lats al vostre sistema.

        * Sistemes operatius: Microsoft Windows, Linux, MacOS
        * Entorns de desenvolupament: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Baixeu la darrera versió de GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Docm file
        string filePath = "input.docm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "a01e1940-997a-444b-89af-9309a2d559a5";

                // provide signature features to delete
                // set up particular signature id
                DigitalSignature signatureToDelete = new DigitalSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signant amb Digital signatures Demostració en directe"
    content: |
       Afegiu diverses signatures electròniques al fitxer Docm ara mateix visitant el lloc web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Suprimeix les teves signatures de Digital amb C#"
    content: |
        "Supressió de signatures electròniques que s'han afegit a diversos formats de documents. Elimina les signatures ràpidament sense codi addicional."
    format: 
       
       
back_to_top:
    enable: true
---