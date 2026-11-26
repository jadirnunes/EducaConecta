# EducaConecta — Protótipo HTML (V4)

**Aprender hoje. Transformar amanhã.**

Protótipo front-end demonstrativo do EducaConecta, ecossistema digital da EaDTech para a Educação Básica (redes municipais, adaptável a redes estaduais e escolas particulares).

## Como executar

Abra `index.html` em um navegador atualizado — não há build nem dependências.

Roteiro sugerido de teste:
1. Navegue pela **Biblioteca BNCC** (temas com faces aluno, professor e família) e pelos cards Saeb, Enem e Encceja.
2. Entre como **Aluno** e responda ao diagnóstico de Matemática do 5º ano.
3. Alterne para **Professor** > **Montar reforço**: combine temas sugeridos pelo diagnóstico e publique o curso.
4. Volte como **Aluno** > **Meu reforço**, conclua os temas, pratique e reavalie.
5. Entre como **Responsável** para acompanhar a evolução e o reforço dos filhos.
6. Entre como **Gestor** > **Rede e cadastros** para navegar Estado → Regional → Escola → Série → Turma → Aluno.

O ciclo entre perfis é mantido via `localStorage` no mesmo navegador.

## Novidades da V4

- **Hierarquia de cadastros:** Estado → Regional → Escola → Série → Turma → Turma por disciplina → Aluno, com indicadores agregados em cada nível.
- **Perfil Responsável:** evolução por habilidade em linguagem simples, reforço atribuído e dicas para ajudar em casa.
- **Biblioteca por tema:** 24 temas indexados por metadados BNCC, cada um com face do aluno, do professor (plano de aula e materiais) e da família.
- **Montagem de curso de reforço:** o diagnóstico sugere temas; o professor combina, ordena e publica.
- **Tema transversal:** Educação Financeira em vários componentes e anos.

## Estrutura

| Arquivo | Conteúdo |
|---|---|
| `index.html` | Ponto de entrada |
| `app.js` | Base V3: páginas públicas, ambientes Aluno/Professor/Gestor e ciclo de avaliação |
| `v4.js` | Camada V4: hierarquia, perfil Responsável, biblioteca por tema e montagem de reforço |
| `styles.css` / `v4.css` | Estilos |
| `assets/hero-reference.webp` | Imagem do hero da home |
| `LEIA-ME.txt` | Notas da V4 |

## Limitações

- Sem autenticação real, backend, banco de dados ou integrações Adobe (AEM/ALM ainda não utilizados).
- Dados, escolas, turmas, estudantes e indicadores são **fictícios**.
- As questões são autorais e ilustrativas; **não são itens oficiais do Inep** nem estimam proficiência oficial.

## Próximos passos

Validar pedagogicamente os temas e códigos BNCC, definir o recorte do piloto (MVP), especificar o banco de questões e substituir os dados simulados por cadastros reais da rede.
