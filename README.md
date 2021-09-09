### openQA paper list

**- [2017/ACL] Reading Wikipedia to Answer Open-Domain Questions** [[pdf]](https://arxiv.org/pdf/1704.00051.pdf)
    
    Supervised, information retrieval (IR)
    
**- [2019/ACL] Latent Retrieval for Weakly Supervised Open Domain question Answering** [[pdf]](https://arxiv.org/pdf/1906.00300.pdf) 
    
    Open Retrieval Question Answering system (ORQA), Not using IR, Inverse Cloze Task (ICT), pre-trained BERT
    
    <u>Two Phase</u>
    
            1) Retriever: question * data (wiki) using pre-trained BERT~Q, BERT~B (score)
    
            2) Reader: select Top K of 1) using BERT~R

**- [2020/ICML] REALM: Retrieval-Augmented Language Model Pre-Training** [[pdf]](https://arxiv.org/pdf/2002.08909.pdf) 
    
    BERT, pre-training, fine-tuning, Inverse Cloze Task (ICT) 
    
    <u>Two Phase</u>
            
            1) Retriever: Train masked language model on BERT structure (pre-training)
            
                ++Embeddings are initilized using ICT
            
            2) Fine-tune the pretrained MLM model 
            
            
