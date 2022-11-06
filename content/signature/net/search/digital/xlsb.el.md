---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Xlsb
productName: .NET
lang: el
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Xlsb with C#

############################# Head ############################
head_title: "Αναζήτηση για Digital υπογραφές στο αρχείο Xlsb στο C#"
head_description: "Χρησιμοποιήστε το .NET για αναζήτηση υπογραφών Digital σε αρχεία Xlsb χρησιμοποιώντας μερικές γραμμές κώδικα."

############################# Header ############################
title: "Αναζητήστε υπογραφές Digital στο αρχείο Xlsb"
description: "Το εγγενές API του .NET επιτρέπει την αναζήτηση για υπογραφές Digital σε ήδη υπογεγραμμένα αρχεία Xlsb. Εκτελέστε σύνθετη αναζήτηση ηλεκτρονικής υπογραφής στα έγγραφά σας Xlsb χρησιμοποιώντας μερικές γραμμές κώδικα."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Σχετικά με το API GroupDocs.Signature for .NET"
    content: |
        Το [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) παρέχει το API .NET για την επεξεργασία εγγράφων χρησιμοποιώντας διάφορους τύπους υπογραφών, όπως κείμενα, εικόνες, ψηφιακά πιστοποιητικά, γραμμωτούς κώδικες, κωδικούς QR, σφραγίδες ή μεταδεδομένα. Οι χρήστες μπορούν να προσθέσουν, να διαγράψουν, να ενημερώσουν, να επαληθεύσουν ή να αναζητήσουν ηλεκτρονικές υπογραφές σε αρχεία PDF, έγγραφα MS Word, βιβλία εργασίας MS Excel, παρουσιάσεις MS PowerPoint, αρχεία Adobe Photoshop και διάφορες μορφές εικόνας, με πρόσθετη υποστήριξη για την προσαρμογή των ιδιοτήτων υπογραφών ανάλογα με τις ανάγκες.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Τρόπος αναζήτησης για υπογραφές Digital στο Xlsb"
    content_left: |
        Το [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) διευκολύνει τους προγραμματιστές του .NET να αναζητήσουν υπογραφές Digital σε αρχεία Xlsb από τις εφαρμογές τους, εφαρμόζοντας μερικά εύκολα βήματα.
        
        * Δημιουργήστε μια νέα παρουσία κλάσης Signature και περάστε τη διαδρομή εγγράφου προέλευσης ως παράμετρο κατασκευής.
        * Δημιουργήστε το αντικείμενο SearchOptions σύμφωνα με τις απαιτήσεις σας και καθορίστε τις επιλογές αναζήτησης.
        * Καλέστε τη μέθοδο αναζήτησης της παρουσίας κλάσης Signature και περάστε το SearchOptions σε αυτήν.
        * Επεξεργαστείτε τα αποτελέσματα αναζήτησης ανάλογα με τις απαιτήσεις σας.

    title_right: "Απαιτήσεις συστήματος"
    content_right: |
        Το GroupDocs.Signature for .NET υποστηρίζεται σε όλες τις μεγάλες πλατφόρμες και λειτουργικά συστήματα. Πριν εκτελέσετε τον παρακάτω κώδικα, βεβαιωθείτε ότι έχετε εγκαταστήσει τις ακόλουθες προϋποθέσεις στο σύστημά σας.

        * Λειτουργικά συστήματα: Microsoft Windows, Linux, MacOS
        * Περιβάλλοντα ανάπτυξης: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Κατεβάστε την πιο πρόσφατη έκδοση του GroupDocs.Signature for .NET από το [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xlsb file
        string filePath = "input.xlsb";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                DigitalSearchOptions options = new DigitalSearchOptions()
                {
                    // specify special search criteria
                    Comments = "Approved",
                    // specify date range period of signature
                    SignDateTimeFrom = new DateTime(year: 2020, month: 01, day: 01),
                    SignDateTimeTo = new DateTime(year: 2020, month: 12, day: 31)
                };

                // search for Digital signatures in Xlsb document
                List<DigitalSignature> signatures = signature.Search<DigitalSignature>(options);

                // process signatures which were found                
                foreach (DigitalSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Αναζήτηση για Digital ηλεκτρονικές υπογραφές Live Demo"
    content: |
       Αναζητήστε στο έγγραφο διάφορες ηλεκτρονικές υπογραφές σε αρχεία Xlsb αυτήν τη στιγμή, μεταβαίνοντας στον ιστότοπο [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Αναζήτηση για άλλες υπογραφές Digital χρησιμοποιώντας C#"
    content: |
        "Αναζήτηση ηλεκτρονικών υπογραφών σε διάφορα έγγραφα. Βρείτε υπογραφές από μια από τις δημοφιλείς μορφές αρχείων όπως φαίνεται παρακάτω."
    format: 
           
       
back_to_top:
    enable: true
---