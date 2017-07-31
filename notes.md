## Outline for the talk

* Encoder Decoder in general
    
    * Basics
        * Encoder -> Map input to hidden space representation (aka code)
        * Decoder -> Map hidden space representation (aka code) to desired output

    * Example
        * Sequence-to-Sequence

* Why Encoders at all

    * General ML workflow

        * Read the problem statement
        * Look at the dataset
        * Extract "relevant" (as we feel) features - aka feature engineering
        * Feed to the network

    * Ideally we would want the network to "learn" how to extract the relevant featues which it thinks are neceassry.

    * Introduce Auto Encoders

* Auto Encoders
    
    * Try to reconstruct their own input
    * Can be used for:
        * Dimensionality Reduction
        * Data Synthesis
        * Regularisation of data

    * Auto Encoders vs feature reduction techniques

        * PCA etc generate a representation independent of the downstream task. So the representation would be the same no matter what model we train.
        * Further, PCA (and other linear techniques) can learn only linear manifolds
        * Auto Encoders can learn both linear and non linear manifolds and hence are supersets
        * Introduce the theory of manifold learning

* Manifold Learning
    
    * Dimensionality of many datasets is just artifically high
    * Give example of say face recognition
    * AutoEncoders with an additional loss can recreate the neighbourhood as well


* Encoder Decoder in depth

    * Multi-modal encoder-decoders
        * General encoder-decoders which operate across modalities
        * Neural Image Captioning

    * Encoders Vs Embedding
        * Enbedding
            * generally just one layer
            * more like a look up table
        * Encoders
            * generally multi layer
            * more like a standalone network in itself