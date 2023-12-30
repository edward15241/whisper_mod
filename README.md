# whisper_mod
Fine-tune, distilling, pruning, finetuning for existing whisper model.

This project is primarily for self learning and experimenting with the existing Whisper model and its fine-tuning methods.
In the event that we have some of our own ideas, we will also carry out some fine-tuning experiments. 
This project encompasses these experimental records, and the majority of the training scripts and pre-trained models 
are sourced from open-source platforms like HuggingFace.

此專案僅用於實驗以及學習微調 whisper 模型，並且多數腳本均來自於網路上的資源或是 hugginface 提供的範例。
有時候自己有一些微條或訓練上調整的想法也會在此專案做嘗試。 

此專案設計方式與一般專案不同，因為多數 script 僅用於測試或驗證模型，
僅執行於 ubuntu 20.04/22.04 上且使用cuda 11.8 以後的cuda 版本，顯示卡為RTX-4090。因此多數實驗腳本僅保證能於 RAM 24GB 的資源執行。
如果有 A6000、A100、H100 等新卡，配置可能不適用。

此專案僅作為個人學習使用，更新時間隨機，以實驗為優先，可能因為本人程式撰寫習慣不好 或是 流程是 copy& paste 導致可讀性不佳， 
因此腳本在初期不適特別高，但會隨時間慢慢修正 (keep learning)。

專案 coding style 採用PEP8 之上的規則做一些修改。工作之餘有時間才更新，有想法才會更新。萬一 whisper 哪天被取代了，那這專案就廢了。 :P

# TODO
1. 基本的 whisper 微調 ( LoRA、AdaLoRA、Finetune )
2. Inference:  Speculative Decoding, Medusa for whisper model
3. Distilled whisper with streaming Conformer
4. Prompt tuning and multi-task learning with whisper model
5. Whisper_transcribe_pipeline
