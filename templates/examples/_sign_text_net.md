        
        // Set up input <% get "FILEFORMAT" %> file
        string filePath = "input.<% lower (get "FILEFORMAT") %>";
        // Set up output file
        string outputFilePath = "output.<% lower (get "FILEFORMAT") %>";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                TextSignOptions options = new TextSignOptions("John Smith")
                {
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign <% get "FILEFORMAT" %> document
                SignResult result = signature.Sign(outputFilePath, options);
        }
