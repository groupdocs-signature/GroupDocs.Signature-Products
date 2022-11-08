---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Pdf
productName: Java
lang: el
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Pdf for Java

############################# Head ############################
head_title: "Επαλήθευση των υπογραφών Digital για αρχεία Pdf μέσω Java"
head_description: "Χρησιμοποιήστε μόνο μερικές γραμμές κώδικα Java για να επαληθεύσετε τα έγγραφα Pdf και τις υπογραφές τους Digital."

############################# Header ############################
title: "Επαλήθευση υπογραφών Digital για αρχεία Pdf"
description: "Το API για το Java παρέχει την ευκαιρία να επαληθεύσετε τις υπογραφές Digital σε έγγραφα Pdf. Η επαλήθευση των ηλεκτρονικών υπογραφών στα έγγραφά σας Pdf μπορεί να πραγματοποιηθεί γρήγορα και εύκολα."
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
    title_left: "Πώς να επικυρώσετε τις υπογραφές Digital στο έγγραφό σας Pdf"
    content_left: |
        Το [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) περιλαμβάνει χρήσιμες λειτουργίες, όπως η επαλήθευση των υπογραφών Digital που τοποθετούνται σε έγγραφα Pdf. Χρησιμοποιήστε αυτήν την ευκαιρία χωρίς να εφαρμόσετε επιπλέον κώδικα.
        
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
                
        // Set up input Pdf file
        String filePath = "input.pdf";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        DigitalVerifyOptions options = new DigitalVerifyOptions();

        // Digital signature comment
        options.setComments("Approved");

        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2020, 12, 12));
        options.setSignDateTimeTo(new Date(2022, 12, 12));
                            
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
    title: "Υπογραφή με Digital υπογραφές Ζωντανή επίδειξη"
    content: |
       Προσθέστε διάφορες ηλεκτρονικές υπογραφές στο αρχείο Pdf αυτήν τη στιγμή, μεταβαίνοντας στον ιστότοπο [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Επαληθεύστε άλλες υπογραφές Digital χρησιμοποιώντας Java"
    content: |
        "Επαλήθευση ηλεκτρονικών υπογραφών που έχουν τοποθετηθεί σε διάφορα έγγραφα. Ελέγξτε την ποιότητα των υπογραφών στις δημοφιλείς μορφές αρχείων όπως αποκαλύπτεται παρακάτω."
    format: 
       
       
back_to_top:
    enable: true
---