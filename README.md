# Gerador de QR Codes a partir de Dados Excel

Este projeto gera códigos QR a partir de dados contidos em uma planilha Excel. Utiliza as bibliotecas `qrcode` e `openpyxl` para gerar e salvar imagens de QR Codes com informações específicas extraídas da planilha.

## Requisitos

Antes de começar, você precisará instalar as seguintes bibliotecas Python. Você pode instalá-las usando `pip`:

```bash
pip install qrcode[pil] openpyxl
```

## Configurações do Código

1. **Caminho do Arquivo Excel**

   Altere a variável `path` para o caminho correto do arquivo Excel em seu sistema:

   ```python
   path = "C:\\Users\\User\\Downloads\\Qr code\\Dados.xlsx"
   ```

2. **Caminho de Salvamento dos QR Codes**

   Altere o caminho na linha onde o QR Code é salvo para o diretório desejado:

   ```python
   img.save(f"C:\\Users\\User\\Downloads\\Qr code\\QR's CODE\\QR.{str((i+1)).zfill(4)}.png")
   ```

3. **Número de QR Codes a Serem Gerados**

   Modifique o valor `4` na linha abaixo para a quantidade de QR Codes que você deseja gerar:

   ```python
   for i in range(4):
   ```

4. **Celulas de Dados**

   As células de onde os dados são extraídos são definidas pelas linhas:

   ```python
   item_1 = celula.cell(row = i+1, column = 1)
   item_2 = celula.cell(row = i+1, column = 3)
   ```

   Ajuste o índice da coluna e da linha conforme a estrutura da sua planilha.

## Executando o Código

1. Certifique-se de que as bibliotecas necessárias estão instaladas.
2. Ajuste os caminhos e configurações conforme descrito acima.
3. Execute o script Python:

   ```bash
   python nome_do_seu_script.py
   ```

## Exemplo de Saída

O código gerará imagens PNG de QR Codes com o seguinte formato de nome:

```
QR.0001.png
QR.0002.png
...
```

As imagens serão salvas no diretório especificado no código.

## Contribuição

Sinta-se à vontade para contribuir com melhorias, correções de bugs ou sugestões.
