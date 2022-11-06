---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Dotx
productName: .NET
lang: el
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Dotx for C#

############################# Head ############################
head_title: "Προσθήκη ηλεκτρονικών υπογραφών μεταδεδομένων σε έγγραφα Dotx μέσω C#"
head_description: "Χρησιμοποιήστε τα Μεταδεδομένα ως κρυφές ηλεκτρονικές υπογραφές στα έγγραφά σας Dotx χρησιμοποιώντας μερικές γραμμές κώδικα C#. Χρησιμοποιήστε το GroupDocs Document Signature API για να υπογράψετε ηλεκτρονικά τα έγγραφα και τα αρχεία της επιχείρησής σας με πληροφορίες μεταδεδομένων."

############################# Header ############################
title: "Οι ηλεκτρονικές υπογραφές μεταδεδομένων για το έγγραφο Dotx μέσω του .NET είναι απλές και εύκολες στη χρήση!"
description: "Ηλεκτρονικά υπογράψτε τα έγγραφα και τις συμβάσεις του Dotx με κρυφές καταχωρίσεις Μεταδεδομένων. Δημιουργήστε μεταδεδομένα για αρχεία PDF, έγγραφα MS Word, βιβλία εργασίας MS Excel, παρουσιάσεις MS PowerPoint και διάφορες μορφές εικόνας χωρίς προβλήματα και επιπλέον κωδικοποίηση."
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
    title: "Σχετικά με το API υπογραφών μεταδεδομένων GroupDocs.Signature for .NET"
    content: |
        Το [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) είναι ένα δημοφιλές API για ηλεκτρονική υπογραφή ψηφιακών εγγράφων. Διατίθενται υπογραφές όπως κείμενα, εικόνες, ψηφιακά πιστοποιητικά, γραμμικοί κώδικες, κωδικοί QR, σφραγίδες ή μεταδεδομένα. Οι υπογραφές ενδέχεται να τοποθετηθούν σε αρχεία PDF, έγγραφα MS Word, βιβλία εργασίας MS Excel, παρουσιάσεις MS PowerPoint, αρχεία Adobe Photoshop και διάφορες μορφές εικόνας. Οι πελάτες μπορούν να υπογράψουν το έγγραφό τους και να ενημερώσουν, να αναζητήσουν, να επαληθεύσουν, να διαγράψουν ή να κάνουν προεπισκόπηση των ηλεκτρονικών υπογραφών που είχαν τοποθετηθεί σε αυτά τα έγγραφα. Επιπλέον, παρέχονται πολλές δυνατότητες για προσαρμογή υπογραφών.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Βήματα για την υπογραφή Dotx με Metadata στο C#"
    content_left: |
        Το [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) παρέχει τη δυνατότητα υπογραφής εγγράφων Dotx με υπογραφές Metadata γρήγορα και εύκολα.
        
        * Δημιουργήστε ένα στιγμιότυπο κλάσης υπογραφής που παρέχει αρχείο Dotx που υποτίθεται ότι υπογράφεται ως διαδρομή ή ροή μνήμης
        * Δημιουργήστε την κλάση SignOptions και ορίστε όλα τα απαιτούμενα δεδομένα.
        * Επικαλέστε τη μέθοδο Signature.Sign() μεταβιβάζοντας την έξοδο Dotx αρχείο ή ροή μνήμης

    title_right: " Απαιτήσεις συστήματος"
    content_right: |
        Το GroupDocs.Signature for .NET υποστηρίζεται σε όλες τις μεγάλες πλατφόρμες και λειτουργικά συστήματα. Πριν εκτελέσετε τον παρακάτω κώδικα, βεβαιωθείτε ότι έχετε εγκαταστήσει τις ακόλουθες προϋποθέσεις στο σύστημά σας.

        * Λειτουργικά συστήματα: Microsoft Windows, Linux, MacOS
        * Περιβάλλοντα ανάπτυξης: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Αποκτήστε το πιο πρόσφατο GroupDocs.Signature for .NET από το [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Dotx file
        string filePath = "input.dotx";
        // Set up output file
        string outputFilePath = "output.dotx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                WordProcessingMetadataSignature mdSign_Author = new WordProcessingMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                WordProcessingMetadataSignature mdSign_DocData = new WordProcessingMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                WordProcessingMetadataSignature mdSign_DocId = new WordProcessingMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Dotx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Υπογραφή εγγράφων Dotx με Metadata Ζωντανή επίδειξη"
    content: |
       Υπογράψτε το αρχείο Dotx με διάφορες υπογραφές αυτήν τη στιγμή, μεταβαίνοντας στον ιστότοπο [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Δωρεάν online demo σας περιμένει.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Άλλες υποστηριζόμενες υπογραφές Metadata για C#"
    content: |
        "Μπορείτε επίσης να υπογράψετε το Dotx με άλλους τύπους υπογραφής. Δείτε την παρακάτω λίστα."
    format: 
       
       
back_to_top:
    enable: true
---