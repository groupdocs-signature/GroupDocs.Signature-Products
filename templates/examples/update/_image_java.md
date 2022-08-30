        
        // Set up input <% get "Fileformat" %> file
        string filePath = "input.<% lower (get "Fileformat") %>";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be get as result of search operation
        string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

        // provide signature features to update
        ImageSignature signatureToUpdate = new ImageSignature();

        // set up particular signature id
        signatureToUpdate.setSignatureId(id);
        // specify signature width
        signatureToUpdate.setWidth(170);
        // specify signature height
        signatureToUpdate.setHeight(250);
        // set left position
        signatureToUpdate.setLeft(10);
        // set top position
        signatureToUpdate.setTop(10);

        // update signature
        bool updateResult = signature.Update(signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }