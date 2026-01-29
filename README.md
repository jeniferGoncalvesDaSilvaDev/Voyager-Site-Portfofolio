# 🚀 Voyager - Compartilhamento de Projetos

![Voyager](https://img.shields.io/badge/Status-Ativo-brightgreen)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## 📖 Sobre o Projeto

**Voyager** é um site de compartilhamento de links inspirado nas sondas espaciais Voyager 1 e 2, lançadas em 1977. Assim como as Voyagers carregam o "Golden Record" com a mensagem da humanidade através do cosmos, este site carrega projetos de **Ciência de Dados, IA e Jogos** através do mundo digital.

### 🌌 Inspiração

As sondas Voyager foram lançadas com a missão de explorar os planetas exteriores do Sistema Solar e além. Elas carregam o Golden Record - um disco de ouro contendo sons, imagens e mensagens representando a diversidade da vida na Terra. Este projeto homenageia essa jornada de exploração e compartilhamento de conhecimento.

## ✨ Funcionalidades

- 🎮 **Seção de Jogos** - Compartilhe links dos seus jogos desenvolvidos
- 🤖 **Seção de Ciência de Dados e IA** - Divulgue seus projetos de Data Science e Inteligência Artificial
- 💾 **Sincronização em Tempo Real** - Os links são compartilhados instantaneamente entre todos os usuários via Firebase
- 🔄 **Modo Offline** - Fallback automático para localStorage se o Firebase não estiver disponível
- 🌟 **Design Espacial** - Interface temática com animações de estrelas
- 📱 **100% Responsivo** - Funciona perfeitamente em qualquer dispositivo (mobile, tablet, desktop, telas grandes)
- ⚡ **Atualização Instantânea** - Mudanças aparecem em tempo real para todos os usuários
- 🟢 **Indicador de Status** - Mostra se está sincronizado ou em modo local

## 🚀 Como Usar

### Adicionando Links

1. **Para Jogos:**
   - Digite o título do jogo no primeiro campo
   - Cole a URL do jogo no segundo campo
   - Clique em "Adicionar Jogo" ou pressione Enter

2. **Para Projetos de IA/Data Science:**
   - Digite o título do projeto no primeiro campo
   - Cole a URL do projeto no segundo campo
   - Clique em "Adicionar Projeto" ou pressione Enter

### Removendo Links

- Clique no botão "Remover" ao lado do link que deseja excluir
- Confirme a remoção na caixa de diálogo

### Acessando Links

- Todos os visitantes podem ver os links compartilhados
- Clique em qualquer URL para abrir em uma nova aba

## 🛠️ Tecnologias Utilizadas

- **HTML5** - Estrutura do site
- **CSS3** - Estilização e animações
- **JavaScript (ES6 Modules)** - Lógica e gerenciamento de dados
- **Firebase Realtime Database** - Sincronização de dados em tempo real
- **localStorage** - Fallback para modo offline

## 📂 Estrutura do Projeto

```
voyager/
│
├── voyager.html          # Arquivo principal (HTML + CSS + JS inline)
└── README.md            # Este arquivo
```

## 💡 Características Técnicas

### Firebase Realtime Database

O site utiliza Firebase para sincronização em tempo real:

```javascript
// Configuração do Firebase já incluída
const firebaseConfig = {
  apiKey: "AIzaSyAt0ALeTBYhcPjzz25uayglbZW42JKJ36k",
  authDomain: "voyager-7531d.firebaseapp.com",
  databaseURL: "https://voyager-7531d-default-rtdb.firebaseio.com",
  projectId: "voyager-7531d",
  storageBucket: "voyager-7531d.firebasestorage.app",
  messagingSenderId: "160118192214",
  appId: "1:160118192214:web:8c1a965d3415ea9791e3f7",
  measurementId: "G-MDP402N7CG"
};
```

### Sincronização em Tempo Real

- Todos os usuários veem os mesmos links instantaneamente
- Mudanças são propagadas automaticamente
- Sem necessidade de refresh da página

### Fallback para localStorage

Se o Firebase não estiver disponível, o site automaticamente usa localStorage como backup.

### Validação de URLs

Todas as URLs são validadas para garantir que começam com `http://` ou `https://`

### Design Responsivo

O layout se adapta automaticamente usando:
- CSS Grid e Flexbox
- Função `clamp()` para tamanhos fluidos
- Media queries para diferentes breakpoints
- Suporte para orientação paisagem em mobile

## 🎨 Paleta de Cores

- **Azul Principal**: `#4a90e2` - Reminiscente do espaço profundo
- **Azul Claro**: `#8ab4f8` - Destaque e interatividade
- **Fundo Escuro**: `#0a0e27` - Espaço sideral
- **Texto**: `#e0e0e0` - Leitura confortável

## 🌟 Animações

- Estrelas piscando no fundo (100 estrelas animadas)
- Transições suaves ao passar o mouse
- Efeitos de hover nos botões e cards

## 📋 Requisitos

- Navegador moderno com suporte a:
  - ES6+ JavaScript (Modules)
  - CSS Grid/Flexbox
  - Firebase SDK (carregado via CDN)
  - localStorage (para fallback)
  - Async/Await
- Conexão com internet (para sincronização em tempo real via Firebase)
  - Funciona offline usando localStorage como backup

## 🚀 Deployment

O site é um arquivo HTML único com Firebase já configurado e pode ser hospedado em:

- **GitHub Pages**
- **Netlify**
- **Vercel**
- **Firebase Hosting** (recomendado, já que o Firebase está configurado)
- Qualquer servidor web estático

### Deploy rápido no Firebase Hosting:

```bash
# Instalar Firebase CLI
npm install -g firebase-tools

# Login no Firebase
firebase login

# Inicializar projeto
firebase init hosting

# Deploy
firebase deploy
```

Basta fazer upload do arquivo `voyager.html` e acessar!

## 🤝 Contribuindo

Este é um projeto pessoal para compartilhamento de links de jogos e projetos de Ciência de Dados/IA.

## 📝 Notas de Uso

- **Sincronização Global em Tempo Real**: Todos os links adicionados são sincronizados instantaneamente via Firebase Realtime Database e visíveis para todos os usuários
- **Persistência**: Os links permanecem salvos no Firebase permanentemente
- **Status de Conexão**: 
  - 🟢 **Sincronizado** - Conectado ao Firebase, dados compartilhados
  - 🔴 **Modo Local** - Usando localStorage, dados apenas no seu navegador
- **Segurança**: As regras do Firebase estão configuradas para permitir leitura/escrita pública. Para ambientes de produção, considere adicionar autenticação
- **Compartilhamento**: Qualquer pessoa com acesso ao site pode adicionar e remover links

## 🎯 Casos de Uso

- Portfolio pessoal de projetos
- Compartilhamento de jogos desenvolvidos
- Divulgação de análises de dados
- Apresentação de modelos de IA/ML
- Coleção de projetos colaborativos
- Hub centralizado de links de projetos

## 📱 Breakpoints Responsivos

O site é totalmente responsivo e se adapta a qualquer tela:

- **Smartphones** (320px - 480px)
  - Layout em coluna única
  - Botões em largura total
  - Fontes otimizadas para leitura
  
- **Tablets** (481px - 768px)
  - Grid adaptativo
  - Espaçamentos otimizados
  
- **Desktop** (769px - 1399px)
  - Layout de duas colunas para formulários
  - Maior espaçamento
  
- **Telas Grandes** (1400px+)
  - Maior largura de container
  - Aproveitamento total do espaço
  
- **Modo Paisagem Mobile**
  - Layout compacto otimizado
  - Menor padding para maximizar espaço

## 📞 Contato

Para reportar problemas ou sugestões, utilize os links compartilhados no próprio site!

## ⚙️ Configuração do Firebase

O projeto já vem com Firebase configurado e pronto para uso. O banco de dados está em:
- **URL**: https://voyager-7531d-default-rtdb.firebaseio.com
- **Projeto**: voyager-7531d

### Regras de Segurança Atuais

```json
{
  "rules": {
    "voyager": {
      ".read": true,
      ".write": true
    }
  }
}
```

**Nota**: Para ambientes de produção, considere implementar autenticação para maior segurança.

---

**Voyager** - Explorando os limites do conhecimento e da criatividade 🌌

*Inspirado nas sondas Voyager 1 e 2 - Levando conhecimento através do cosmos digital desde 2026*
