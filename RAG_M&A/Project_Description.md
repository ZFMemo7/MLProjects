## RAG Model as an M&A Summarizer ##
This model utilizes a Retrieval-Augmented Generation (RAG) model to quickly summarize the important parts of an announced M&A deal in order to bring an investor with no prior knowledge up to speed with the opportunities and challenges of such deal.

The RAG model is composed of a 3B parameter, open-sourced LLM by Stability AI and a small embedding model to vectorize texts. 

## Process to run it ##
1. Compile all relevant textual data of an M&A deal into one PDF (e.g., announcement, anti-competition rulings, discussions, etc.)
2. Open up Google Colab and change the GPU settings to TPU (free!), and upload the document to your current repository
3. Change some of the questions you want to know regarding the deal / write some general questions you would like to know about every deal
4. Run the model and check the output

## Limitations ##
1. Too short of a context window (will need greater than 4096 tokens), which sometimes leads to repeated outputs
2. Need to write questions before hand, so it would be good to finalize and prompt some general questions
3. PDF needs to be compiled manually, maybe a bot to quickly scrape online data and compile into a PDF will be good
