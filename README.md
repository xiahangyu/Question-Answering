# Question-Answering
This project is aiming to find an answer for questions when a document is given. 

## Files in the data directory
  * documents.jason : A list of documents. Each item is a tuple of a document_id and a list of paragraphs.
  * training.jason & devel.jason : A list of questions along with the answers. Each item is in the format of (question, answer, answer_paragraph, document_id).
  * testing.jason : A list of questions only. Each item is in the format of (question, document_id, id).
  * random.csv : Answer for the questions in the testing.jason file.
  
## Methods
  * Infomation Retrival: find answers based on NER.
  * Seq2Seq models: one with GRU, one with LSTM. Both locate the answer paragraph/sentence first then predict the answer by approxiamting the function (answer para/sents, question)->answer. 
