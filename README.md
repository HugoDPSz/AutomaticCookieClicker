# 🖱️ Automatic Cookie Clicker (Selenium)

Este projeto é uma automação simples do jogo [Cookie Clicker](https://orteil.dashnet.org/cookieclicker/) usando **Python** e **Selenium WebDriver**. Foi desenvolvido como exercício prático para explorar e testar diferentes funcionalidades do Selenium, como interação com elementos da página, espera explícita e lógica de automação de cliques e compras.

## 📂 Estrutura

- `CookieClicker.py`: script principal que executa a automação.
- Utiliza o **Google Chrome** com WebDriver para navegar e interagir com a página.

## 🧠 O que o script faz?

1. Abre o site do Cookie Clicker.
2. Seleciona o idioma "English".
3. Começa a clicar continuamente no cookie principal (`bigCookie`).
4. A cada clique, verifica a quantidade de cookies disponíveis.
5. Compara com os preços dos primeiros upgrades (produtos `0` a `3`) e compra se possível.

## ⚙️ Pré-requisitos

- Python 3.7+
- [Google Chrome](https://www.google.com/chrome/)
- [ChromeDriver](https://sites.google.com/a/chromium.org/chromedriver/) compatível com sua versão do navegador
- Instale os pacotes necessários com:

```bash
pip install selenium
```

## 🚀 Como rodar

1. Altere o caminho do ChromeDriver no script, se necessário:
   ```python
   service = Service(r"C:\Users\user\Desktop\chromedriver\chromedriver.exe")
   ```

2. Execute o script:
   ```bash
   python CookieClicker.py
   ```

## 📌 Observações

- Este projeto é **experimental e educativo**.
- Foi desenvolvido com base em um tutorial, com adaptações e testes próprios.
- Serve como ponto de partida para aprender automação de tarefas web com Selenium.

## 📚 Aprendizados

Durante o desenvolvimento, foram testados e aplicados:
- Esperas explícitas (`WebDriverWait` e `EC.presence_of_element_located`)
- Localização de elementos por `ID` e `XPath`
- Conversão e manipulação de strings numéricas
- Estrutura de repetição com lógica de compra
