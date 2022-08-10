        // Instantiate Signature for <% get "FILEFORMAT" %> file
        string filePath = "input.<% lower (get "FILEFORMAT") %>";
        // Set up output <% get "FILEFORMAT" %> file
        string outputFilePath = "output.<% lower (get "FILEFORMAT") %>";

        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.<% get "BARCODETYPE" %>,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50
                };

                // sign <% get "FILEFORMAT" %> document
                SignResult result = signature.Sign(outputFilePath, options);
        }
