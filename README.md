# Ferramentas para a redação

Busca demonstrativa em acervo de vídeos e preparação de fotografias em lote. As fotos são processadas no navegador, sem upload. O acervo usa dados de exemplo.

Projeto criado na oficina Codesinfo · REC’n’Play, Recife, 13 de novembro de 2026.

- [Demonstração da oficina](https://codesinfo-ferramentas.burgos.chatgpt.site/)
- Slug preservado: `codesinfo-ferramentas`.
- Esta cópia é independente do ambiente de hospedagem original. Não contém chaves de API nem o histórico privado de desenvolvimento.

## Instalação e execução

Requisito: Python 3 para servir os arquivos (nenhum pacote adicional).

```sh
git clone https://github.com/BurgosNY/codesinfo-ferramentas.git
cd codesinfo-ferramentas
python3 -m http.server 8000 --bind 127.0.0.1 --directory dist
```

Abra http://localhost:8000. Para publicar, hospede o conteúdo de `dist/` em qualquer hospedagem estática.

## IA e chaves

A interface e o fluxo principal deste projeto **não precisam de chave de API**. Não adicione uma chave ao JavaScript do navegador. OpenAI não é uma dependência obrigatória.

## Módulos

- `dist/fotos.html`: abre também com duplo clique, sem servidor; processa fotos localmente e baixa ZIP. Originais não são modificados.
- `dist/acervo.html`: busca no catálogo demonstrativo; não é um servidor de vídeos de uma emissora.
- `preserved-pauta-local/`: protótipo anterior preservado, separado da versão atual.

## Limites e uso editorial

Protótipo de oficina, não produto auditado para produção. Revise resultados, datas, contexto e fontes antes de publicar. Demonstrações históricas não indicam que a informação continua atual. Marcas e materiais de terceiros mantêm seus direitos; consulte `ASSETS.md`.
