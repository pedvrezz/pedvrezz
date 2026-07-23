# Como publicar o README animado

O GitHub só mostra o README especial do perfil quando o repositório possui exatamente o mesmo nome do usuário.

Para este perfil, o nome correto é `pedvrezz`.

## Etapa 1 — Criar o repositório

1. Entre no GitHub com a conta `pedvrezz`.
2. Clique em **New repository**.
3. Em **Repository name**, digite `pedvrezz`.
4. Marque o repositório como **Public**.
5. Não é necessário adicionar outro README, pois este pacote já contém um.
6. Crie o repositório.

## Etapa 2 — Enviar os arquivos

Envie tudo que existe dentro da pasta `pedvrezz-github-profile`, preservando a estrutura:

```text
pedvrezz/
├── README.md
├── SETUP.md
├── assets/
│   ├── banner.svg
│   ├── github-contribution-grid-snake.svg
│   └── github-contribution-grid-snake-dark.svg
└── .github/
    └── workflows/
        └── snake.yml
```

A pasta `.github` começa com ponto e pode ficar oculta no Windows. Não deixe essa pasta de fora.

## Etapa 3 — Gerar a cobra de contribuições

1. Abra o repositório `pedvrezz`.
2. Entre na aba **Actions**.
3. Se o GitHub pedir autorização para workflows, habilite-os.
4. Abra **Generate contribution snake**.
5. Clique em **Run workflow**.
6. Depois que a execução terminar, atualize seu perfil.

Os arquivos provisórios serão substituídos pelas animações geradas. Depois disso, o workflow atualizará a cobra automaticamente todos os dias.

## Etapa 4 — Publicar os projetos

A seção de projetos já aponta para:

```text
netforge-iac
lantern-cpp
infrapulse-dotnet
leonardo-deskpad
```

Publique os quatro repositórios usando exatamente esses nomes. Enquanto ainda não estiverem publicados, os links retornarão página não encontrada.

## Observação sobre as estatísticas

Os cartões usam a instância pública do `github-readme-stats`. Ela pode falhar temporariamente por limite de requisições. Isso não significa que seu README esteja errado. O banner e a cobra ficam no seu próprio repositório.
