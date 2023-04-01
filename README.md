# Criador de Planilhas Excel
Este é um programa em Python que cria planilhas do Excel para cada mês do ano e permite que o usuário adicione informações a essas planilhas. O programa utiliza a biblioteca openpyxl para manipular os arquivos do Excel.

## Instalação
Antes de executar o programa, certifique-se de ter a biblioteca openpyxl instalada em seu sistema. Você pode instalá-la executando o seguinte comando no terminal ou prompt de comando:

_pip install openpyxl_

## Como utilizar
Para utilizar o programa, siga os seguintes passos:

Abra o terminal ou prompt de comando.
Navegue até o diretório onde o arquivo criador_planilhas_excel.py está localizado.
Execute o seguinte comando:

_python criador_planilhas_excel.py_

O programa irá solicitar o mês desejado e os dados do novo cadastro, adicionando-os à planilha correspondente ao mês escolhido.
As planilhas são salvas em uma pasta chamada planilhas, criada automaticamente pelo programa se ainda não existir.

##Limitações
Este programa possui algumas limitações:

O programa só permite que um cadastro seja adicionado por vez.
O programa não possui validação de dados, ou seja, é possível inserir dados inválidos (por exemplo, uma data de nascimento inválida).
O programa só permite que planilhas sejam criadas para os meses de 1 a 12.
O programa só permite que um cadastro seja adicionado por mês.

## Contribuição
Se você encontrar algum problema no programa ou tiver sugestões de melhoria, sinta-se à vontade para abrir uma issue ou pull request no repositório do projeto.
