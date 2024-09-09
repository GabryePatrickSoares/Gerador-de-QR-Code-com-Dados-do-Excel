# Gerador-de-QR-Code-com-Dados-do-Excel

```markdown
# Gerador de QR Code a partir de Dados do Excel

Este projeto é uma ferramenta simples para gerar códigos QR a partir dos dados de uma planilha do Excel. O código lê os dados de uma planilha e gera um código QR para cada entrada, salvando as imagens resultantes em um diretório específico.

## Requisitos

Antes de executar o script, você precisará instalar as seguintes bibliotecas Python:

- `qrcode`
- `openpyxl`

Você pode instalar essas bibliotecas usando o `pip`:

```bash
pip install qrcode[pil] openpyxl
```

## Como Usar

1. **Prepare sua planilha Excel:**
   - Certifique-se de que seu arquivo Excel esteja no formato `.xlsx`.
   - Os dados devem estar na primeira coluna da primeira planilha.

2. **Configure o caminho do arquivo Excel e o diretório de saída:**
   - Edite o script para apontar para o caminho correto do seu arquivo Excel substituindo `"C:\\###\\###\\###\\###\\Dados.xlsx"`.
   - Substitua o caminho de saída do arquivo na linha `img.save(f"###\QR.{str((i+1)).zfill(4)}.png")` pelo diretório onde você deseja salvar as imagens dos códigos QR.

3. **Execute o script:**
   - Certifique-se de que o Python esteja instalado em seu sistema.
   - Execute o script Python:

   ```bash
   python nome_do_seu_script.py
   ```

   Certifique-se de substituir `nome_do_seu_script.py` pelo nome real do seu script.

## Contribuição

Sinta-se à vontade para contribuir com melhorias ou correções.

---
