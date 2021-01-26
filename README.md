# transformer_upload
1- Proesss: https://huggingface.co/transformers/model_doc/auto.html


2- requirement: 
2.1. install lfs: https://git-lfs.github.com/
2.2. `sudo apt-get install git-lfs`
Ref: https://stackoverflow.com/questions/48734119/git-lfs-is-not-a-git-command-unclear


3. Load and save model:
```
model = AutoModel.from_pretrained(
  "./model, from_tf=False)

tokenizer = ByteLevelBPETokenizer(
    "./voc/vocab.json",
    "./voc/merges.txt",
)

model.save_pretrained("/model/final")
tokenizer.save_model("/model/final")
```
