---
title: Como a WEB funciona
description: Ao acessar sites como Google ou Facebook um usuário comum não tem noção do que acontece, ele apenas quer que a página carregue. E o mais rápido possível! Nesse artigo vamos conhecer um pouco sobre esse processo. 
tags:
  - internet
authors:
  - danilodcn
---

{% for author in authors %}
  {% with data = authors_list.get(author)%}
  <div class="md-post__authors md-typeset"> 
    <div class="md-profile md-post__profile">
      <span class="md-author md-author--long">
      <a href=https://github.com/{{author}}/ target='blank'>
        <img src="{{ data.avatar }}" alt="{{ data.name }}">
      </a>
        </span>
          <span class="md-profile__description">
          <strong>{{ data.name }}</strong>
          <br>
          {{ data.description }}
    </span>
    </div>
  </div>
  {% endwith %}
{% endfor %}

## Internet: a rede mundial de computadores

![internet image]

O principal responsável pela WEB como a conhecemos é a `internet`. Damos o nome de internet a uma rede gigantesca de computadores espalhados por todo o mundo, de maneira que possam se comunicar. É importante salientar que a internet é feita de forma descentralizada, isso significa que ela mantida pelos próprios usuários que a compõe.

De forma simplificada a internet é o meio pelo qual a informação é transferida de um computador a outro. A essa informação damos o nome de `pacotes`. Para que esses pacotes sejam transferidos entre todas as redes, usa-se o conjunto de protocolos `TCP/IP`. Esses protocolos são constituídos por três principais protocolos: IP (_Internet Protocol_), UDP (_User Datagram Protocol_) e TCP (_Transmission Control Protocol_).

 - __IP__: Cada computador conectado à internet precisa de um número de identificação único, a esse número damos o nome de __Endereço IP__. Esse número possui 16 bits, constituído por uma sequencia de 4 números, por exemplo o meu IP atual é: 192.168.2.7.
 - __UDP__: 


<!-- image section -->
[internet image]: internet.jpg 