---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Wmf
productName: Java
lang: el
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Wmf for Java

############################# Head ############################
head_title: "Προσθήκη ηλεκτρονικών υπογραφών μεταδεδομένων σε έγγραφα Wmf μέσω Java"
head_description: "Χρησιμοποιήστε τα Μεταδεδομένα ως κρυφές ηλεκτρονικές υπογραφές στα έγγραφά σας Wmf χρησιμοποιώντας μερικές γραμμές κώδικα Java. Χρησιμοποιήστε το GroupDocs Document Signature API για να υπογράψετε ηλεκτρονικά τα έγγραφα και τα αρχεία της επιχείρησής σας με πληροφορίες μεταδεδομένων."

############################# Header ############################
title: "Οι ηλεκτρονικές υπογραφές μεταδεδομένων για το έγγραφο Wmf μέσω του Java είναι απλές και εύκολες στη χρήση!"
description: "Ηλεκτρονικά υπογράψτε τα έγγραφα και τις συμβάσεις του Wmf με κρυφές καταχωρίσεις Μεταδεδομένων. Δημιουργήστε μεταδεδομένα για αρχεία PDF, έγγραφα MS Word, βιβλία εργασίας MS Excel, παρουσιάσεις MS PowerPoint και διάφορες μορφές εικόνας χωρίς προβλήματα και επιπλέον κωδικοποίηση."
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
    title: "Σχετικά με το API υπογραφών μεταδεδομένων GroupDocs.Signature for Java"
    content: |
        Το [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) είναι ένα δημοφιλές API για ηλεκτρονική υπογραφή ψηφιακών εγγράφων. Διατίθενται υπογραφές όπως κείμενα, εικόνες, ψηφιακά πιστοποιητικά, γραμμικοί κώδικες, κωδικοί QR, σφραγίδες ή μεταδεδομένα. Οι υπογραφές ενδέχεται να τοποθετηθούν σε αρχεία PDF, έγγραφα MS Word, βιβλία εργασίας MS Excel, παρουσιάσεις MS PowerPoint, αρχεία Adobe Photoshop και διάφορες μορφές εικόνας. Οι πελάτες μπορούν να υπογράψουν το έγγραφό τους και να ενημερώσουν, να αναζητήσουν, να επαληθεύσουν, να διαγράψουν ή να κάνουν προεπισκόπηση των ηλεκτρονικών υπογραφών που είχαν τοποθετηθεί σε αυτά τα έγγραφα. Επιπλέον, παρέχονται πολλές δυνατότητες για προσαρμογή υπογραφών.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Βήματα για την υπογραφή Wmf με Metadata στο Java"
    content_left: |
        Το [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) παρέχει τη δυνατότητα υπογραφής εγγράφων Wmf με υπογραφές Metadata γρήγορα και εύκολα.
        
        * Δημιουργήστε ένα στιγμιότυπο κλάσης υπογραφής που παρέχει αρχείο Wmf που υποτίθεται ότι υπογράφεται ως διαδρομή ή ροή μνήμης
        * Δημιουργήστε την κλάση SignOptions και ορίστε όλα τα απαιτούμενα δεδομένα.
        * Επικαλέστε τη μέθοδο Signature.Sign() μεταβιβάζοντας την έξοδο Wmf αρχείο ή ροή μνήμης

    title_right: " Απαιτήσεις συστήματος"
    content_right: |
        Το GroupDocs.Signature for Java υποστηρίζεται σε όλες τις μεγάλες πλατφόρμες και λειτουργικά συστήματα. Πριν εκτελέσετε τον παρακάτω κώδικα, βεβαιωθείτε ότι έχετε εγκαταστήσει τις ακόλουθες προϋποθέσεις στο σύστημά σας.

        * Λειτουργικά συστήματα: Microsoft Windows, Linux, MacOS
        * Περιβάλλοντα ανάπτυξης: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Αποκτήστε το πιο πρόσφατο GroupDocs.Signature for Java από το [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Wmf file
        String filePath = "input.wmf";
        // Set up output file
        String outputFilePath = "output.wmf";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // Specify different Metadata Signatures and add them to options signature collection
        // set start id
        int imgsMetadataId = 41996;
        // setup int value
        ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
        options.getSignatures().add(mdSign_DocId);
        // setup Author property
        ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
        options.getSignatures().add(mdSign_Author);
        // setup data of sign date
        ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, new Date()); // DateTime
        options.getSignatures().add(mdSign_Date);
        // setup double
        ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456); //decimal value
        options.getSignatures().add(mdSign_Amnt);

        // sign Wmf document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Υπογραφή εγγράφων Wmf με Metadata Ζωντανή επίδειξη"
    content: |
       Υπογράψτε το αρχείο Wmf με διάφορες υπογραφές αυτήν τη στιγμή, μεταβαίνοντας στον ιστότοπο [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Δωρεάν online demo σας περιμένει.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Άλλες υποστηριζόμενες υπογραφές Metadata για Java"
    content: |
        "Μπορείτε επίσης να υπογράψετε το Wmf με άλλους τύπους υπογραφής. Δείτε την παρακάτω λίστα."
    format: 
       
       
back_to_top:
    enable: true
---