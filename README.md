# Repositório para loja do TigerOS.
Esse repositório é unicamente para adicionar, atualizar ou remover aplicações da loja do TigerOS, a Tiger Store.

# API e tradução.

Utilizamos uma API externa disponibilizada pelo o Flathub. Conferido e curado semanalmente as alterações, é feito a tradução do summary, existente no JSON em lista, e description, existente no JSON para detalhes. A tradução é realizada pela a IA (ChatGPT, Gemini, etc) utilizando o seguinte prompt. 

**ATENÇÃO**: É recomendado que faça a tradução de uma lista de 6 items (JSON) no total. Ou seja, a cada prompt traduza apenas 6 JSON. Isso garante uma certa exatidão na respota do prompt, acima disso, pode ser que quebre. 

## Prompt para traduzir uma lista de aplicações.
```
Traduza a lista JSON até o final que está neste prompt. Traduza os campos summary na lista JSON deste prompt, me retorne a lista JSON orginal com a tradução. Retorne a lista completa. 

[
    {
        exemplo-item 1; dados para serem traduzidos.
    },
    {
        exemplo-item 2; dados para serem traduzidos.
    },
    {
        exemplo-item 3; dados para serem traduzidos.
    },
    ...
]
```

## Prompt para traduzir uma aplicação.
```
Traduza o JSON até o final que está neste prompt. Traduza os campos summary e description no JSON deste prompt, me retorne o JSON orginal com a tradução. Retorne o JSON completo. 

{
    dados para serem traduzidos.
}
```

# Como submeter aplicação ao repositório?

- Faça um fork.
- Faça uma branch em seu fork referente a submissão.
- Faça um commit, e se estiver tudo certo, abra o PR.

# Requerimentos para submeter ao repositório.

- Se for uma lista: O campo summary, obrigatoriamente, deve ser em português (pt-BR)
- Se for detalhes da aplicação: o campo summary e description, obrigatoriamente, deve ser em português (pt-BR)