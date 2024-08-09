
        // Set up input <% get "Fileformat" %> file
        string filePath = "input.<% lower (get "Fileformat") %>";
        // Set up output file
        string outputFilePath = "output.<% lower (get "Fileformat") %>";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                PdfMetadataSignature mdSign_Author = new PdfMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                PdfMetadataSignature mdSign_DocData = new PdfMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                PdfMetadataSignature mdSign_DocId = new PdfMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign <% get "Fileformat" %> document
                SignResult result = signature.Sign(outputFilePath, options);
        }
