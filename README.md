# React + Vite

# 🏫 MinhaAppReact

Este projeto exibe os colégios com **maiores matrículas** no estado da Paraíba.

---

## 📊 Fonte dos Dados

Os dados utilizados **não são de uma API ao vivo**. O sistema lê um arquivo JSON estático (`dados_censo_pb.json`), que foi gerado por um script Python chamado **app.py**.

---

## ⚙️ Processamento dos Dados

Como o arquivo JSON contém todas as escolas do estado, o filtro final é feito no navegador pelo React:

- 🔢 **Ordenação (`.sort`)**: Organiza os colégios em ordem decrescente pelo número total de matrículas (`qt_mat_bas`).
- 🎯 **Ranking (`.slice`)**: Seleciona as 3 primeiras escolas do ranking para exibição.

---

## 🖼️ Gestão das Imagens das Escolas

Como os dados oficiais não possuem imagens das escolas, implementamos a seguinte lógica:

- 📚 **Dicionário de imagens**: Mapeia o ID da escola (`co_entidade`) para uma URL de imagem específica.
- 🖼️ **Imagem padrão (Fallback)**: Caso não haja imagem cadastrada para a escola, uma imagem padrão é exibida automaticamente via operador lógico curto-circuito (`||`).

---

<div align="center">
  <sub>Projeto desenvolvido com ❤️ usando React e React-Bootstrap.</sub>
</div>
