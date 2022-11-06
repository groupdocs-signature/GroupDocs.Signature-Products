---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Text
fileformat: Xls
productName: Java
lang: el
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Xls for Java

############################# Head ############################
head_title: "Διαγραφή υπογραφών Text από αρχεία Xls μέσω Java"
head_description: "Η διαγραφή συγκεκριμένων υπογραφών Text από υπογεγραμμένα έγγραφα Xls μπορεί να πραγματοποιηθεί εύκολα με σύντομο κωδικό Java."

############################# Header ############################
title: "Καταργήστε τις υπογραφές Text που τοποθετούνται σε αρχεία Xls"
description: "Διαγράψτε διάφορες υπογραφές Text από έγγραφα Xls. Η κατάργηση υπογραφών Text απαιτεί απλό κώδικα Java."
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
    title: "Λάβετε πληροφορίες σχετικά με τις λειτουργίες API του GroupDocs.Signature for Java"
    content: |
        Το [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API παρέχει πολλούς τρόπους επεξεργασίας των εγγράφων σας χρησιμοποιώντας ηλεκτρονικές υπογραφές. Διατίθενται ψηφιακές υπογραφές όπως κείμενα, εικόνες, ψηφιακά πιστοποιητικά, γραμμικοί κώδικες, κωδικοί QR, σφραγίδες ή μεταδεδομένα. Οι πελάτες έχουν τη δυνατότητα να προσθέσουν, να διαγράψουν, να ενημερώσουν, να επαληθεύσουν ή να αναζητήσουν ψηφιακές υπογραφές σε PDF, έγγραφα MS Word, βιβλία εργασίας MS Excel, παρουσιάσεις MS PowerPoint, αρχεία Adobe Photoshop και διάφορες μορφές εικόνας. Παρέχεται ένας τεράστιος αριθμός χρήσιμων λειτουργιών και ρυθμίσεων.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Πώς να αφαιρέσετε τις υπογραφές Text από το έγγραφό σας Xls"
    content_left: |
        Το [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) παρέχει χρήσιμη δυνατότητα για τη διαγραφή εγγράφων Xls από υπογραφές Text με μερικές γραμμές κώδικα.
        
        * Αρχικά, δημιουργήστε τη διαδρομή διέλευσης αντικειμένου υπογραφής στο έγγραφό σας ως παράμετρος κατασκευής.
        * Στη συνέχεια, δημιουργήστε ένα κατάλληλο αντικείμενο υπογραφής και ορίστε το μοναδικό του αναγνωριστικό.
        * Μετά από αυτό, καλέστε τη μέθοδο Διαγραφής μεταβιβάζοντας το αντικείμενο υπογραφής που πρέπει να διαγραφεί.
        * Τέλος, τα αποτελέσματα της λειτουργίας της διαδικασίας.

    title_right: "Απαιτήσεις συστήματος"
    content_right: |
        Το GroupDocs.Signature for Java υποστηρίζεται σε όλες τις μεγάλες πλατφόρμες και λειτουργικά συστήματα. Πριν εκτελέσετε τον παρακάτω κώδικα, βεβαιωθείτε ότι έχετε εγκαταστήσει τις ακόλουθες προϋποθέσεις στο σύστημά σας.

        * Λειτουργικά συστήματα: Microsoft Windows, Linux, MacOS
        * Περιβάλλοντα ανάπτυξης: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Κατεβάστε την πιο πρόσφατη έκδοση του GroupDocs.Signature for Java από το [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
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
        String id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

        // provide signature features to delete
        TextSignature signatureToDelete = new TextSignature(id);

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
    title: "Υπογραφή με Text υπογραφές Ζωντανή επίδειξη"
    content: |
       Προσθέστε διάφορες ηλεκτρονικές υπογραφές στο αρχείο Xls αυτήν τη στιγμή, μεταβαίνοντας στον ιστότοπο [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Διαγράψτε τις υπογραφές σας Text με το Java"
    content: |
        "Διαγραφή ηλεκτρονικών υπογραφών που προστέθηκαν σε διάφορες μορφές εγγράφων. Αφαιρέστε τις υπογραφές γρήγορα χωρίς επιπλέον κωδικό."
    format: 
       
       
back_to_top:
    enable: true
---