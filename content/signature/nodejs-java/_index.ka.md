---
############################# Static ############################
layout: "landing"
date: 2024-03-04T17:52:03
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: ka
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
head_title: ".NET, Java, Cloud API და ონლაინ დოკუმენტის ხელმოწერის აპები"
head_description: "მიიღეთ ერთში დოკუმენტის ელექტრონული ხელმოწერის გადაწყვეტა .NET, Java და ღრუბელზე დაფუძნებული აპლიკაციებისთვის. ხელი მოაწერეთ დოკუმენტების საერთო ფორმატებს ინტერნეტით მარტივი გადაადგილების ფუნქციის გამოყენებით"

############################# Header ############################
title: "მოაწერეთ დოკუმენტები<br>Node.js API-ით"
description: "მოაწერეთ ციფრული დოკუმენტები და სურათები ნებისმიერ პლატფორმაზე ჩვენი მოქნილი API-ების და აპებზე დაფუძნებული გადაწყვეტილებების გამოყენებით პროგრამისტებისა და საბოლოო მომხმარებლებისთვის."
words:
  for: "ამისთვის"

actions:
  main: "ჩამოტვირთეთ NPM-დან"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "ლიცენზირება"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "მზად ხართ დასაწყებად?"
  description: "სცადეთ GroupDocs.Signature ფუნქციები უფასოდ ან მოითხოვეთ ლიცენზია"

release:
  title: "ვერსია {0} გამოვიდა"
  notes: "ნახეთ რა არის ახალი"
  downloads: "ჩამოტვირთვები"

code:
  title: "PDF-ების ხელმოწერა Node.js-ის მიერ"
  more: "მეტი მაგალითები"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```javascript {style=abap}   
    // აირჩიეთ PDF დოკუმენტი
    let signature = new Signature("sample.pdf");
    
    // მიაწოდეთ ტექსტი
    let options = new TextSignOptions("John Smith");
    
    // დააყენეთ ფერი
    options.ForeColor = Color.Red;
    
    // ხელი მოაწერეთ დოკუმენტს და შეინახეთ ფაილში
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature მიმოხილვა"
  description: "დოკუმენტების ხელმოწერის ბიბლიოთეკა, რომელიც მზად არის Node.js აპლიკაციებში გამოსაყენებლად"
  features:
    # feature loop
    - title: "ციფრული ხელმოწერების გადაწყვეტა ბიზნეს დოკუმენტებისთვის Node.js-ით"
      content: "GroupDocs.Signature for Node.js via Java გთავაზობთ ციფრული ხელმოწერის ვარიანტების ყოვლისმომცველ კომპლექტს PDF, Office დოკუმენტებისა და სურათებისთვის. ხელმისაწვდომია ტექსტი, შტრიხკოდები, სურათები, ციფრული სერთიფიკატები და მეტამონაცემები. დოკუმენტების გამარტივებული დამუშავება უზრუნველყოფს ეფექტურობას."

    # feature loop
    - title: "ხელმოწერილი დოკუმენტების გაფართოებული მანიპულირება"
      content: "GroupDocs.Signature გაძლევთ უფლებას, დაამუშავოთ ხელმოწერილი დოკუმენტები. მოძებნეთ და შეამოწმეთ ხელმოწერები სხვადასხვა კრიტერიუმების გამოყენებით. გარდა ამისა, ამოიღეთ დეტალური დოკუმენტის ინფორმაცია ან შექმენით გვერდების გადახედვის სურათები."

    # feature loop
    - title: "სხვადასხვა გამომავალი ფორმატები"
      content: "ჩვენი გადაწყვეტა უზრუნველყოფს ხელმოწერილი დოკუმენტების გამომავალი ფორმატის ფართო კონტროლს. ზუსტად განათავსეთ ხელმოწერები ნებისმიერ გვერდზე და შეცვალეთ მათი გარეგნობა. შეინახეთ ხელმოწერილი დოკუმენტები მრავალ მხარდაჭერილ ფორმატში და სურვილისამებრ დაიცავით ისინი პაროლებით."

############################# Platforms ############################
platforms:
  enable: true
  title: "პლატფორმის დამოუკიდებლობა"
  description: "GroupDocs.Signature for Node.js via Java ახორციელებს დოკუმენტების დამუშავებას სხვადასხვა ოპერაციული სისტემებით"
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
  title: "მხარდაჭერილი ფაილის ფორმატები"
  description: |
    GroupDocs.Signature for Node.js via Java აადვილებს ოპერაციებს [ფაილის პოპულარული ფორმატები](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office ფორმატები
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### სურათები და სხვა ფორმატები
        * **პორტატული:** PDF
        * **სურათები:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **სხვა საოფისე ფორმატები:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### სხვა ფორმატები
        * **ვებ:** HTML, MHTML
        * **არქივები:** ZIP, TAR, 7Z
        * **სერთიფიკატები:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Signature-ის მახასიათებლები"
  description: "ხელი მოაწერეთ PDF-ებს, ოფისის დოკუმენტებს და სურათებს ციფრული ხელმოწერებით"

  items:
    # feature loop
    - icon: "sign"
      title: "ბიზნეს ხელმოწერები"
      content: "გამოიყენეთ სხვადასხვა სახის ხელმოწერები დოკუმენტების ხელმოწერისთვის. განათავსეთ ციფრული ხელმოწერები ზუსტად ნებისმიერ გვერდზე."

    # feature loop
    - icon: "custom"
      title: "ხელმოწერის გარეგნობის მორგება"
      content: "მოარგეთ ხელმოწერების ვიზუალური ასპექტები ფერის, შრიფტის, საზღვრების, როტაციის და სხვათა მორგებით სასურველი შედეგის მისაღწევად."

    # feature loop
    - icon: "password"
      title: "პაროლით დაცული დოკუმენტები"
      content: "მრავალი მხარდაჭერილი დოკუმენტის ფორმატებისთვის, დაიცავით ხელმოწერილი დოკუმენტები პაროლით დამატებითი უსაფრთხოებისთვის."

    # feature loop
    - icon: "protect"
      title: "არასანქცირებული ცვლილებების პრევენცია"
      content: "დაიცავით ციფრული სერთიფიკატებით ხელმოწერილი მნიშვნელოვანი ბიზნეს დოკუმენტები არაავტორიზებული ცვლილებებისგან."

    # feature loop
    - icon: "convert"
      title: "სასურველი გამომავალი ფორმატები"
      content: "უპრობლემოდ მიიღეთ ხელმოწერილი დოკუმენტები ნებისმიერი მხარდაჭერილი ფორმატით. მარტივად გადააკეთეთ MS Word დოკუმენტები PDF ფორმატში."

    # feature loop
    - icon: "preview"
      title: "დოკუმენტების გადახედვა"
      content: "შეინახეთ ინდივიდუალური დოკუმენტის გვერდები სურათებად მომავალი საჭიროებისთვის."

    # feature loop
    - icon: "search"
      title: "ხელმოწერის ძებნა"
      content: "მიიღეთ ინფორმაცია ადრე დამატებული ხელმოწერების შესახებ თქვენს დოკუმენტებში."

    # feature loop
    - icon: "validate"
      title: "დოკუმენტის დადასტურება"
      content: "შეამოწმეთ ნებისმიერ დოკუმენტში წარმოდგენილი ხელმოწერების ავთენტურობა."

    # feature loop
    - icon: "update"
      title: "ხელმოწერის მენეჯმენტი"
      content: "წაშალეთ, გადაიტანეთ ან შეცვალეთ ნებისმიერი ხელმოწერა, რომელიც განთავსებულია დოკუმენტის ნებისმიერ გვერდზე."

############################# Code samples ############################
code_samples:
  enable: true
  title: "კოდის ნიმუშები"
  description: "საილუსტრაციო მაგალითები, რომლებიც ასახავს ტიპიურ GroupDocs.Signature for Node.js via Java ოპერაციებს"
  items:
    # code sample loop
    - title: "მონიშნეთ PDF QR კოდებით"
      content: |
        [შტრიხკოდების](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) კონკრეტულ PDF დოკუმენტის გვერდებში ჩართვისას შეუძლია ბიზნეს პროცესების გამარტივება. ამ განყოფილებაში მოცემულია QR კოდის დამატების მაგალითი GroupDocs.Signature for Node.js via Java-ის გამოყენებით.
        {{< landing/code title="როგორ ჩავდოთ QR კოდი PDF-ში.">}}
        ```javascript {style=abap}
        // ჩატვირთეთ დოკუმენტი ხელმოწერისთვის
        let signature = new Signature("file_to_sign.pdf");
        
        // შექმენით QR კოდის ვარიანტები წინასწარ განსაზღვრული ტექსტით
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // დააკონფიგურირეთ QR კოდის კოდირების ტიპი და პოზიცია გვერდზე
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // მოაწერეთ ხელი დოკუმენტს და შეინახეთ შედეგის ფაილად
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX-ის დაცვა ციფრული ხელმოწერით"
      content: |
        [დაიცავით თქვენი დოკუმენტები](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) ციფრული სერთიფიკატების საფუძველზე ხელმოწერებით. ციფრული ხელმოწერა იცავს თქვენს ბიზნეს დოკუმენტებს შინაარსის ცვლილებისგან.
        {{< landing/code title="აქ მოცემულია, თუ როგორ უნდა უზრუნველყოთ დოკუმენტის მთლიანობა.">}}
        ```javascript {style=abap}   
        // ჩატვირთეთ დოკუმენტი ციფრული ხელმოწერისთვის
        let signature = new Signature("file_to_sign.pdf");
        
        // მიუთითეთ ციფრული ხელმოწერის ვარიანტები და მიუთითეთ გზა სერტიფიკატის ფაილამდე
        let options = new DigitalSignOptions("certificate.pfx");

        // დააყენეთ სერტიფიკატის პაროლი
        options.Password = "1234567890";

        // ხელი მოაწერეთ დოკუმენტს და შეინახეთ სასურველ გზაზე
        signature.Sign("digitally_signed.pdf", options);

        ```
        {{< /landing/code >}}

---
