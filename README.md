#  Clube do Jogo

Este repositório contém o código-fonte da *landing page* oficial do nosso **Clube do Jogo**. O objetivo da página é apresentar as sugestões de games de cada membro, com os respectivos trailers, sinopses, preços e informações técnicas, centralizando a votação para os nossos encontros.

🌐 **Acesse a página aqui:** [Insira aqui o link do seu GitHub Pages]

---

## 👥 Integrantes
O clube é composto por 6 membros:
* Bernardo
* João Pedro
* João Victor
* Navarro
* Pedro
* Renan

---

## 📜 Regras do Clube

Para garantir a dinâmica e o sucesso dos nossos encontros, adotamos as seguintes diretrizes iniciais:

1. **Duração dos Jogos:** As sugestões devem focar em jogos com uma campanha principal curta, idealmente entre **5 a 10 horas** de duração, para que todos consigam conciliar com a rotina.
2. **Sistema de Votação:** A escolha do próximo jogo é feita de forma democrática através da página.
3. **Voto de Minerva (Fair Play):** **Não é permitido votar na própria sugestão.** Isso nos força a avaliar as propostas dos outros e a sair da nossa zona de conforto.

---

## 📊 Histórico e Status dos Jogos

Para mantermos um registro do que já passou pelo clube e organizar nossas planilhas de acompanhamento, utilizamos as seguintes nomenclaturas:
* **Concluído:** O jogo foi finalizado pela maioria e devidamente discutido na nossa reunião.
* **Bloqueado:** O grupo decidiu abandonar o título no meio da jornada ou mudou de abordagem, descartando a ideia de continuar investindo tempo nele.
* **Na Fila:** Títulos aprovados na votação que estão aguardando o início do seu respectivo ciclo.

---

## 🛠️ Como Adicionar um Novo Jogo

Quando um membro sugerir um novo jogo ou mudar de ideia, a página pode ser atualizada editando o arquivo `index.html` diretamente no GitHub:

### 1. Fundo Temático (CSS)
Na tag `<style>`, adicione o ID do jogo com a imagem de fundo e o filtro de escurecimento (`rgba`):

```css
#id-do-jogo { 
    background-image: linear-gradient(rgba(0, 0, 0, 0.8), rgba(0, 0, 0, 0.8)), url('LINK_DA_IMAGEM'); 
}
```

### 2. Estrutura do Jogo (HTML)
No `<body>`, logo antes da seção de votação final, cole o bloco padrão preenchendo as informações e o link de incorporação (`/embed/`) do YouTube:

```html
<section id="id-do-jogo" class="game-section">
    <div class="game-content">
        <h2>Título do Jogo</h2>
        <iframe src="[https://www.youtube.com/embed/CODIGO_DO_VIDEO](https://www.youtube.com/embed/CODIGO_DO_VIDEO)" allowfullscreen></iframe>
        <p>Sinopse oficial da Steam ou descrição do jogo.</p>
        <div class="game-tags">
            <span class="tag price-tag">R$ Preço</span>
            <span class="tag">Tag 1</span>
            <span class="tag">Tag 2</span>
        </div>
    </div>
</section>
```

---

## 🚀 Tecnologias Utilizadas
* HTML5
* CSS3 (Flexbox, Linear Gradients, Efeito Parallax)
* Google Forms (Incorporado para votação secreta)
* GitHub Pages (Hospedagem gratuita)
