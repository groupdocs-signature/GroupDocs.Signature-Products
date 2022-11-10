---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Xls
productName: Java
lang: ka
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xls for Java

############################# Head ############################
head_title: "წაშალეთ Digital ხელმოწერა Xls ფაილებიდან Java-ით"
head_description: "კონკრეტული Digital ხელმოწერების წაშლა ხელმოწერილი Xls დოკუმენტებიდან შეიძლება მარტივად განხორციელდეს მოკლე Java კოდით."

############################# Header ############################
title: "წაშალეთ Digital ხელმოწერები, რომლებიც განთავსებულია Xls ფაილში"
description: "წაშალეთ სხვადასხვა Digital ხელმოწერა Xls დოკუმენტებიდან. Digital ხელმოწერის ამოღებას სჭირდება მარტივი Java კოდი."
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
    title: "მიიღეთ ინფორმაცია GroupDocs.Signature for Java API ფუნქციების შესახებ"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API გთავაზობთ მრავალ გზას თქვენი დოკუმენტების ელექტრონული ხელმოწერების გამოყენებით დასამუშავებლად. ხელმისაწვდომია ციფრული ხელმოწერები, როგორიცაა ტექსტები, სურათები, ციფრული სერთიფიკატები, შტრიხკოდები, QR-კოდები, შტამპები ან მეტამონაცემები. მომხმარებელს აქვს შესაძლებლობა დაამატონ, წაშალონ, განაახლონ, გადაამოწმონ ან მოძებნონ ციფრული ხელმოწერები PDF-ებში, MS Word დოკუმენტებში, MS Excel სამუშაო წიგნებში, MS PowerPoint პრეზენტაციებში, Adobe Photoshop ფაილებსა და გამოსახულების სხვადასხვა ფორმატებში. მოწოდებულია სასარგებლო ფუნქციების და პარამეტრების დიდი რაოდენობა.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "როგორ ამოიღოთ Digital ხელმოწერა თქვენი Xls დოკუმენტიდან"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) გთავაზობთ სასარგებლო ფუნქციას Xls დოკუმენტების Digital ხელმოწერების გასასუფთავებლად რამდენიმე სტრიქონის კოდით.
        
        * უპირველეს ყოვლისა, შექმენით ხელმოწერის ობიექტი, რომელიც გადადის თქვენს დოკუმენტში, როგორც კონსტრუქტორის პარამეტრი.
        * შემდეგ შექმენით შესაბამისი ხელმოწერის ობიექტი და დააყენეთ მისი უნიკალური იდენტიფიკატორი.
        * ამის შემდეგ, გამოიძახეთ Delete მეთოდი, რომელიც გადასცემს ხელმოწერის ობიექტს, რომელიც უნდა წაიშალოს.
        * საბოლოოდ, დაამუშავეთ ოპერაციის შედეგები.

    title_right: "სისტემის მოთხოვნები"
    content_right: |
        GroupDocs.Signature for Java მხარდაჭერილია ყველა ძირითად პლატფორმაზე და ოპერაციულ სისტემაზე. ქვემოთ მოცემული კოდის შესრულებამდე, დარწმუნდით, რომ თქვენს სისტემაში დაინსტალირებული გაქვთ შემდეგი წინაპირობები.

        * ოპერაციული სისტემები: Microsoft Windows, Linux, MacOS
        * განვითარების გარემო: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * ჩამოტვირთეთ GroupDocs.Signature for Java-ის უახლესი ვერსია [Maven]-დან (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xls file
        String filePath = "input.xls";
        // Set up output file
        String outputFilePath = "output.xls";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "a01e1940-997a-444b-89af-9309a2d559a5";

        // provide signature item to delete
        DigitalSignature signatureToDelete = new DigitalSignature(id);

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
    title: "ხელმოწერა Digital ხელმოწერებით Live Demo"
    content: |
       დაამატეთ სხვადასხვა ელექტრონული ხელმოწერები Xls ფაილს ახლავე, ეწვიეთ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ვებსაიტს.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "წაშალეთ თქვენი Digital ხელმოწერები Java-ით"
    content: |
        "ელექტრონული ხელმოწერების წაშლა, რომლებიც დაემატა სხვადასხვა დოკუმენტის ფორმატებს. სწრაფად ამოიღეთ ხელმოწერები დამატებითი კოდის გარეშე."
    format: 
       
       
back_to_top:
    enable: true
---