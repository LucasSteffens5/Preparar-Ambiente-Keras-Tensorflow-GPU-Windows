# Preparar Ambiente Keras Tensorflow GPU Windows
Este repositório tem como objetivo de ensinar/relembrar como preparar um ambiente keras/tensorflow utilizando GPU no Windows.


# Baixando os arquivos

Primeiramente você deve ter realizado o donwload dos seguites softwares.

* Drivers  <a href="https://www.nvidia.com/download/index.aspx?lang=en-us">GPU NVIDIA</a> (CUDA® 11.0 requer uma versão 450.xxx ou mais recente).
* <a href="https://developer.nvidia.com/cuda-toolkit-archive">CUDA Toolkit</a> Se utilizar o CUDA 11 o TensorFlow  deve estar na versão 2.4.0 ou maior.
* 



Após preparar o ambiente com todas bibliotecas é fortemente recomendado criar um arquivo de configuração para backup, basta executar o comando no prompt do conda.

'''
conda env create -f environment. yml
'''


Para restaurar futuramente use:

'''
conda env create -f environment.yml
'''
