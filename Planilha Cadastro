import openpyxl
import os.path

# Cria uma pasta para as planilhas, se não existir
if not os.path.exists('planilhas'):
    os.mkdir('planilhas')

while True:
    # Pede o mês desejado
    mes = input('Digite o mês desejado (1-12): ')
    if not mes.isdigit() or int(mes) < 1 or int(mes) > 12:
        print('Mês inválido. Tente novamente.')
        continue

    # Cria o nome do arquivo da planilha
    nome_arquivo = f'planilhas/{mes}.xlsx'

    # Cria a planilha se ela ainda não existir
    if not os.path.exists(nome_arquivo):
        wb = openpyxl.Workbook()
        ws = wb.active
        ws.title = f'{mes}'
        ws.append(['Nome', 'Data de Nascimento', 'CPF', 'Cidade'])
        wb.save(nome_arquivo)
    
    # Abre a planilha existente
    wb = openpyxl.load_workbook(nome_arquivo)
    ws = wb.active

    # Pede os dados do novo cadastro
    nome = input('Digite o nome: ')
    data_nascimento = input('Digite a data de nascimento (DD/MM/AAAA): ')
    cpf = input('Digite o CPF: ')
    cidade = input('Digite a cidade: ')

    # Adiciona os dados na planilha
    ws.append([nome, data_nascimento, cpf, cidade])
    wb.save(nome_arquivo)

    print('Cadastro concluído.')
