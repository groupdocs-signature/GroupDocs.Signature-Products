        
        // Set up input <% get "Fileformat" %> file
        string filePath = "input.<% lower (get "Fileformat") %>";
        // Set up output file
        string outputFilePath = "output.<% lower (get "Fileformat") %>";
        // Provide image file
        string imageFilePath = "image.png";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                ImageSignOptions signOptions = new ImageSignOptions(imageFilePath);
                {
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign <% get "Fileformat" %> document
                SignResult result = signature.Sign(outputFilePath, options);
        }
