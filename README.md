# AuulaLP10
PYTHON
# Solicita o nome do arquivo e os parâmetros
nome_arquivo = input("Digite o nome do arquivo: ")
num_parametros = int(input("Quantos parâmetros você deseja inserir? "))

# Abre o arquivo para escrita
with open(nome_arquivo, "w", encoding="utf-8") as f:
    for i in range(num_parametros):
        parametro = input(f"Digite o parâmetro {i+1}: ")
        f.write(parametro + "\n")

print(f"Parâmetros escritos no arquivo {nome_arquivo}")
