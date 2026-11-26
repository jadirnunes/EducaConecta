# EducaConecta — Protótipo HTML

**Aprender hoje. Transformar amanhã.**

Protótipo front-end demonstrativo do EducaConecta, ecossistema digital da EaDTech para a Educação Básica (redes municipais, adaptável a redes estaduais e escolas particulares).

## Como executar

Abra `index.html` em um navegador atualizado — não há build nem dependências.

Roteiro sugerido de teste:
1. Navegue pela **Biblioteca BNCC** (temas com faces aluno, professor, família e gestor) e pelos cards Saeb, Enem e Encceja.
2. Entre como **Aluno** e responda ao diagnóstico de Matemática do 5º ano.
3. Alterne para **Professor** > **Montar reforço**: combine temas sugeridos pelo diagnóstico e publique o curso.
4. Volte como **Aluno** > **Meu reforço**, conclua os temas, pratique e reavalie.
5. Entre como **Responsável** para acompanhar a evolução e o reforço dos filhos.
6. Entre como **Gestor** > **Rede e cadastros** para navegar Estado → Regional → Escola → Série → Turma → Aluno.

O ciclo entre perfis é mantido via `localStorage` no mesmo navegador.

## Principais recursos

- **Hierarquia de cadastros:** Estado → Regional → Escola → Série → Turma → Turma por disciplina → Aluno, com indicadores agregados em cada nível.
- **Perfil Responsável:** evolução por habilidade em linguagem simples, reforço atribuído com dicas para ajudar em casa, calendário escolar e comunidade de pais moderada pela escola, com guias de boas práticas.
- **Biblioteca por tema:** 24 temas indexados por metadados BNCC, cada um com face do aluno, do professor (plano de aula e materiais), da família e do gestor (uso do tema na rede).
- **Montagem de curso de reforço:** o diagnóstico sugere temas; o professor combina, ordena e publica.
- **Tema transversal:** Educação Financeira em vários componentes e anos, com base no programa de Educação Financeira do Banco Central (Aprender Valor).

## Estrutura

| Arquivo | Conteúdo |
|---|---|
| `index.html` | Ponto de entrada |
| `app.js` | Páginas públicas, ambientes Aluno/Professor/Gestor e ciclo de avaliação |
| `extensoes.js` | Hierarquia de cadastros, perfil Responsável, biblioteca por tema e montagem de reforço |
| `styles.css` / `extensoes.css` | Estilos |
| `assets/hero-reference.webp` | Imagem do hero da home |
| `LEIA-ME.txt` | Roteiro rápido |

## Limitações

- Sem autenticação real, backend, banco de dados ou integrações Adobe (AEM/ALM ainda não utilizados).
- Dados, escolas, turmas, estudantes e indicadores são **fictícios**.
- As questões são autorais e ilustrativas; **não são itens oficiais do Inep** nem estimam proficiência oficial.

## Próximos passos

Validar pedagogicamente os temas e códigos BNCC, definir o recorte do piloto (MVP), especificar o banco de questões e substituir os dados simulados por cadastros reais da rede.
