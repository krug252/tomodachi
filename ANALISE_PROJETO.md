# 📋 Análise do Projeto Tomodachi

## 📌 Visão Geral

O **Tomodachi** é um site institucional para um restaurante de sushi localizado em Ivoti, RS. O projeto é uma aplicação web estática desenvolvida com **HTML5**, **CSS3** e **JavaScript vanilla**, focada em apresentar informações sobre o restaurante, exibir o cardápio e direcionar clientes para o sistema de pedidos online.

---

## 🏗️ Estrutura do Projeto

### Páginas Principais

- **`index.html`** - Página inicial com informações institucionais
- **`pedidos.html`** - Cardápio completo organizado por categorias
- **`cart.html`** - Protótipo de carrinho de compras (demonstração)

### Arquivos CSS

- **`styles/style.css`** - Estilos globais e variáveis CSS
- **`styles/header.css`** - Header responsivo e navegação
- **`styles/pedidos.css`** - Estilos do cardápio e overlay
- **`styles/cart.css`** - Estilos do carrinho
- **`styles/footer.css`** - Rodapé
- **`styles/newsletter.css`** - Seção de newsletter
- **`styles/ofertas.css`** - Seção de ofertas e horários
- **`styles/buffet.css`** - Informações sobre buffets
- **`styles/sobre.css`** - Seção sobre o restaurante
- **`styles/sobre..css`** - ⚠️ Possível erro de nomenclatura (dois pontos)

### Assets

- **`assets/`** - Contém todas as imagens, ícones e SVGs do projeto

---

## ✨ Funcionalidades Implementadas

### 1. Página Inicial (`index.html`)

#### Seções Principais:

- **Header Fixo (Sticky)**
  - Logo do Tomodachi
  - Menu de navegação (SOBRE, MENU, NOS ENCONTRE)
  - Link para cardápio completo
  - Responsivo para diferentes tamanhos de tela

- **Seção Hero**
  - Imagem central com arte japonesa
  - Legenda explicativa sobre o significado de "Tomodachi"

- **Seção "Sobre"**
  - História e filosofia do restaurante
  - Imagens decorativas com tema japonês
  - Texto sobre a essência da culinária japonesa

- **Seção "Ofertas"**
  - Informações sobre delivery e rodízio presencial
  - Link para sistema de pedidos online
  - Horários de funcionamento:
    - Almoço: Terça a sábado das 11h30 às 13h30
    - Jantar: Terça a domingo das 19h às 22h

- **Seção "Buffets"**
  - **Buffet Tradicional**: R$ 46,90 (almoço) / R$ 59,90 (jantar)
  - **Buffet Especial**: R$ 74,90 (almoço) / R$ 89,90 (jantar)
  - **Buffet Tomodachi**: R$ 139,00 (almoço) / R$ 159,00 (jantar)

- **Newsletter**
  - Formulário de cadastro de email
  - Validação de email em tempo real
  - Checkbox de consentimento obrigatório
  - Mensagens de feedback (sucesso/erro)
  - ⚠️ **Nota**: Apenas simulação - sem backend real

- **Footer**
  - Mapa do Google Maps integrado
  - Endereço completo do restaurante
  - Telefone de contato
  - Links para redes sociais (Instagram, WhatsApp)
  - Informações legais (CNPJ, direitos reservados)

#### Funcionalidades JavaScript:

- **Scroll Suave**: Navegação entre seções com animação suave
- **Validação de Email**: Regex para validação de formato
- **Newsletter**: Sistema de mensagens temporárias

---

### 2. Página de Pedidos (`pedidos.html`)

#### Estrutura do Cardápio:

O cardápio está organizado em **6 categorias principais**:

1. **DESTAQUES** (7 itens)
   - 4 itens visíveis inicialmente
   - 3 itens ocultos (expandir com "Ver mais")
   - Preços: R$ 89,90 a R$ 209,90

2. **ENTRADAS** (7 itens)
   - Sunomono, Sunomono Especial, Edamame, Sushi Hot
   - 3 itens adicionais ocultos
   - Preços: R$ 12,90 a R$ 29,90

3. **COMBOS** (7 itens)
   - Combos temáticos (Salmão, Atum, Peixe Branco, Camarão, etc.)
   - Preços: R$ 79,90 a R$ 99,90

4. **POKES** (7 itens)
   - Pokes variados com diferentes proteínas
   - Preço padrão: R$ 44,90

5. **TEMAKI** (7 itens)
   - Temakis variados
   - Preço padrão: R$ 25,90

6. **BEBIDAS** (7 itens)
   - Água, refrigerantes, sucos naturais
   - Preços: R$ 6,00 a R$ 10,00

#### Funcionalidades:

- **Botão "Ver mais"**: Expande itens ocultos por categoria
- **Overlay de Produto**: Estrutura HTML/CSS presente, mas **não totalmente funcional**
  - Função `abrirOverlay()` definida no JavaScript
  - Não está vinculada aos itens do cardápio
- **Link para Sistema Externo**: Redireciona para `https://tomodachi.mandarpedido.com/mobile/home`

---

### 3. Carrinho de Compras (`cart.html`)

#### Funcionalidades Implementadas:

- **Exibição de Itens**: Lista de produtos no carrinho
- **Controle de Quantidade**: Botões +/- para ajustar quantidade
- **Adicionais**: Checkboxes para molho extra e gengibre
- **Cálculo Automático**:
  - Subtotal baseado em itens e quantidades
  - Taxa de entrega fixa (R$ 10,00)
  - Total final calculado automaticamente
- **Botão Finalizar**: Presente, mas sem ação definida

#### ⚠️ Limitações:

- **Itens Estáticos**: Produtos hardcoded no HTML
- **Sem Persistência**: Não salva dados no localStorage ou backend
- **Sem Integração**: Não conectado ao sistema de pedidos real
- **Prototipo**: Apenas para demonstração visual

---

## 🎨 Design e Estilização

### Paleta de Cores

- **Fundo Principal**: `#181818` (preto suave)
- **Destaque Primário**: `#DA0037` (vermelho)
- **Texto**: Branco e cinza claro (`#ccc`)
- **Cards**: `#1c1c1c` (cinza escuro)

### Tipografia

- **Fonte Principal**: `Jost` (Google Fonts)
- **Fonte Secundária**: `Josefin Sans` (Google Fonts)
- Uso de variáveis CSS para gerenciamento de fontes

### Responsividade

O projeto possui **breakpoints bem definidos**:

- **Tablets** (768px - 1024px)
- **Mobile Grande** (481px - 767px)
- **Mobile Pequeno** (até 480px)
- **Telas Muito Pequenas** (até 320px)

#### Características Responsivas:

- Header adaptável (empilhamento em mobile)
- Menu flexível com wrap
- Imagens responsivas
- Cards de cardápio ajustáveis
- Overlay adaptado para diferentes telas

---

## 🔧 Tecnologias Utilizadas

- **HTML5**: Estrutura semântica
- **CSS3**: 
  - Variáveis CSS
  - Flexbox
  - Media Queries
  - Animações e transições
- **JavaScript (Vanilla)**: 
  - Sem frameworks
  - Manipulação do DOM
  - Event listeners
- **Google Fonts**: Jost e Josefin Sans
- **Google Maps**: Integração via iframe

---

## ⚠️ Pontos de Atenção e Melhorias Sugeridas

### 1. Integração de Pedidos

**Situação Atual:**
- O site redireciona para sistema externo (`tomodachi.mandarpedido.com`)
- Carrinho local é apenas protótipo

**Sugestão:**
- Considerar integração via API do sistema de pedidos
- Ou manter redirecionamento, mas melhorar UX do link

### 2. Newsletter

**Situação Atual:**
- Validação de email funcionando
- Apenas simulação de envio (sem backend)

**Sugestão:**
- Integrar com serviço de email marketing (Mailchimp, SendGrid, etc.)
- Ou implementar endpoint backend para armazenar emails

### 3. Overlay de Produtos

**Situação Atual:**
- Estrutura HTML/CSS completa
- JavaScript com função `abrirOverlay()` definida
- **Não está conectado aos itens do cardápio**

**Sugestão:**
- Adicionar event listeners aos cards do cardápio
- Passar dados do produto (imagem, título, descrição, preço) para o overlay
- Implementar funcionalidade de adicionar ao carrinho

### 4. Arquivo CSS com Erro

**Problema:**
- Arquivo `sobre..css` (dois pontos) - possível erro de nomenclatura

**Sugestão:**
- Renomear para `sobre.css` e atualizar referências no HTML

### 5. Link do WhatsApp

**Problema:**
- Link do WhatsApp no footer está vazio (`href=""`)

**Sugestão:**
- Adicionar link completo: `https://wa.me/5551998423675`

### 6. SEO e Meta Tags

**Situação Atual:**
- Meta tags básicas presentes
- Falta otimização para SEO

**Sugestão:**
- Adicionar meta description
- Open Graph tags para redes sociais
- Schema.org markup para restaurante
- Alt text em todas as imagens (já presente)

### 7. Acessibilidade

**Sugestões:**
- Verificar contraste de cores (WCAG)
- Adicionar aria-labels onde necessário
- Melhorar navegação por teclado
- Testar com leitores de tela

### 8. Performance

**Sugestões:**
- Otimizar imagens (WebP, lazy loading)
- Minificar CSS e JavaScript em produção
- Considerar CDN para assets

---

## 📊 Estado Atual do Projeto

### ✅ Funcionalidades Completas

- [x] Navegação entre páginas
- [x] Scroll suave entre seções
- [x] Design responsivo
- [x] Exibição do cardápio
- [x] Expansão de itens ("Ver mais")
- [x] Cálculo de carrinho (protótipo)
- [x] Validação de formulário de newsletter
- [x] Integração com Google Maps
- [x] Links para redes sociais

### ⚠️ Funcionalidades Parciais

- [ ] Overlay de produtos (estrutura pronta, não conectada)
- [ ] Newsletter (validação OK, sem backend)
- [ ] Carrinho (funcional, mas apenas protótipo)

### ❌ Funcionalidades Não Implementadas

- [ ] Integração com sistema de pedidos real
- [ ] Backend para newsletter
- [ ] Persistência de dados (localStorage/sessionStorage)
- [ ] Sistema de busca no cardápio
- [ ] Filtros por categoria
- [ ] Página de detalhes do produto

---

## 🎯 Conclusão

O projeto **Tomodachi** está em um estado **funcional para apresentação**, com design moderno e responsivo. O site cumpre seu objetivo principal de apresentar informações sobre o restaurante e direcionar clientes para o sistema de pedidos online.

### Pontos Fortes

- ✅ Design limpo e profissional
- ✅ Responsividade bem implementada
- ✅ Código organizado e estruturado
- ✅ Navegação intuitiva
- ✅ Cardápio completo e organizado

### Áreas de Melhoria

- 🔧 Integração do overlay de produtos
- 🔧 Backend para newsletter
- 🔧 Correção de pequenos bugs (link WhatsApp, nome do arquivo CSS)
- 🔧 Otimizações de SEO e performance

---

## 👥 Autores

Projeto desenvolvido por:
- **Arthur Bürkle Schneider**
- **Guilherme Räder Krug**
- **Pedro Vitor Vedovatto**

---

## 📝 Notas Finais

Este documento foi gerado através de análise automatizada do código-fonte do projeto. Para atualizações ou correções, consulte os desenvolvedores do projeto.

**Última atualização**: Janeiro 2025

