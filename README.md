# EducaConecta — Protótipo HTML (V3)

**Aprender hoje. Transformar amanhã.**

Protótipo front-end demonstrativo do EducaConecta, ecossistema digital da EaDTech para a Educação Básica (redes municipais, adaptável a redes estaduais e escolas particulares).

## Como executar

Abra `index.html` em um navegador atualizado — não há build nem dependências.

Roteiro sugerido de teste:
1. Navegue pelos cards públicos (Saeb, Enem e Encceja).
2. Entre como **Aluno** e responda ao diagnóstico de Matemática do 5º ano.
3. Alterne para **Professor** e atribua a trilha de reforço "Frações no cotidiano".
4. Volte como **Aluno** para praticar e reavaliar.
5. Entre como **Gestor** para ver o painel da rede.

O ciclo entre perfis é mantido via `localStorage` no mesmo navegador.

## Estrutura

| Arquivo | Conteúdo |
|---|---|
| `index.html` | Ponto de entrada |
| `app.js` | Páginas públicas, ambientes Aluno/Professor/Gestor e ciclo de avaliação |
| `styles.css` | Estilos |
| `assets/hero-reference.webp` | Imagem do hero da home |
| `LEIA-ME.txt` | Notas da V3 |

## Limitações

- Sem autenticação real, backend, banco de dados ou integrações Adobe (AEM/ALM ainda não utilizados).
- Dados, escolas, turmas, estudantes e indicadores são **fictícios**.
- As questões são autorais e ilustrativas; **não são itens oficiais do Inep** nem estimam proficiência oficial.

## Próximos passos

Evoluir para a V4 a partir desta base, conforme o documento de passagem de bastão: definir o recorte pedagógico do piloto, especificar o banco de questões e os relatórios por habilidade, e demonstrar o ciclo integrado com dados consistentes entre aluno, professor e gestor.
