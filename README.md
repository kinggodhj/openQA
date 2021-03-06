### openQA paper list



**- [2017/ACL] Reading Wikipedia to Answer Open-Domain Questions** [[pdf]](https://arxiv.org/pdf/1704.00051.pdf)
    
    Supervised, information retrieval (IR)
    
    
**- [2019/ACL] Latent Retrieval for Weakly Supervised Open Domain question Answering** [[pdf]](https://arxiv.org/pdf/1906.00300.pdf) 
    
    Open Retrieval Question Answering system (ORQA), Not using IR, Inverse Cloze Task (ICT), pre-trained BERT
    
    **Two Phase**
    
            1) Retriever: question * data (wiki) using pre-trained BERT~Q, BERT~B (score)
    
            2) Reader: select Top K of 1) using BERT~R


**- [2020/EMNLP] How Much Knowledge Can You Pack Into the Parameters of a Language Model?** [[pdf]](https://arxiv.org/pdf/2002.08910.pdf) 
            
    T5 (Text-to-Text Transfer Transformer), pre-training, fine-tuning, without external information (only questions)

    **Two Phase**
            
            1) Retriever: Transformer (Text-to-Text, pre-training)
            
            2) Fine-tune the pretrained MLM model 
            
                ++During fine-tuning, any additional information (context) is not provided. Only using the questions
               


**- [2020/ICML] REALM: Retrieval-Augmented Language Model Pre-Training** [[pdf]](https://arxiv.org/pdf/2002.08909.pdf) 
    
    BERT, pre-training, fine-tuning, Inverse Cloze Task (ICT) 
    
    **Two Phase**
            
            1) Retriever: Train masked language model on BERT structure (pre-training)
            
                ++Embeddings are initilized using ICT
            
            2) Fine-tune the pretrained MLM model 
    
    
**- [2020/EMNLP] Dense Passage Retrieval for Open-Domain Question Answering** [[pdf]](https://arxiv.org/pdf/2004.04906.pdf) 
            
    Dense Parse Retrieval (DPR) model, bi-encoder (independent) 
    
    

**- [2020/NeurIPS] Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks** [[pdf]](https://arxiv.org/abs/2005.11401.pdf) 
            
    BART-large (pre-trained), DPR model 
    
    **Two Phase**
            
            1) Retriever: DPR (bi-encoder)
            
                ++pre-trained bi-encoder (BERT) from DPR
            
            2) Generator: Any encoder-decoder
    
                ++authors used pre-trained BART-large
 
 
 
**- [2021/NAACL] Hurdles to Progress in Long-form Question Answering** [[pdf]](https://arxiv.org/pdf/2103.06332.pdf) 
            
    REALM + contrastive loss
    
    

