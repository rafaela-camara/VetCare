# 🐾 VetCare - Clínica Veterinária e Centro Diagnóstico

O **VetCare** é uma aplicação web desenvolvida como projeto de simulação de ambiente profissional front-end. O objetivo é apresentar a estrutura, especialidades, corpo clínico, diferenciais e informações de atendimento do hospital veterinário de forma moderna, intuitiva e totalmente acessível.

## 🛠️ Tecnologias e Conceitos Aplicados

O projeto foi construído utilizando tecnologias modernas de desenvolvimento web, com foco em boas práticas de arquitetura, semântica e acessibilidade:

* **HTML5 Semântico:** Estruturação correta das páginas utilizando tags semânticas (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<details>`, `<summary>`, `<footer>`) para garantir acessibilidade e SEO.

* **CSS3 Avançado:**

  * **Variáveis CSS (Design System Tokens):** Uso de `:root` para centralizar paleta de cores, tipografia, sombras e tempos de transição.

  * **Flexbox:** Construção do layout responsivo, alinhamento de componentes e distribuição dos cards.

  * **Unidades Relativas e Escala REM:** Configuração da escala base do elemento raiz (`html { font-size: 62.5%; }` ou proporcional) para garantir acessibilidade e uso estrito de `rem`, `%`, `vh` e `vw`.

* **Metodologia BEM (Block Element Modifier):** Padrão rigoroso de nomenclatura de classes para manter a manutenibilidade e evitar acoplamento no CSS (ex.: `.card`, `.card__title`, `.card--highlight`).

* **Design Responsivo & Mobile-First / Media Queries:** Adaptação fluida do layout para smartphones, tablets e desktops.

* **Microinterações:** Efeitos sutis com `:hover`, `:focus` e transições suaves (`transition`, `box-shadow`, `transform`).

* **Integração com APIs e Serviços Externos:**

  * **Google Fonts:** Importação da família tipográfica *Poppins* (pesos 400, 500, 600 e 700).

  * **WhatsApp Business API:** Link dinâmico no botão flutuante direcionado ao número oficial do SENAI Henrique Lupo.

## 📁 Organização da Arquitetura de Arquivos

Para garantir a separação rigorosa de responsabilidades (RNF04) e facilitar a manutenção, o projeto foi organizado na seguinte estrutura de diretórios:

```
vetcare/
│
│  ── css/
│      ├── variables.css      # Variáveis globais do Design System (tokens)
│      ├── reset.css          # Reset CSS, estilos globais e regras de raiz (REM)
│      ├── responsive.css     # Estilos de cards, botões e elementos reutilizáveis      # Estrutura do menu lateral, seções e rodapé
│      └── style.css          # Arquivo principal que importa/consolida as folhas de estilo
│                             # Imagens do projeto e ícones
├── index.html                # Documento HTML principal da aplicação
└── README.md                 # Documentação do projeto

```

## 🚀 Instruções de Visualização e Execução

Para visualizar ou executar o projeto localmente em sua máquina, siga os passos abaixo:

### Pré-requisitos

* Um navegador web moderno (Google Chrome, Mozilla Firefox, Microsoft Edge, Safari, etc.).

* Opcional: Extensão **Live Server** no VS Code.

### Passos para Execução

1. **Clonar o Repositório:**

   ```
   git clone https://github.com/seu-usuario/vetcare.git
   
   ```

2. **Navegar até a pasta do projeto:**

   ```
   cd vetcare
   
   ```

3. **Abrir o projeto:**

   * **Opção 1:** Clique duas vezes no arquivo `index.html` para abri-lo diretamente no navegador.

   * **Opção 2:** Se estiver utilizando o **VS Code**, abra a pasta no editor, clique com o botão direito no arquivo `index.html` e selecione **"Open with Live Server"**.

## 🧠 Principais Desafios Técnicos e Aprendizados

Durante o desenvolvimento deste projeto, surgiram desafios importantes que consolidaram aprendizados fundamentais para a rotina de um desenvolvedor front-end:

1. **Arquitetura de Layout com Menu e Rodapé Fixos (Fixed Positioning):**

   * *Desafio:* Garantir que a barra lateral fixa e o rodapé fixo não cobrissem o conteúdo das seções durante a rolagem e que o clique nos links do menu levasse o usuário exatamente ao início visível da seção (`scroll-margin-top` / `scroll-behavior`).

   * *Aprendizado:* Domínio das propriedades de posicionamento (`position: fixed`), gestão de espaçamentos (`padding`/`margin`) e ajuste fino de rolagem suave em CSS.

2. **Ajuste da Escala REM e Acessibilidade:**

   * *Desafio:* Substituir completamente o uso de pixels por unidades relativas (`rem`, `%`, `vh`, `vw`), mantendo a precisão visual do layout conforme o Design System.

   * *Aprendizado:* Compreensão profunda sobre acessibilidade tipográfica, escalabilidade de interface e como o controle da fonte base (`html`) impacta a responsividade em diferentes dispositivos.

3. **Padronização e Rigor com a Metodologia BEM:**

   * *Desafio:* Manter uma estrutura limpa e sem sobreposição de seletores genéricos em arquivos CSS separados.

   * *Aprendizado:* Aplicação prática do padrão BEM, promovendo reutilização de componentes e facilitando a leitura e manutenção do código.

4. **Componentização Semântica do FAQ:**

   * *Desafio:* Implementar uma seção interativa do tipo "Sanfona/Accordion" de forma nativa e acessível sem o uso de JavaScript.

   * *Aprendizado:* Utilização das tags HTML5 `<details>` e `<summary>`, aproveitando recursos semânticos do próprio navegador para melhorar a usabilidade e a acessibilidade.

🔒 **Desenvolvido para fins educacionais - VetCare 2026**