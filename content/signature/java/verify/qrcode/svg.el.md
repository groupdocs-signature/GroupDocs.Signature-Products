---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Svg
productName: Java
lang: el
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Svg for Java

############################# Head ############################
head_title: "Επαλήθευση των υπογραφών Qrcode για αρχεία Svg μέσω Java"
head_description: "Χρησιμοποιήστε μόνο μερικές γραμμές κώδικα Java για να επαληθεύσετε τα έγγραφα Svg και τις υπογραφές τους Qrcode."

############################# Header ############################
title: "Επαλήθευση υπογραφών Qrcode για αρχεία Svg"
description: "Το API για το Java παρέχει την ευκαιρία να επαληθεύσετε τις υπογραφές Qrcode σε έγγραφα Svg. Η επαλήθευση των ηλεκτρονικών υπογραφών στα έγγραφά σας {{Μορφή αρχείου}} μπορεί να πραγματοποιηθεί γρήγορα και εύκολα."
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
    title: "Ανακαλύψτε νέες δυνατότητες API του GroupDocs.Signature for Java"
    content: |
        Το [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API παρέχει ευρύ φάσμα τρόπων επεξεργασίας πολλών μορφών εγγράφων χρησιμοποιώντας ηλεκτρονικές υπογραφές. Υποστηρίζονται πολλοί τύποι ψηφιακών υπογραφών όπως κείμενα, εικόνες, ψηφιακά πιστοποιητικά, barcodes, QR-codes, γραμματόσημα ή μεταδεδομένα. Οι πελάτες μπορούν να προσθέσουν, να αφαιρέσουν, να επεξεργαστούν, να επικυρώσουν ή να αναζητήσουν ψηφιακές υπογραφές σε PDF, έγγραφα MS Word, βιβλία εργασίας MS Excel, παρουσιάσεις MS PowerPoint, αρχεία Adobe Photoshop και διάφορες μορφές εικόνας. Διατίθεται εκπληκτικός αριθμός πρόσθετων λειτουργιών και ρυθμίσεων.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Πώς να επικυρώσετε τις υπογραφές Qrcode στο έγγραφό σας Svg"
    content_left: |
        Το [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) περιλαμβάνει χρήσιμες λειτουργίες, όπως η επαλήθευση των υπογραφών Qrcode που τοποθετούνται σε έγγραφα Svg. Χρησιμοποιήστε αυτήν την ευκαιρία χωρίς να εφαρμόσετε επιπλέον κώδικα.
        
        * Πρώτον, δημιουργήστε την κλάση Signature που παρέχει ως διαδρομή παραμέτρου κατασκευαστή σε ένα έγγραφο που υποτίθεται ότι πρέπει να επαληθευτεί.
        * Δεύτερον, δημιουργήστε ένα νέο αντικείμενο VerifyOptions και ρυθμίστε όλες τις απαιτούμενες ιδιότητες.
        * Τέλος, επικαλέστε τη μέθοδο Verify του αντικειμένου της υπογραφής περνώντας την παρουσία VerifyOptions.
        * Στη συνέχεια, επεξεργαστείτε τα αποτελέσματα επαλήθευσης.

    title_right: "Απαιτήσεις συστήματος"
    content_right: |
        Το GroupDocs.Signature for Java υποστηρίζεται σε όλες τις μεγάλες πλατφόρμες και λειτουργικά συστήματα. Πριν εκτελέσετε τον παρακάτω κώδικα, βεβαιωθείτε ότι έχετε εγκαταστήσει τις ακόλουθες προϋποθέσεις στο σύστημά σας.

        * Λειτουργικά συστήματα: Microsoft Windows, Linux, MacOS
        * Περιβάλλοντα ανάπτυξης: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Κατεβάστε την πιο πρόσφατη έκδοση του GroupDocs.Signature for Java από το [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Svg file
        String filePath = "input.svg";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        QrCodeVerifyOptions options = new QrCodeVerifyOptions();

        // process only first page
        options.setPagesSetup(new PagesSetup());
        options.setPageNumber(1);
        options.setAllPages(false);
        // specify text match type
        options.setMatchType(TextMatchType.StartsWith);
        // specify text pattern to search
        options.setText("QrCode text");
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Υπογραφή με Qrcode υπογραφές Ζωντανή επίδειξη"
    content: |
       Προσθέστε διάφορες ηλεκτρονικές υπογραφές στο αρχείο Svg αυτήν τη στιγμή, μεταβαίνοντας στον ιστότοπο [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Επαληθεύστε άλλες υπογραφές Qrcode χρησιμοποιώντας Java"
    content: |
        "Επαλήθευση ηλεκτρονικών υπογραφών που έχουν τοποθετηθεί σε διάφορα έγγραφα. Ελέγξτε την ποιότητα των υπογραφών στις δημοφιλείς μορφές αρχείων όπως αποκαλύπτεται παρακάτω."
    format: 
       
       
back_to_top:
    enable: true
---