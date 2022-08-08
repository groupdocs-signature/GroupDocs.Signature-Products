        // Instantiate Signature for <% get "FILEFORMAT" %> file
        string filePath = "input.<% lower (get "FILEFORMAT") %>";
        // Set up output <% get "FILEFORMAT" %> file
        string outputFilePath = "input.<% lower (get "FILEFORMAT") %>";

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