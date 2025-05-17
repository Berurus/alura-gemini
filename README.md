# Robô Berry - Gerador de Prompts para Gemini

[![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)](https://github.com/Berurus/alura-gemini)
[![Linguagem](https://img.shields.io/badge/Linguagem-Python-blue)](https://www.python.org/)
[![Biblioteca](https://img.shields.io/badge/Biblioteca-google--generativeai-brightgreen)](https://ai.google.dev/gemini-api/docs/python_quickstart)

## Visão Geral

O Robô Berry é uma ferramenta interativa desenvolvida em Python, projetada para auxiliar na criação de prompts criativos e eficazes para o modelo de inteligência artificial Gemini do Google. 
Através de uma interface de linha de comando amigável, o Robô Berry guia o usuário por uma série de perguntas sobre a imagem desejada, gerando dois prompts distintos: 
um baseado nas escolhas do usuário e outro com sugestões da própria IA.

## Funcionalidades Principais

* **Interface Interativa:** Conduz o usuário através de perguntas claras e concisas para definir os detalhes da imagem desejada (tema, ambientação, estilo, sentimento, etc.).
* **Geração de Prompt Original:** Cria um prompt direto e objetivo com base nas respostas fornecidas pelo usuário.
* **Sugestão de Prompt Inteligente:** Utiliza a biblioteca `google-generativeai` e o modelo Gemini para gerar um prompt alternativo, explorando diferentes perspectivas e detalhes.
* **Comparação Facilitada:** Apresenta ambos os prompts (original e sugerido) para que o usuário possa escolher o mais adequado para usar no [Gemini Google](https://gemini.google.com).
* **Formatação Clara:** Utiliza cores e negrito para destacar os prompts e facilitar a leitura na saída do programa.
* **Histórico de Prompts:** Permite ao usuário visualizar um histórico dos prompts gerados durante a sessão.

## Como Usar

Para utilizar o Robô Berry, siga estes passos:

1.  **Pré-requisitos:**
    * Python 3.x instalado no seu sistema.
    * Acesso ao Google Colaboratory (Colab) é recomendado para uma experiência mais simples, especialmente para configurar a chave da API.
    * Uma chave de API do Google AI Studio. Você pode obtê-la seguindo as instruções em [https://ai.google.dev/gemini-api/docs/get_started](https://ai.google.dev/gemini-api/docs/get_started).

2.  **Instalação (Opcional - Já feito no Colab):**
    Se você estiver executando o script localmente, clone este repositório e instale as dependências:
    ```bash
    git clone [https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git](https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git)
    cd SEU_REPOSITORIO
    pip install -r requirements.txt
    ```
    *(Crie um arquivo `requirements.txt` com `google-generativeai` e `rich`)*

3.  **Configuração da Chave da API:**
    * **No Google Colab (Recomendado):**
        * Abra o notebook `.ipynb` do Robô Berry.
        * Vá em "Ambiente de execução" -> "Variáveis de ambiente".
        * Adicione uma variável com o nome `GOOGLE_API_KEY` e cole sua chave da API no valor.
        * Execute a célula de configuração da API no notebook.
    * **Localmente:**
        * Você pode definir a chave da API como uma variável de ambiente no seu sistema operacional.
        * Ou, pode modificar a célula de configuração da API no script Python para inserir sua chave diretamente (não recomendado por questões de segurança).

4.  **Execução:**
    * **No Google Colab:** Execute as células do notebook na ordem. A função `robo_berry()` iniciará a interação.
    * **Localmente:** Execute o script Python principal (`robo_berry.py` ou o nome do seu arquivo principal).
        ```bash
        python robo_berry.py
        ```

5.  **Interação:**
    * O Robô Berry fará uma série de perguntas sobre a imagem que você deseja criar. Responda a cada pergunta na linha de comando.
    * Ao final das perguntas, dois prompts serão exibidos: o Prompt Original (baseado nas suas respostas) e o Prompt do Robô Berry (sugerido pela IA).
    * Copie o prompt que você preferir e cole-o no [Gemini Google](https://gemini.google.com) para gerar a imagem.
    * Você pode optar por gerar outro prompt, visualizar o histórico ou sair do programa.

## Requisitos

* Python 3.6 ou superior.
* Biblioteca `google-generativeai`.
* Biblioteca `rich` para formatação de texto no terminal.

## Contribuição

Contribuições são bem-vindas! Se você tiver alguma sugestão de melhoria, correção de bugs ou novas funcionalidades, sinta-se à vontade para abrir uma Issue ou enviar um Pull Request.

## Licença

Este projeto está sob a licença [MIT](LICENSE) - consulte o arquivo `LICENSE` para obter detalhes.

## Autor

[Bruno Murakami] ([Berurus](https://github.com/Berurus))

---
