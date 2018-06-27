---
layout: documentation
title: Integrando o Chatweb da ZCC em seu site
description: 
categories: docs
---

<style>
  iframe
  {
    width: 100%;
    height: 355px;
    border: 5px dashed black;
  }
</style>

O Chatweb da [ZCC](../) também pode ser utilizado integrado em seu site.
Existem várias configurações e possibilidades de uso, mas a integração mais básica pode
ser feita assim:

```html
<html>
  <head>
    <title>Meu site de exemplo</title>
  </head>
  <body>
    <div>Conteúdo Original do site.</div>

    <!-- Início do código do chat -->
    <div class="znv-chat"></div>
    <script src="https://static.zenvia.com/embed/js/zenvia-chat.min.js"></script>
    <script>
        new ZenviaChat('id-do-chat-aqui').build();
    </script>
    <!-- Fim do código do chat -->
  </body>
</html>
```


No trecho do código:
```javascript
'id-do-chat-aqui'
```
É necessário que seja utilizado um id válido de Chatweb, o qual pode ser obtido na lista de integrações.



Abaixo você pode ver um exemplo de Embedded Chatweb usando as configurações padrão (o qual pode ser acessado [aqui]({{ site.url }}/html/chat-embedded/default-config.html)):
<iframe src="{{ site.url }}/html/chat-embedded/default-config.html"></iframe>

