---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Metadata
fileformat: Tiff
productName: Java
lang: el
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Metadata signatures at Tiff with Java

############################# Head ############################
head_title: "Αναζήτηση για Metadata υπογραφές στο αρχείο Tiff στο Java"
head_description: "Χρησιμοποιήστε το Java για αναζήτηση υπογραφών Metadata σε αρχεία Tiff χρησιμοποιώντας μερικές γραμμές κώδικα."

############################# Header ############################
title: "Αναζητήστε υπογραφές Metadata στο αρχείο Tiff"
description: "Το εγγενές API του Java επιτρέπει την αναζήτηση για υπογραφές Metadata σε ήδη υπογεγραμμένα αρχεία Tiff. Εκτελέστε σύνθετη αναζήτηση ηλεκτρονικής υπογραφής στα έγγραφά σας Tiff χρησιμοποιώντας μερικές γραμμές κώδικα."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Σχετικά με το API GroupDocs.Signature for Java"
    content: |
        Το [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) παρέχει το API Java για την επεξεργασία εγγράφων χρησιμοποιώντας διάφορους τύπους υπογραφών, όπως κείμενα, εικόνες, ψηφιακά πιστοποιητικά, γραμμωτούς κώδικες, κωδικούς QR, σφραγίδες ή μεταδεδομένα. Οι χρήστες μπορούν να προσθέσουν, να διαγράψουν, να ενημερώσουν, να επαληθεύσουν ή να αναζητήσουν ηλεκτρονικές υπογραφές σε αρχεία PDF, έγγραφα MS Word, βιβλία εργασίας MS Excel, παρουσιάσεις MS PowerPoint, αρχεία Adobe Photoshop και διάφορες μορφές εικόνας, με πρόσθετη υποστήριξη για την προσαρμογή των ιδιοτήτων υπογραφών ανάλογα με τις ανάγκες.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Τρόπος αναζήτησης για υπογραφές Metadata στο Tiff"
    content_left: |
        Το [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) διευκολύνει τους προγραμματιστές του Java να αναζητήσουν υπογραφές Metadata σε αρχεία Tiff από τις εφαρμογές τους, εφαρμόζοντας μερικά εύκολα βήματα.
        
        * Δημιουργήστε μια νέα παρουσία κλάσης Signature και περάστε τη διαδρομή εγγράφου προέλευσης ως παράμετρο κατασκευής.
        * Δημιουργήστε το αντικείμενο SearchOptions σύμφωνα με τις απαιτήσεις σας και καθορίστε τις επιλογές αναζήτησης.
        * Καλέστε τη μέθοδο αναζήτησης της παρουσίας κλάσης Signature και περάστε το SearchOptions σε αυτήν.
        * Επεξεργαστείτε τα αποτελέσματα αναζήτησης ανάλογα με τις απαιτήσεις σας.

    title_right: "Απαιτήσεις συστήματος"
    content_right: |
        Το GroupDocs.Signature for Java υποστηρίζεται σε όλες τις μεγάλες πλατφόρμες και λειτουργικά συστήματα. Πριν εκτελέσετε τον παρακάτω κώδικα, βεβαιωθείτε ότι έχετε εγκαταστήσει τις ακόλουθες προϋποθέσεις στο σύστημά σας.

        * Λειτουργικά συστήματα: Microsoft Windows, Linux, MacOS
        * Περιβάλλοντα ανάπτυξης: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Κατεβάστε την πιο πρόσφατη έκδοση του GroupDocs.Signature for Java από το [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
        
        // Set up input Tiff file
        String filePath = "input.tiff";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // search for Metadata signatures in Tiff document
        List<ImageMetadataSignature> signatures = signature.search(ImageMetadataSignature.class, SignatureType.Metadata);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));


        ```

############################# Demos ############################
demos:
    enable: true
    title: "Αναζήτηση για Metadata ηλεκτρονικές υπογραφές Live Demo"
    content: |
       Αναζητήστε στο έγγραφο διάφορες ηλεκτρονικές υπογραφές σε αρχεία Tiff αυτήν τη στιγμή, μεταβαίνοντας στον ιστότοπο [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Αναζήτηση για άλλες υπογραφές Metadata χρησιμοποιώντας Java"
    content: |
        "Αναζήτηση ηλεκτρονικών υπογραφών σε διάφορα έγγραφα. Βρείτε υπογραφές από μια από τις δημοφιλείς μορφές αρχείων όπως φαίνεται παρακάτω."
    format: 
           
       
back_to_top:
    enable: true
---