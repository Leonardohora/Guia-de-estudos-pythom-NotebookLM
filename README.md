## Guia-de-estudos-pythom-NotebookLM
Um "Norte"/Guia de estudos do python usando o NotebookLM


  ## **Contexto**

Este projeto foi desenvolvido como parte do desafio da DIO utilizando o NotebookLM como ferramenta de aprendizagem ativa.

O tema escolhido foi Python para automação, com foco em compreender como utilizar Python para automatizar tarefas repetitivas, aumentar produtividade e facilitar processos do dia a dia.


##  **objetivos**

- Aprender fundamentos de automação com Python;
- Entender bibliotecas utilizadas em automação;
- Utilizar IA para auxiliar no aprendizado;
- Criar prompts eficientes para estudos técnicos;
- Organizar conhecimento utilizando NotebookLM.

## **Ferramentas Utilizadas**

- Python
- NotebookLM
- ChatGPT
- GitHub
- VSCode


 ## **Fontes:**  
  
  https://www.python.org /
  https://blog.dsacademy.com.br/e-book-de-linguagem-python-do-hello-world-a-projetos-profissionais/#wrapper /
  https://www.youtube.com/watch?v=NpmFbWO6HPU /
  https://kinsta.com/blog/python-frameworks/ /
  https://selenium-python.readthedocs.io /

  Essas são as principais fontes, sendo elas, a página oficial da linguagem Python, vídeo com 9 horas de projetos    do básico ao avançado, diversos frameworks e seus objetos.


##  **Engenharia de Prompts:**

 **Prompt 1:** Me explique o que é automação com python.

 **Resultado:** Automação com Python é o uso de scripts para executar tarefas repetitivas, manuais ou complexas sem a necessidade de intervenção humana constante. 
Em vez de você clicar em botões ou mover arquivos um a um, você escreve um código que faz isso por você de forma muito mais rápida e precisa.

**Prompt 2:** Crie exemplos simples de automação usando python e o selenium
 
 **Resultado:** Automação com Python é a criação de scripts para executar tarefas repetitivas, manuais ou complexas de forma independente, sem a necessidade de intervenção humana constante

. O objetivo principal é aumentar a produtividade e permitir que você foque em problemas mais estratégicos, deixando o "trabalho chato" para o computador.

Aqui estão três exemplos simples de como isso funciona na prática:
Backup Automático de Pastas: Você pode usar a biblioteca shutil para copiar recursivamente todos os arquivos de um diretório de trabalho para uma pasta de segurança, garantindo que nada se perca.

Organização de Arquivos: Usando o módulo os, é possível criar um script que percorre uma pasta cheia de documentos, identifica padrões no nome (como a palavra "venda" ou uma extensão específica) e move cada um para sua respectiva pasta organizada.

Agendamento de Rotinas: Com a biblioteca schedule, você define que um script de limpeza de sistema ou de envio de relatórios deve rodar todos os dias em um horário exato (ex: às 08:00), permitindo que ele funcione sozinho em segundo plano.

Para avançarmos no seu curso, você prefere que eu mostre um exemplo de código para mover arquivos ou quer entender como agendar um script para rodar sozinho todos os dias?

**Promtp 3:** Crie exemplos simples de automação usando o Python e o Selenium.

 **Resultado:**  O Selenium é uma ferramenta poderosa para automatizar navegadores web, permitindo realizar desde tarefas repetitivas até testes complexos.
Como você já tem nível intermediário em Python, a sintaxe será bem direta para você.
Aqui estão três exemplos simples e práticos baseados nas fontes:
1. Navegação Básica e Captura de Dados
Este exemplo abre um site, maximiza a janela e captura o título da página para verificação.

from selenium import webdriver

# Inicia o driver (ex: Firefox ou Chrome)
browser = webdriver.Firefox()

# Abre um site e maximiza a tela
browser.get("http://www.selenium.dev")
browser.maximize_window()

# Captura e exibe o título da página
print(f"O título da página é: {browser.title}")

# Fecha o navegador
browser.quit()
2. Automação de Login
Uma das tarefas mais comuns é preencher formulários. Você localiza os campos (por ID, nome ou CSS) e usa o comando send_keys para digitar e click() para enviar.

# Supondo que o driver já esteja iniciado
browser.get("https://www.saucedemo.com/")

# Localiza os campos e preenche os dados
browser.find_element("id", "user-name").send_keys("standard_user")
browser.find_element("id", "password").send_keys("secret_sauce")

# Clica no botão de login
browser.find_element("id", "login-button").click()
3. Extração de Informações (Scraping Simples)
Você pode automatizar a busca por produtos e extrair uma lista de nomes ou preços.

Ação: Ir para uma página de resultados.
Extração: Usar um loop for para percorrer os elementos encontrados (como títulos de produtos H2) e imprimir o texto de cada um.

O Selenium também permite lidar com alertas, janelas múltiplas e até arrastar objetos (drag and drop).
Para o seu curso de análise, você prefere ver um exemplo de como extrair uma lista de preços para um CSV ou como lidar com várias abas do navegador ao mesmo tempo?.
 

## Dificuldades Encontradas

- Prompts genéricos geravam respostas superficiais;
- Algumas respostas utilizavam bibliotecas avançadas sem explicação;
- Foi necessário especificar o nível de dificuldade desejado;
- O contexto do prompt influenciou diretamente na qualidade das respostas.


##  **Miniguia de Estudo:**

   *Resumos:*
     Python é uma ótima linguagem de programação para Automações e Análises. Devido a sua simplicidade e variedades de bibliotecas, ela é muito utilizada.
     Suas principais bibliotecas são:
     - os
     - Selenium
     - Pandas
     - Pyautogui
     - shutil
     
   A automação pode ser utilizada para:
     - manipular arquivos;
     - automatizar tarefas repetitivas;
     - preencher formulários;
     - web scraping;
     - automação de planilhas

   ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)


   *glossário:*
   
   ### Automação
   Processo de executar tarefas automaticamente.
   
   ### Selenium
   Biblioteca utilizada para automação web.
   
   ### Script
   Arquivo contendo código executável.
   
   ### Web Scraping
   Extração automática de dados de sites.

   
   *Prompts reutilizaveis:*
   
   ### Explicar código
   "Explique esse código Python linha por linha."
   
   ### Criar automações
   "Crie uma automação simples em Python para organizar arquivos."
   
   ### Corrigir erros
   "Analise esse erro em Python e explique como corrigir."
