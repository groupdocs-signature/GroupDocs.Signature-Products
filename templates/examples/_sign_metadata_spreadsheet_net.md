//spread
        // Set up input <% get "Fileformat" %> file
        string filePath = "input.<% lower (get "Fileformat") %>";
        // Set up output file
        string outputFilePath = "output.<% lower (get "Fileformat") %>";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create metadata signature with predefined barcode text
                var options = new MetadataSignOptions();

                // add various metadata signature items to the document
                //  no encryption
                options
                    .Add(new PdfMetadataSignature("Author", "Mr.Scherlock Holmes")) // String value
                    .Add(new PdfMetadataSignature("CreatedOn", DateTime.Now))       // Datetime value
                    .Add(new PdfMetadataSignature("DocumentId", 123456))            // Integer value
                    .Add(new PdfMetadataSignature("SignatureId", 123.456D))         // Double value
                    .Add(new PdfMetadataSignature("Amount", 123.456M))              // Decimal value
                    .Add(new PdfMetadataSignature("Total", 123.456F));              // Float value
                
                // sign <% get "Fileformat" %> document
                SignResult result = signature.Sign(outputFilePath, options);
        }
