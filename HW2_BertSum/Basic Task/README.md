# Basic Task: Replicate the BertSum Model.
📌 因為免費版的 Colab 有GPU的使用限制 (一天12小時)，且閒置過長時間會斷線的問題 <br>
📌 本人決定在自家電腦建一個環境來跑作業

## 於 Windows 系統 - 建立虛擬環境 (Anaconda)
1. 首先，安裝 Anaconda
   1. 進入 Anaconda 官網 https://www.anaconda.com/download#windows
   2. 提供 Email 就可以取得安裝包
   3. 跟著指引安裝就可以安裝完畢
   4. 開啟 CMD.exe Prompt 就可以開始建立 Python 環境
2. 建立 Python 環境 (Python Version = 3.12.7)
   1. 查看電腦安裝的 CUDA 版本 (12.6)
   2. 到 Pytorch 官網尋找與 CUDA 版本相容的指令進行下載 https://pytorch.org/get-started/previous-versions/

          # For CUDA 12.6
          pip install torch==2.6.0 torchvision==0.21.0 torchaudio==2.6.0 --index-url https://download.pytorch.org/whl/cu126
   3. 接著安裝作業需要的套件
  
          pip install pytorch_pretrained_bert
          pip install tensorboardX
          pip install multiprocess
   4. 安裝 Pyrouge 套件
