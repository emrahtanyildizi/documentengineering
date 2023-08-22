# documentengineering

post-doc research repository

Table of contents:
- Topic
- Problem Statement
- Research question
- Objective
- Key business usage
- Methods
- Topics of interest
- Keywords
- Datasets
- Papers
- Business sources
- News
- Conferences/events



TOPIC: ""Using AI to Build Document Processing Workflows""

Problem statement - Research question:
STATEMENT: Companies worldwide heavily depend on documents as a means to store and communicate vital information. Often, the transformation of this information into a digital format is essential for its utility. Nevertheless, today achieving this digitization typically involves laborious and time-consuming manual procedures that introducing inefficiencies that hinder business operations and decrease effective decision-making capabilities. The AI-based interpretation of documents such as invoices and contracts represents a profitable prospect and leading in new business opportunities. Moreover, the unstructured nature of documents introduces complexity, making it crucial to mobilize this unstructured data for a seamless and cohesive data flow. This converted data could be used for traditional analytics, BI or other downstream ML processes. Deep learning breakthroughs have driven substantial development in Large Language Models, natural language processing and computer vision, resulting in the incorporation of these approaches into modern document understanding systems. 

QUESTION: How does the implementation of LLM-driven Document AI impact the efficiency and accuracy of transforming diverse document types into usable data, considering the variations in document structures, layouts, and information relevance? How does this transformation influence enterprises' ability to shift their operational focus from data compilation to informed decision-making?

Objective: Mobilize unstructured data/information for business needs #fitforpurpose


KEY BUSINESS USAGE:
* Completing medical intake forms during visits to medical facilities
* Processing expense reports utilizing receipts and invoices (service fee processing - fixed fees, capped fees, success-based fees, dynamic pricing (demand vs. cost)
* Verifying identity through ID card authentication
* Granting loan approvals using income details from tax forms
* Interpreting contracts relevant to significant business agreements
* Immigration document automation - RPA


Methods: 
- Large Language Model (LLM) - driven
- Generative Pre-trained Transformer (GPT)
- Key Information Extraction (KIE) / Key-Value Pair Extraction Models
- Natural Language Processing (NLP)
- Document Layout Analysis (DLA)
- Document Question Answering (DQA)
- Scientific Document Understanding (SDU)
- Optical Character Recognition (OCR)
- Table Extraction Models
- Tabular Data Comprehension (TDC)
- Robotic Process Automation (RPA)

Topics of Interest:
Document image processing / Physical and logical layout analysis / Text and symbol recognition / Handwriting recognition / Document analysis systems / Document classification / Indexing and retrieval of documents / Document synthesis / Extracting document semantics / NLP/LLM for document understanding / Human document interaction / Document Representation Modeling / Structured document generation / Multimedia document analysis / Mobile text recognition / Pen-based document analysis / Scene text detection and recognition / Recognition of tables and formulas / Historical document analysis / Signature verification / Document summarization and translation / Document forensics and provenance / Medical document analysis / Document analysis for social good / Document analysis for literature search / Gold-standard benchmarks and datasets

Keywords: Document AI, Document engineering, Document Intelligence, Intelligent document processing, document understanding, Generative AI for business documents, Deep learning, Applied data science, ADL-computer vision, Machine Learning Models, Structured/unstructured data, Tensorflow, extract text, key-value pairs, document processing, knowledge mining, automate business workflows,transformers, ...

Datasets:
Microsoft research: https://github.com/doc-analysis
XFUND:  https://github.com/doc-analysis/XFUND


Papers
1- TrOCR: Transformer-based Optical Character Recognition with Pre-trained Models Minghao Li, Tengchao Lv, Jingye Chen, Lei Cui, Yijuan Lu, Dinei Florencio, Cha Zhang, Zhoujun Li, Furu Wei AAAI 2023 | February 2023 https://arxiv.org/abs/2109.10282
Efforts to convert textual content within documents into a digital format have posed a persistent challenge in research circles. Conventional methodologies typically rely on Convolutional Neural Networks (CNNs) for comprehending images, and Recurrent Neural Networks (RNNs) for generating text on a character-by-character basis. Additionally, it's common to introduce an additional language model as a refinement step to enhance overall accuracy. However, the paper introduces a new approach, TrOCR, a comprehensive solution for text recognition that covers the entire process. The researchers harness the power of pre-trained image Transformer and text Transformer models, seamlessly integrated into a unified framework. With TrOCR, it is not solely interpreting images and constructing characters; it is also deconstructing words into smaller units for enhanced comprehension. TrOCR adopts an elegantly simple methodology, yet its impact is profound. Reseahers can initially train it on synthetically generated data and then fine-tune it using meticulously labeled human-generated datasets. Furthermore, this experiment demonstrate that TrOCR outperforms incumbent models in recognizing text across printed, handwritten, and even scene-based scenarios. The TrOCR models and code accessible at the following link https://github.com/microsoft/unilm/tree/master/trocr

2- DocILE Benchmark for Document Information Localization and Extraction, Stepan Simsa, et al. 2023 -  https://arxiv.org/abs/2302.05658    
This research paper introduces the DocILE benchmark, featuring the most extensive collection of business documents designed for two primary tasks: Key Information Localization and Extraction, as well as Line Item Recognition. The dataset encompasses 6.7k meticulously annotated business documents, supplemented by 100k synthetically generated documents, and an additional ~1M unlabeled documents to facilitate unsupervised pre-training. The construction of this dataset incorporates domain- and task-specific expertise, resulting in the following notable attributes:
Annotations span across 55 distinct classes, a substantial improvement in granularity compared to previously published datasets for key information extraction.
The Line Item Recognition task addresses a practical scenario where essential information must be associated with items within a table.
The documents originate from a diverse range of layouts, and the test set includes instances with zero- and few-shot cases, along with layouts commonly encountered in the training set.
The benchmark is accompanied by several baseline models, including RoBERTa, LayoutLMv3, and DETR-based Table Transformer, all applied to both tasks within the DocILE benchmark. The results of these baselines are presented in the paper, serving as a valuable starting point for future research endeavors. 

3- XDoc: Unified Pre-training for Cross-Format Document Understanding
Jingye Chen, Tengchao Lv, Lei Cui, Cha Zhang, Furu Wei EMNLP 2022 | December 2022 https://arxiv.org/abs/2210.02849
The recent proliferation of pre-training techniques has fueled rapid advancements in the realm of document comprehension. The pre-training and fine-tuning framework has proven highly effective in addressing texts of diverse formats, encompassing plain text, document content, and web-based textual data. Despite their promising achievements, current pre-trained models tend to specialize in specific document formats, hindering the amalgamation of insights from multiple document types. In response, the authors introduce XDoc, a holistic pre-trained model designed to seamlessly accommodate a spectrum of document formats within a single architecture. To optimize parameter utilization, they employ shared backbone parameters for distinct formats, encompassing elements like word embedding layers and Transformer components. Simultaneously, adaptive layers are introduces and characterized by lightweight parameters, to enrich the model's adaptability across varying formats. Empirical findings underscore the effectiveness of XDoc. Remarkably, with a mere 36.7% of the parameters utilized by individual pre-trained models, XDoc attains comparable, if not superior, performance across a diverse array of downstream tasks. This cost-effective efficacy positions XDoc as a valuable asset for real-world deployment. For those interested, the code and pre-trained models are accessible through the following link: https://github.com/microsoft/unilm/tree/master/xdoc

4- Business Document Information Extraction: Towards Practical Benchmarks - Matyas Skalicky, et al. 2022 - https://arxiv.org/abs/2206.11229

Efficient business-to-business (B2B) communication heavily relies on extracting information from partially structured documents. Despite the long-standing exploration of Machine Learning challenges associated with Document Information Extraction (IE), many prevailing problem formulations and performance standards fail to encompass industry-specific nuances and the tangible requirements for automating B2B document exchange. Our assessment traverses the landscape of Document IE quandaries, datasets, and performance yardsticks. We underscore the real-world aspects that elude conventional definitions and introduce the Key Information Localization and Extraction (KILE) as well as the Line Item Recognition (LIR) predicaments. The scarcity of pertinent datasets and benchmarks for Document IE concerning semi-structured business documents stems from their customary legal or sensitive content. We delve into potential resources for accessible documents, including the prospect of synthetic data.

5- DiT: Self-supervised Pre-training for Document Image Transformer
Junlong Li, Yiheng Xu, Tengchao Lv, Lei Cui, Cha Zhang, Furu Wei ACM Multimedia 2022 | October 2022 https://arxiv.org/abs/2203.02378
The Image Transformer paradigm has achieved remarkable strides in comprehending natural images, whether through supervised methodologies (such as ViT, DeiT, etc.) or self-supervised approaches (like BEiT, MAE, etc.). This study introduces \textbf{DiT}, a self-supervised pre-trained model centered on \textbf{D}ocument \textbf{I}mage \textbf{T}ransformation. DiT capitalizes on a vast collection of unlabeled text images, a necessity for Document AI tasks where supervised counterparts are conspicuously absent, given the scarcity of human-labeled document images.

6- DiT takes on the role of the foundational network in diverse vision-driven Document AI tasks, encompassing document image classification, document layout analysis, table detection, and text detection for OCR applications. Empirical outcomes underscore that the self-supervised, pre-trained DiT model establishes a fresh benchmark in these downstream tasks, exemplified by its superior performance in document image classification and beyond

7- LayoutLMv3: Pre-training for Document AI with Unified Text and Image Masking
Yupang Huang, Tengchao Lv, Lei Cui, Yutong Lu, Furu Wei ACM Multimedia 2022 | October 2022 https://arxiv.org/abs/2204.08387
Significant strides have been made in Document AI through the application of self-supervised pre-training techniques. While most multimodal pre-trained models leverage masked language modeling objectives to attain bidirectional representations for the text modality, their divergence in pre-training objectives for the image modality introduces complexities to the process of multimodal representation learning. Addressing this challenge, this study presents \textbf{LayoutLMv3}, a novel approach for multimodal Transformer pre-training in the context of Document AI. Its method introduces unified text and image masking, unifying the pre-training process. Furthermore, LayoutLMv3 incorporates a word-patch alignment objective during pre-training. This alignment objective enhances cross-modal alignment by predicting whether a masked image patch corresponds to a given text word. The elegantly straightforward architecture and training objectives of LayoutLMv3 position it as a versatile pre-trained model suitable for both text-centric and image-centric Document AI tasks. Empirical findings affirm the efficacy of LayoutLMv3. It not only attains state-of-the-art performance in text-centric tasks, such as form understanding, receipt understanding, and document visual question answering, but also excels in image-centric tasks, including document image classification and document layout analysis. The code and models are available to the public via the following link: https://github.com/microsoft/unilm/tree/master/layoutlmv3

8- MarkupLM: Pre-training of Text and Markup Language for Visually-rich Document Understanding by Junlong Li, Yiheng Xu, Lei Cui, Furu Wei ACL 2022 | May 2022 https://arxiv.org/abs/2110.08518
Considerable advancements have been achieved in Visually Rich Document Understanding (VRDU) through multimodal pre-training involving text, layout, and images. This progress has been particularly noticeable for documents with fixed layouts, like scanned document images. Nonetheless, a substantial volume of digital documents still exists, characterized by fluid and adaptable layouts that require interactive and dynamic rendering for effective visualization. As a result, conventional layout-focused pre-training techniques face challenges when applied to such cases. In this research paper, the authors introduce MarkupLM, a novel approach tailored for tasks related to document comprehension, specifically for documents structured using markup languages like HTML/XML. MarkupLM involves the joint pre-training of both text and markup information, forming a robust foundation. Empirical evaluations demonstrate that the pre-trained MarkupLM model consistently outperforms established benchmark models across various document understanding tasks. The model's pre-trained version and accompanying code will be made publicly accessible via the following URL https://github.com/microsoft/unilm/tree/master/markuplm.

9- Document AI: Benchmarks, Models and Applications, Lei Cui and et al. 2021 - https://arxiv.org/abs/2111.08609
Emerging as a novel field of study, Document AI, or Document Intelligence, pertains to the realm of automating the interpretation, comprehension, and assessment of business documents. Positioned at the intersection of natural language processing and computer vision, it holds significant importance. The ascent of deep learning techniques in recent times has propelled the advancement of Document AI, encompassing areas like document layout analysis, visual information extraction, document visual question answering, document image classification, and more. This document provides a succinct overview of key models, tasks, and benchmark datasets that characterize this domain. Additionally, it delves into preliminary heuristic rule-based document analysis, statistical machine learning algorithms, and primarily pre-training methodologies within the purview of deep learning. Lastly, prospective avenues for future research in the field of Document AI are contemplated.

10 - Efficient Automated Processing of the Unstructured Documents Using Artificial Intelligence: A Systematic Literature Review and Future Directions, Dipali Baviskar and et al. - https://ieeexplore.ieee.org/abstract/document/9402739
Ninety-five percent of organizations are affected by unstructured data, resulting in annual costs amounting to millions of dollars. Skillful management of this data holds the potential to substantially enhance business productivity. Conventional information extraction methods have inherent limitations, whereas AI-powered approaches offer a more promising remedy. Surprisingly, a comprehensive exploration of AI-driven methods for autonomously extracting information from unstructured documents remains absent in existing literature. This Systematic Literature Review (SLR) aims to identify and scrutinize research concerning techniques employed in the automatic extraction of information from unstructured documents, while also charting pathways for future investigative efforts.


Business sources: 
Google: Document AI https://cloud.google.com/document-ai
Google: DocumentAI for developers https://developers.google.com/learn/topics/document-ai
Azure Document Intelligence: https://azure.microsoft.com/en-us/products/ai-services/ai-document-intelligence
Amazon: Scaling intelligent document processing workflows with AWS AI services https://aws.amazon.com/blogs/publicsector/scaling-intelligent-document-processing-workflows-aws-ai/
UiPath: https://www.uipath.com/product/document-understanding
IBM:Accelerate business decisions and processes with an AI-powered intelligent document understanding and content analysis platform https://www.ibm.com/products/watson-discovery?utm_content=SRCWW&p1=Search&p4=43700075721478226&p5=p&gclid=Cj0KCQjwldKmBhCCARIsAP-0rfx01dIg_SouZjSJc9qfIFlD3CDu3U0SOlua3VnzaF_pK8ybHxLJhR4aAgffEALw_wcB&gclsrc=aw.ds
Petal: document analysis platform: https://www.petal.org/
Snowflake: Snowflake is making another generative AI push. Today at its annual conference, the data cloud company announced Document AI, a new large language model (LLM)-based interface that allows enterprises to quickly extract value from their barrage of documents. The move marks a major development for the data giant — which started off with a focus on structured data — and provides an easy way to mobilize useful unstructured information that often remains scattered across silos.Customers will see an end-to-end experience where they will able to have documents in Snowflake and ask structured questions from those documents — like what’s the name of the employee, what’s their address or the total value in the invoice,” Kleinerman explained in a press briefing. “This will trigger the system to take the documents, which are unstructured files, and convert them into structured data. This converted data could be used for traditional analytics, BI or other downstream ML processes
Applica: acquired by Snowflake https://www.applica.ai/
Docsumo: https://www.docsumo.com/blog/document-ai-future#:~:text=AI%2Dbased%20document%20processing%20technology,easily%20analyzed%20and%20stored%20later.


News:
Using AI To Automate Enterprise Document Processing Workflows: https://www.forbes.com/sites/forbestechcouncil/2021/04/20/using-ai-to-automate-enterprise-document-processing-workflows/?sh=1d10a02f1323


Conferences / workshops
- International Conference on Document Analysis and Recognition (ICDAR) 2023 https://icdar2023.org/program/accepted-papers/
- 

6. 
