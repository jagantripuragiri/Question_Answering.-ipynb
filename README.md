###Build a document-based question answering system by using Docling with Granite 3.1


##What is Docling?
Docling is an IBM open-source toolkit for parsing documents and exporting them to preferred formats. Input file formats include PDF, DOCX, PPTX, XLSX, Images, HTML, AsciiDoc and Markdown. These documents can be exported to markdown or JSON. Docling also provides OCR (optical character recognition) support for scanned documents. Use cases include scanning medical records, banking documents and even travel documents for quicker processing.

##RAG and large context windows
Retrieval augmented generation (RAG) is an architecture for connecting large language models (LLMs) with external knowledge bases without fine-tuning or retraining. Text is embedded, stored in a vector database and finally, is used by the pre-trained model to return relevant information for natural language processing (NLP) and machine learning tasks.

When an LLM has a larger context window, the generative AI model can process more information at once. This means that we can use both RAG and models with large context windows to leverage the ability to efficiently process more relevant information at a time. The LLM we use in this tutorial is the IBM Granite-3.1-8B-Instruct model. This model extends to a context window size of 128K tokens. We will access the model locally by using Ollama, without the use of an API. This model is also available on Hugging Face.
