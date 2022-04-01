### Anaconda 安裝 ###

wget anaconda.網址 
bash XXX.sh
直接enter Y到底
最後會詢問是否添加 conda $Path 到 .bashrc中 輸入Yes


<h3>指令紀錄</h3>

建立 conda 環境

    conda create -n(name) $env_name 
若有.yml檔，則可以使用
    
    conda env create -f $conda_environment.yml -n $env_name
便可以利用人家匯出的環境編制，建立並匯入屬於自身的conda環境

匯出conda環境編制 **必須在conda環境內**

    conda env export > $environment.yml

執行conda環境

    conda activate $env_name
在conda環境下便可以安裝package

    conda install numpy
在conda環境下移除package

    conda remove $env_name numpy
離開conda環境

    conda deacitvate
移除conda環境

    conda env remove -n(name) $env_name
常用conda 指令

    conda list
    conda env list
