
        // Set up input <% get "Fileformat" %> file
        string filePath = "input.<% lower (get "Fileformat") %>";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // search for <% get "Signaturetype" %> signatures in <% get "Fileformat" %> document
                List<WordProcessingMetadataSignature> signatures = signature.Search<WordProcessingMetadataSignature>(SignatureType.Metadata);

                // process signatures which were found 
                foreach (WordProcessingMetadataSignature item in signatures)
                {
                    //...
                }
        }
