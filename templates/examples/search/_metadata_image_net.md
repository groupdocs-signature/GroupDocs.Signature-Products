
        // Set up input <% get "Fileformat" %> file
        string filePath = "input.<% lower (get "Fileformat") %>";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // search for <% get "Signaturetype" %> signatures in <% get "Fileformat" %> document
                List<ImageMetadataSignature> signatures = signature.Search<ImageMetadataSignature>(SignatureType.Metadata);

                // process signatures which were found 
                foreach (ImageMetadataSignature mdSignature in signatures)
                {
                    //...
                }
        }
