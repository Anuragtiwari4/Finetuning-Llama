**HINDI DATASET TOKENIZATION**

Dataset Used: "ai4bharat/IndicQA", "indicqa.hi"

Dataset Structure: Dataset used for tokenization is of form context, question and answer. For tokenization contexts, questions and answers are combined to form single hindi sentence. 


Algorithm Used: BPE (Byte Pair Encoding) Algorithm 

BPE Algorithm : Byte-Pair Encoding (BPE) is a compression algorithm used in Natural Language Processing (NLP) to represent large vocabulary with a small set of subword units. It was introduced by Sennrich et al. in 2016 and has been widely used in various NLP tasks such as machine translation, text classification, and text generation. The basic idea of BPE is to iteratively merge the most frequent pair of consecutive bytes or characters in a text corpus until a predefined vocabulary size is reached. The resulting subword units can be used to represent the original text in a more compact and efficient way.

Few Terms related to BPE Algorithm:

Vocabulary: A set of subword units that can be used to represent a text corpus.

Byte: A unit of digital information that typically consists of eight bits.

Character: A symbol that represents a written or printed letter or numeral.

Frequency: The number of times a byte or character occurs in a text corpus.

Merge: The process of combining two consecutive bytes or characters to create a new subword unit.

Steps involved in BPE Algorithm:

1. Initialization vocabulary with all the bytes or characters in the text dataset.

2. Calculate frequency of each byte or character in the text dataset.
   
3. Repeat the following steps until the desired vocabulary size is reached:

    1. Find the most frequent pair of consecutive bytes or characters in the text corpus
    2. Merge the pair to create a new subword unit.
    3. Update the frequency counts of all the bytes or characters that contain the merged pair.
    4. Add the new subword unit to the vocabulary.
4. Represent the text corpus using the subword units in the vocabulary


**Appending the custum vocab created using BPE Tokenization in Llama 3.1 Tokenizer**

Model Used : https://huggingface.co/akjindal53244/Llama-3.1-Storm-8B

Updated Model: https://huggingface.co/Anurag-Tiwari/hindi_updated-llama-model

Updated Tokenizer: https://huggingface.co/Anurag-Tiwari/hindi_updated-llama-tokenizer
