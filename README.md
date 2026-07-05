# ScrapingManga - Mundo dos Infinitos

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)
![Selenium](https://img.shields.io/badge/Selenium-Web%20Scraping-43B02A?logo=selenium&logoColor=white)
![Status](https://img.shields.io/badge/Status-Concluído-success)
![License](https://img.shields.io/badge/License-MIT-blue)

Projeto desenvolvido em Python utilizando Selenium para automatizar a coleta de informações de mangás e seus respectivos volumes no site Mundo dos Infinitos.

O sistema realiza a pesquisa de uma obra, acessa sua coleção, organiza os volumes em ordem crescente e extrai informações detalhadas sobre o mangá e cada edição disponível.

---

## Estrutura do Projeto

```text
MangaScraper
├── coletaManga.py
├── requirements.txt
├── LICENSE
└── README.md
```

---

## Funcionalidades

### Coleta de Dados do Mangá

* Pesquisa automática por nome
* Acesso à coleção da obra
* Captura da capa principal
* Captura do título
* Captura do autor
* Captura da editora
* Captura da demografia
* Contagem total de volumes

### Coleta de Dados dos Volumes

* Navegação automática por todos os volumes
* Captura da capa de cada edição
* Captura do ISBN
* Armazenamento dos dados em memória
* Coleta em ordem crescente dos volumes

---

## Fluxo da Automação

1. Acessa o site Mundo dos Infinitos
2. Pesquisa o mangá informado pelo usuário
3. Abre o primeiro resultado encontrado
4. Acessa a coleção da obra
5. Ordena os volumes em ordem crescente
6. Coleta os dados gerais do mangá
7. Conta a quantidade de volumes
8. Percorre todos os volumes da coleção
9. Extrai capa e ISBN de cada edição
10. Armazena os dados coletados

---

## Dados Coletados

### Mangá

| Campo | Descrição |
|---------|---------|
| Título | Nome da coleção |
| Capa | Imagem principal da obra |
| Autor | Autor do mangá |
| Editora | Editora responsável |
| Demografia | Público-alvo da obra |
| Quantidade de Volumes | Total encontrado na coleção |

### Volume

| Campo | Descrição |
|---------|---------|
| Capa | Imagem da edição |
| ISBN | Código ISBN do volume |

---

## Site Utilizado

https://mundosinfinitos.com.br/

---

## Ferramentas Utilizadas

<div align="center">

<img width="60" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg"/>

<img width="60" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/selenium/selenium-original.svg"/>

<img width="60" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg"/>

<img width="60" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg"/>

</div>

<br>

| Ferramenta | Descrição |
|------------|------------|
| Python | Linguagem utilizada para desenvolver a automação |
| Selenium | Biblioteca responsável pela automação do navegador |
| ChromeDriver | Controle do navegador Google Chrome |
| VS Code | Ambiente de desenvolvimento |
| Git | Controle de versão |
| XPath | Localização de elementos HTML |
| CSS Selectors | Navegação e identificação de componentes da página |

---

## Instalação

Clone o repositório:

```bash
git clone https://github.com/seu-usuario/MangaScraper.git
```

Acesse a pasta:

```bash
cd MangaScraper
```

Instale as dependências:

```bash
pip install selenium requests
```

Caso utilize ambiente virtual:

```bash
python -m venv venv

# Windows
venv\Scripts\activate

# Linux/Mac
source venv/bin/activate

pip install selenium requests
```

---

## Executando

Execute o script:

```bash
python coletaManga.py
```

Informe o nome do mangá quando solicitado:

```text
Digite o nome do manga:
One Piece
```

O sistema realizará toda a navegação e exibirá os dados coletados no terminal.

---

## Exemplo de Saída

```text
Título: One Piece

Autor: Eiichiro Oda

Editora: Panini

Demografia: Shounen

Quantidade de volumes: 110

Volume 1 -> ISBN: 9788573516973

Volume 2 -> ISBN: 9788573516980

Volume 3 -> ISBN: 9788573516997
```

---

## Conceitos Aplicados

* Web Scraping
* Automação de Navegadores
* Selenium WebDriver
* XPath
* CSS Selectors
* Manipulação de Dados
* Navegação entre Páginas
* Extração de Informações
* Estruturas de Repetição
* Tratamento de Elementos Dinâmicos

---

## Aviso

Este projeto foi desenvolvido para fins de estudo e prática de automação web.

Antes de realizar coletas automatizadas em qualquer site, consulte os Termos de Uso, as políticas de acesso e o arquivo `robots.txt` da plataforma.

---

## Licença

Este projeto está licenciado sob a licença MIT. Consulte o arquivo LICENSE para mais informações.

---

## Autor

Lucas Iber Dias

Estudante de Análise e Desenvolvimento de Sistemas com foco em Desenvolvimento Full Stack, Automação e Web Scraping.
