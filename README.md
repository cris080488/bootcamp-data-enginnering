#Projeto: Pacote de Processamento de Imagens

##Autora do Projeto: Karina Kato

Aula: Coding Lab PRO - Digital Innovation One
(clique aqui para ver o meu perfil na plataforma)

Tecnologia: Python
Data: 22/08/2020
###Descrição
O pacote "image_processing-test" é usado para:

Módulo "Processing":

Correspondência de histograma;
Similaridade estrutural;
Redimensionar imagem;
Módulo "Utils":

Ler imagem;
Salvar imagem;
Plotar imagem;
Resultado do gráfico;
Plotar histograma;
Passo a passo da configuração para hospedar um pacote em Python no ambiente de testes Test Pypi
 Instalação das últimas versões de "setuptools" e "wheel"
´´´py -m pip install --user --upgrade setuptools wheel´´´
 Tenha certeza que o diretório no terminal seja o mesmo do arquivo "setup.py"
C:\User\Henrique\image-processing-package> py setup.py sdist bdist_wheel
 Após completar a instalação, verifique se as pastas abaixo foram adicionadas ao projeto:

 build;
 dist;
 image_processing_test.egg-info.
 Basta subir os arquivos, usando o Twine, para o Test Pypi:

py -m twine upload --repository testpypi dist/*
 Após rodar o comando acima no terminal, será pedido para inserir o usuário e senha. Feito isso, o projeto estará hospedado no Test Pypi.hospedá-lo no Pypi diretamente.
Aqui o objetivo não é utilizar o projeto da Karina para postar em meu perfil do Pypi pessoal, visto que o projeto é dela. Ainda não tenho nenhum projeto que possa ser utilizado como pacote.
No entanto, tenha em mente que o Test Pypi, como o próprio nome diz, é apenas um ambiente de testes. Para que o projeto esteja disponível como um pacote para ser usado publicamente, é necessário hospedá-lo no site oficial do Pypi.
Instalação local, após hospedagem no Test Pypi
 Instalação de dependências
´´´pip install -r requirements.txt´´´
 Instalção do Pacote
Use o gerenciador de pacotes pip install -i https://test.pypi.org/simple/ image-processing-test para instalar image_processing-test

´´´pip install image-processing-test´´´
Como usar em qualquer projeto
´´´from image-processing-test.processing import combination
combination.find_difference(image1, image2)´´´


Autor (quem hospedou o projeto no Test Pypi)
Cristiano Oliveira da Silva

Licença
MIT
