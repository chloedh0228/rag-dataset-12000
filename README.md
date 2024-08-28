
# **Retrieval-Augmented Generation (RAG) Dataset 12000**

**Retrieval-Augmented Generation (RAG) Dataset 12000 is an English dataset designed for RAG-optimized models, built by  [Neural Bridge AI](https://www.neuralbridge.ai/), and released under  [Apache license 2.0](https://www.apache.org/licenses/LICENSE-2.0.html).**

## Dataset Description**

#### Dataset Summary

Retrieval-Augmented Generation (RAG) enhances large language models (LLMs) by allowing them to consult an external authoritative knowledge base before generating responses. This approach significantly boosts the models' ability to produce relevant, accurate, and context-specific output by extending their capabilities to specialized domains or an organization's internal data, without the need for retraining. RAG offers a cost-effective method to leverage the vast data processing power of LLMs, equipped with billions of parameters, for tasks such as question-answering, language translation, and sentence completion, ensuring that the output is always up-to-date and applicable to various contexts.

RAG's importance lies in its potential to address the inherent challenges of LLMs, such as unpredictability in responses, reliance on static and potentially outdated training data, and the risk of disseminating incorrect or non-authoritative information. These issues can negatively affect user trust in AI-powered applications, making RAG's ability to guide LLMs toward authoritative sources for information retrieval invaluable.

RAG has multiple benefits, including cost-effective implementation and maintenance, access to current information, improved user trust through accurate information and source attribution, and greater control for developers over the information retrieval process. This approach allows for the dynamic updating of LLMs with the latest research, statistics, or news, directly addressing the challenges of maintaining relevancy and accuracy in rapidly changing knowledge landscapes. Additionally, it empowers organizations to deploy generative AI more confidently across a wider range of applications, enhancing both the user experience and the reliability of AI-driven interactions.

Retrieval-Augmented Generation (RAG) Dataset 12000 dataset is a triple-feature collection, with each entry containing a "context", "question", "answer", "extacted_sentences" and "logical_category" fields, designed to help build RAG-optimized models. This data consists of 12000 entries, and the context data is from  [Falcon RefinedWeb](https://huggingface.co/datasets/tiiuae/falcon-refinedweb).

```
from datasets import load_dataset
rag_dataset = load_dataset("chloed28/rag-dataset-12000")
```
#### Languages

The text in the dataset is in English. The associated BCP-47 code is  `en`.


## **Dataset Structure**

#### Data Instances

A typical data point comprises a context, a question about the context, and an answer for the question. The context is obtained from  [Falcon RefinedWeb](https://huggingface.co/datasets/tiiuae/falcon-refinedweb).

An example from the dataset looks like the following:

```
{
  context: ...
  question: ...
  answer: ...
  extracted_sentences: ...
  logical_category: ...
}

```
#### Data Fields

-   `context`: A string consisting of a range of tokens.
-   `question`: A string consisting of a question related to the context.
-   `answer`: A string consisting of an answer for the question.
-   `extracted_sentences`: A list of strings, each representing an original sentence from the source article, used to generate the answer.
-   `logical_category`: An enumerated string indicating the logical category between the question and the answer.


#### Data Splits

The data is split into a training and test set. The split sizes are as follow:
|  | Train | Test |
|--|--|--|
| RAG Dataset 12000 | 9600 |2400 |



## Source Data

The data points in the dataset are from the  [Falcon RefinedWeb](https://huggingface.co/datasets/tiiuae/falcon-refinedweb)  dataset.


## **License**

This public extract is made available under  [Apache license 2.0](https://www.apache.org/licenses/LICENSE-2.0.html). Users should also abide to the  [Falcon RefinedWeb](https://huggingface.co/datasets/tiiuae/falcon-refinedweb)  ToU.