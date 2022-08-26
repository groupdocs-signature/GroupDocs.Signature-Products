        
        // Set up input <% get "Fileformat" %> file
        string filePath = "input.<% lower (get "Fileformat") %>";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                ImageSearchOptions options = new ImageSearchOptions()
                {
                    // set minimum size if needed
                    MinContentSize = 100,
                    // set maximum image size if needed
                    MaxContentSize = 2000,                    
                    // return  <% get "Signaturetype" %> images for processing
                    ReturnContent = true,
                    // set up type of returned  <% get "Signaturetype" %> images
                    ReturnContentType = FileType.PNG                                 
                };

                // search for <% get "Signaturetype" %> signatures in <% get "Fileformat" %> document
                List<ImageSignature> signatures = signature.Search<ImageSignature>(options);

                // process signatures which were found                
                foreach (ImageSignature signature in signatures)
                {
                    //...
                }
        }
