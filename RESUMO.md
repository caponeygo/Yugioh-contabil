# Resumo: CFC do Ygo

## O que é
App de flashcards para o Exame de Suficiência CFC 2026, em um único HTML, sem build nem dependências. O progresso fica salvo no `localStorage` do navegador.

## O que o app faz (Vol. 3, 50 questões)
- Questões de 4 alternativas com explicação após responder
- Disciplinas intercaladas, como na prova real
- Filtro por disciplina
- Botão para embaralhar questões e alternativas
- Botão para revisar só as erradas
- Botão para zerar o progresso
- Placar, barra de progresso e tema claro/escuro automático
- Atalhos: `←` `→` navegam e `A`–`D` respondem

## Estrutura do repo
```
cfc-do-ygo/
├── index.html        # app atual (Vol. 3)
├── volumes/vol-3.html
├── README.md
└── RESUMO.md
```

## Criar o git local (na pasta com os arquivos)
```
git init -b main
git add -A
git commit -m "Flashcards Exame CFC 2026 - Vol. 3"
gh repo create cfc-do-ygo --public --source=. --push
```

Sem o `gh`, crie o repo vazio em github.com/new e rode:
```
git remote add origin https://github.com/caponeygo/cfc-do-ygo.git
git push -u origin main
```

## Abrir no celular
Ative o GitHub Pages em Settings → Pages → branch `main`, pasta `/ (root)`.

## Próximos passos
1. Separar as questões em `questoes/vol-N.json`, para o HTML só carregar os dados.
2. Criar novos volumes (Vol. 4 em diante).
3. Opcional: seletor de volume e PWA para uso offline.
