# Preparar Ambiente Keras Tensorflow GPU Windows
Este repositório tem como objetivo de ensinar/relembrar como preparar um ambiente keras/tensorflow utilizando GPU no Windows.


# Baixando os arquivos

Primeiramente você deve ter realizado o donwload dos seguites softwares.

* Drivers  <a href="https://www.nvidia.com/download/index.aspx?lang=en-us">GPU NVIDIA</a> (CUDA® 11.0 requer uma versão 450.xxx ou mais recente).
* <a href="https://developer.nvidia.com/cuda-toolkit-archive">CUDA Toolkit</a> Se utilizar o CUDA 11 o TensorFlow  deve estar na versão 2.4.0 ou maior.

Após o donwload realize a instalação dos drivers e em seguida extrai o arquivo do CUDA Toolkit para uma pasta localizada em C:\tools:

<img src="https://github.com/LucasSteffens5/Preparar-Ambiente-Keras-Tensorflow-GPU-Windows/blob/main/installCuda.png" >


Edite as variaveis de ambiente. 

<img src="https://github.com/LucasSteffens5/Preparar-Ambiente-Keras-Tensorflow-GPU-Windows/blob/main/variaveisSitema.png" >

<img src="https://github.com/LucasSteffens5/Preparar-Ambiente-Keras-Tensorflow-GPU-Windows/blob/main/variaveisSistemaPath.png" >
Adicione baseado em seu diretorio as seguintes variaveis de ambiente:
```
C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.0\bin
C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.0\extras\CUPTI\lib64
C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.0\include
C:\tools\cuda\bin
```

Baixe e instale o Anaconda Navigator:

Após abra o prompt de comando do Anaconda e digite o seguinte comando:
```
conda create --name nomeDeSeuAmbiente python=3.8
```
<img src="https://github.com/LucasSteffens5/Preparar-Ambiente-Keras-Tensorflow-GPU-Windows/blob/main/promptconda.png" >

Você estara criando um ambiente com python 3.8.
Aceite todas as dependências solicitadas.

Após utilize os comandos: 
```
conda activate nomeDeSeuAmbiente

pip install tensorflow-gpu
```
Garanta que o C++ esteja instalado em sua máquina, caso não esteja instalado basta realizar o donwload neste <a href="">link</a> e instala-lo em sua versão x64.

Após preparar o ambiente com todas bibliotecas é fortemente recomendado criar um arquivo de configuração para backup, basta executar o comando no prompt do conda.

```
conda env create -f environment. yml
```


Para restaurar futuramente use:
```
conda env create -f environment.yml
```
