# Faculdade Hogwars — Projeto Web Interativo

## 🧩 Descrição Geral do Projeto

Este projeto foi desenvolvido como parte da atividade prática da disciplina de **Programação Web com HTML, CSS e JavaScript**.

O objetivo é aplicar os conceitos aprendidos em aula, estruturando o site da **Faculdade Hogwars** com HTML e CSS já fornecidos, e adicionando **funcionalidades interativas em JavaScript**, utilizando a tag `<script src="script.js"></script>` de forma externa.

---

## 📂 Estrutura de Arquivos do Projeto

/projeto-hogwars
│
├── index.html        → Página principal do site
├── style.css         → Arquivo de estilos
├── script.js         → Código JavaScript externo
└── README.md         → Documentação do projeto

Todos os arquivos devem estar na **mesma pasta**, e o `index.html` deve conter o link externo:
```html
<script src="script.js"></script>
```

---

## 🧠 Objetivos da Atividade

1. Criar um projeto utilizando **HTML, CSS e JavaScript** com estrutura organizada.  
2. Adicionar o JavaScript de forma **externa ao HTML**.  
3. Implementar **pelo menos 5 funcionalidades básicas** vistas em aula.  
4. Adicionar **pelo menos 5 funcionalidades extras** escolhidas de referências.  
5. Comentar todo o código explicando o funcionamento.  
6. Criar um arquivo `README.md` com **pelo menos 100 linhas** descrevendo o projeto.  
7. Versionar o projeto com **Git** e publicar no **GitHub**.  
8. Registrar prints das etapas e enviar tudo no **Canvas**.

---

## ⚙️ Funcionalidades Implementadas (10 no total)

### 🧩 Funcionalidades básicas (vistas em aula)

1. **console.log()**  
   - Exibe mensagens no console do navegador para depuração.  
   - Usado em vários pontos do `script.js` para verificar se funções foram carregadas corretamente.  

2. **alert(), prompt(), confirm()**  
   - Interagem com o usuário através de janelas modais.  
   - São usadas na função de boas-vindas ao clicar no botão “Inscreva-se Agora”.

3. **document.getElementById() / document.querySelector()**  
   - Utilizadas para selecionar elementos HTML e manipulá-los dinamicamente.  
   - Exemplo: selecionar o botão “Inscreva-se Agora”, o formulário de eventos e os cards de curso.

4. **addEventListener()**  
   - Adiciona eventos a elementos da página.  
   - Aplicado em botões, formulários e teclas do teclado (como atalho para modo escuro).

5. **innerHTML / textContent**  
   - Usadas para modificar o conteúdo de elementos dinamicamente.  
   - Exemplo: atualizar o relógio no rodapé em tempo real.

---

### 💎 Funcionalidades extras (referências adicionais)

6. **localStorage**  
   - Salva dados localmente no navegador (ex: e-mails da newsletter e preferência de modo escuro).  
   - Os dados permanecem mesmo após fechar o navegador.

7. **Modo Escuro (Dark Mode)**  
   - Ativado pelo atalho **Ctrl + D** ou clicando em botão específico.  
   - Usa `classList.toggle()` para alternar a classe `dark-mode` no `<body>`.  
   - Preferência é armazenada no `localStorage`.

8. **Validação de Formulários com setTimeout()**  
   - O formulário de eventos é validado antes do envio.  
   - Um `setTimeout()` simula um atraso de “envio”, exibindo mensagens de confirmação amigáveis.

9. **Math.random() e Math.floor()**  
   - Gera números aleatórios para exibir um **depoimento aleatório** ao clicar em um botão.  
   - Demonstra uso prático de números aleatórios no site.

10. **Manipulação de Arrays com map(), filter(), reduce()**  
    - Mostra exemplos no console manipulando listas de cursos.  
    - Usa métodos modernos do JavaScript para processar arrays de forma funcional.

---

## 🧮 Funcionalidades bônus implementadas (extras opcionais)

11. **Relógio em tempo real com setInterval() e Date()**  
    - Mostra a data e hora atualizadas a cada segundo no rodapé do site.

12. **Botão “Copiar Lista de Cursos” com Clipboard API**  
    - Copia automaticamente os nomes dos cursos para a área de transferência.  

13. **Botão “Gerar Relatório JSON”**  
    - Cria um arquivo `.json` com as inscrições da newsletter e permite download.  

14. **Detectar status de conexão (online/offline)**  
    - Exibe alertas quando o usuário fica offline ou volta a ficar online.  

15. **Scroll automático (decorativo)**  
    - Usa `setInterval()` para rolar a página suavemente até o final.  

---

## 💬 Descrição Técnica do Código

- Todo o código JavaScript está **separado** em `script.js`.  
- Cada bloco de código contém **comentários explicativos**.  
- Os botões são criados dinamicamente via JS e estilizados via CSS global.  
- Nenhuma parte do HTML original foi alterada, apenas manipulada via DOM.  
- O CSS adiciona **estilo moderno aos botões** com gradiente, sombra e animações suaves.  

---

## 🎨 Design e Estilo

- O projeto utiliza tons de azul como cor principal (`#0044cc`, `#007bff`).  
- Todos os botões seguem um estilo consistente:  
  - Degradê azul,  
  - Bordas arredondadas,  
  - Transições suaves,  
  - Efeitos de hover e clique.  
- O modo escuro usa tons `#0f1720` e `#e6eef8` para contraste e conforto visual.  

---

## 🧰 Tecnologias Utilizadas

| Tecnologia | Descrição |
|-------------|------------|
| **HTML5** | Estrutura da página |
| **CSS3** | Estilização visual e responsividade |
| **JavaScript (ES6)** | Lógica e interatividade |
| **LocalStorage API** | Armazenamento local |
| **Clipboard API** | Cópia automática de texto |
| **Date API** | Manipulação de datas e horas |
| **setTimeout / setInterval** | Controle de tempo e eventos repetitivos |

---

## 🧩 Como Testar o Projeto

1. Certifique-se de que os três arquivos (`index.html`, `style.css` e `script.js`) estejam na mesma pasta.  
2. Abra o arquivo `index.html` no navegador.  
3. Clique no botão “Inscreva-se Agora” para testar as interações com `alert()` e `prompt()`.  
4. Teste o filtro de cursos, newsletter, modo escuro e relógio.  
5. Use os botões flutuantes (“Copiar cursos” e “Gerar relatório”) para verificar as funções extras.  

---

## 💾 Como Publicar no GitHub (Passo a Passo)

1. Abra o projeto no **VS Code**.  
2. Abra o terminal (`Ctrl + ~`).  
3. Execute os comandos:

```bash
git init
git add .
git commit -m "Atividade Faculdade Hogwars - versão inicial"
git branch -M main
git remote add origin https://github.com/seuusuario/nome-do-repositorio.git
git push -u origin main
```

4. Verifique no GitHub se os arquivos foram enviados corretamente.  
5. Tire prints do terminal e da página publicada.  

---

## 📸 Prints que devem ser enviados no Canvas

- Print do **VS Code** com os arquivos no Explorer.  
- Print do **terminal** com os comandos Git executados.  
- Print do **repositório GitHub** com os arquivos.  
- Print da **página rodando** no navegador.  
- Print dos **botões estilizados** e das funcionalidades (modo escuro, relógio, alert etc.).  

---

## 🧾 Conclusão

O projeto da **Faculdade Hogwars** cumpre todos os requisitos propostos:

✅ HTML, CSS e JavaScript integrados corretamente.  
✅ JavaScript externo com mais de 10 funcionalidades.  
✅ Código comentado e bem estruturado.  
✅ README.md com mais de 100 linhas, explicativo e detalhado.  
✅ Uso de Git e publicação no GitHub.  
✅ Prints e documentação prontos para envio no Canvas.  

---

### ✨ Autor

**Nome:** [Seu Nome Aqui]  
**Curso:** [Nome do Curso]  
**Disciplina:** Programação Web  
**Professor(a):** [Nome do(a) Professor(a)]  
**Ano/Semestre:** 2025/2  

---

> “Educação é a arma mais poderosa que você pode usar para mudar o mundo.” — Nelson Mandela
