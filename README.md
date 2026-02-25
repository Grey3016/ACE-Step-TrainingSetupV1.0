# My ACE-Step-Training Setup V1.0

I use Ace-Step-Trainer but will be trying out the other trainers shortly - 
<img width="1246" height="539" alt="image" src="https://github.com/user-attachments/assets/fbe31890-401b-4e5d-bdf7-72acc145c3f9" />
I select Base , I initially used SFT but from most of the advice , it appears that Base is the best um......base for training 

<img width="1873" height="946" alt="image" src="https://github.com/user-attachments/assets/2ff8a00b-a314-43e9-80d4-8ffc659691e6" />

Upper section of the DataSet tab


Note that the files have a lyrics txt file associated with them ie the same name but with a .txt suffix . I use a preparatory python file that gets them ready for training - normalises the folder of audio files , renames them to their tags (this gives the best chance of finding their lyrics) , then searches for the lyrics and finally saves them as a 48kHz wav in a separate folder (along with their lyrics)

In this example, all of the tracks are not instrumental , so I've NOT selected the Instrumental box .

Genre Ratio should be at 30% and position for tag is Prepend (both of these are from notes across several Discords)

<img width="1877" height="718" alt="image" src="https://github.com/user-attachments/assets/d26034f3-e7a5-45b0-adaa-a4294c6bb018" />

Lower section of Dataset tab , obviously pressing the Analyse and then the Save buttons on the screen

<img width="1864" height="564" alt="image" src="https://github.com/user-attachments/assets/51bdf114-5226-4d8b-8143-0701893793ad" />

The Preprocess tab , apart from adjusting the folder name for clarity, just press the Preprocess button to start making the pt files (this tab automatically uses the dataset you made in the Dataset tab) 


<img width="1873" height="1018" alt="image" src="https://github.com/user-attachments/assets/34d625a9-a32f-45e3-b706-9d97ecda6955" />

Upper half of the Training tab, I select my GPU and it puts in the values - I adjust some , epochs I increase to 1500 (it doesn't matter as it auto stops when it sees that the epochs aren't getting better) . I also increase the Rank and Alpha .

<img width="936" height="907" alt="image" src="https://github.com/user-attachments/assets/29c7123b-4a37-40b4-aa24-878b158f5466" />

Middle section of the training tab , I increase the Steps to max

<img width="1886" height="954" alt="image" src="https://github.com/user-attachments/assets/890a2766-f7df-4d6f-99f8-f252c5fe742e" />

Adjusting the output lora directory, just a matter of pressing Start Training and then Export after it's done. 
