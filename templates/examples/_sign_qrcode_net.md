        
        // Set up input <% get "Fileformat" %> file
        string filePath = "input.<% lower (get "Fileformat") %>";
        // Set up output file
        string outputFilePath = "output.<% lower (get "Fileformat") %>";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined QrCode text
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // setup QrCode encoding type
                    EncodeType = QrCodeTypes.<% get "Codetype" %>,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50
                };

                // sign <% get "Fileformat" %> document
                SignResult result = signature.Sign(outputFilePath, options);
        }
