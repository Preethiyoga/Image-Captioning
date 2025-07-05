<b>Image Captioning</b>



Image captioning is a method to describe an image by generating a textual description. It is in massive demand for people with impaired visuals as this method helps them listen to the text with the help of AI. Image captioning converts an image which is considered a sequence of pixels, into a sequence of words.


<b>MODEL DESIGN (Architecture)</b>
            
            
            Image                             Partial Caption
      
       -------------                         -----------------
      
      | CNN (InceptionV3) |                 | Embedding Layer |
      
       -------------                         -----------------  
              
              |                                      |
     
     Dense Layer -1 (feature vector)              LSTM Layer
              
              |                                      |
              
              |-------- Concatenate -----------------|
                            
                            |
                        
                        Dense Layer
                     
                            |
                    
                    
                    Softmax (Vocab Size)
                         
                            
                            ↓
               
                
                Predict Next Word in Caption
