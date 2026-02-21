<h1 align="center"> Leitor de Texto </h1>

<p align="center">
Projeto simples de leitor de texto em voz (Text-to-Speech) usando a API de síntese de voz do navegador.
</p>

<p align="center">
  <a href="#-tecnologias">Tecnologias</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-projeto">Projeto</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-layout">Layout</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-licença">Licença</a>
</p>

<p align="center">
  <img alt="License" src="https://img.shields.io/static/v1?label=license&message=MIT&color=49AA26&labelColor=000000">
</p>

<br>

## 🚀 Tecnologias

O projeto foi desenvolvido com:

- HTML5 — estrutura da página
- CSS3 — estilo visual
- JavaScript — lógica do leitor de texto e síntese de voz

## 💻 Projeto

Esse projeto é uma aplicação web leve que permite ao usuário digitar um texto e ouvir esse texto sendo narrado em voz em português brasileiro. Ele foi criado com HTML, CSS e JavaScript usando a interface de SpeechSynthesis do navegador.

## 1. 🚀 Funcionalidades

- ✔️ Recebe texto do usuário
- ✔️ Converte texto em fala em português do Brasil (pt-BR)
- ✔️ Interface limpa e responsiva

## 2. 🧠 Como funciona

O usuário digita ou cola um texto na caixa disponível e clica no botão para que o sistema converta o texto em áudio usando o recurso nativo de síntese de voz do navegador.

## 📌 3. Exemplo de código principal

``` js
const textarea = document.getElementById('text'),
      button = document.getElementById('btn')

button.addEventListener('click', () => {
  const text = textarea.value,
        speak = new SpeechSynthesisUtterance(text);

  speak.lang = 'pt-br';
  window.speechSynthesis.speak(speak);
});
```

## :memo: Licença

Esse projeto está sob a licença MIT.
