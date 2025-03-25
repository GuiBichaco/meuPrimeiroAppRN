# Aula de React Native com TypeScript

## O que é React Native?
O React Native é um framework de desenvolvimento mobile cross-platform criado pelo Facebook (agora Meta) que permite a criação de aplicativos para iOS e Android usando JavaScript e React. Ele possibilita o desenvolvimento de apps nativos sem a necessidade de utilizar Java/Kotlin (Android) ou Swift/Objective-C (iOS).

Diferente de outras soluções híbridas, o React Native não renderiza uma WebView, mas sim componentes nativos reais, garantindo melhor performance e experiência de usuário.

## Cronologia do React Native
- **2012** – O Facebook percebe dificuldades em escalar seu app mobile para iOS e Android. Surge a ideia de criar uma solução baseada em React para mobile.
- **2013** – Um hackathon interno no Facebook leva à primeira versão do React Native.
- **2015** – O Facebook lança oficialmente o React Native como um projeto open-source na conferência React.js Conf.
- **2016** – Empresas como Airbnb, Tesla e Walmart começam a adotar o React Native.
- **2018** – O Facebook anuncia grandes mudanças no core do React Native para melhorar desempenho.
- **2020** – Lançamento da versão 0.62, trazendo suporte oficial ao Flipper (ferramenta de debug).
- **2021** – Nova arquitetura anunciada, trazendo melhorias no desempenho com Fabric e TurboModules.
- **2023** – React Native continua sendo um dos frameworks mais usados para desenvolvimento mobile.

## Por que o React Native se destaca no mercado?
O React Native se tornou uma das principais tecnologias para desenvolvimento mobile devido a diversos fatores:
- **Código único para iOS e Android** → Reduz o tempo e custo de desenvolvimento.
- **Componentes nativos reais** → Melhor desempenho comparado a soluções híbridas como Ionic e Cordova.
- **Hot Reloading e Fast Refresh** → Permite visualizar mudanças no código em tempo real.
- **Grande comunidade e suporte** → Empresas como Instagram, Tesla, Shopify e Uber Eats usam React Native.
- **Integração com bibliotecas modernas** → Suporte a Expo, Firebase, Redux e TypeScript.

## Configuração do Ambiente de Desenvolvimento para React Native com Expo

### 1. Instalação do Node.js e Yarn/NPM
Abra o terminal e execute os seguintes comandos para verificar a instalação:
```sh
node -v  # Verifica a versão do Node.js
npm -v   # Verifica a versão do NPM
```

### 2. Instalação do Expo CLI
O Expo CLI é uma ferramenta que facilita a criação, desenvolvimento e gerenciamento de projetos React Native.
Para instalar globalmente, rode:
```sh
npm install -g expo-cli
```
Verifique a instalação com:
```sh
expo --version
```
Mais informações: [Documentação Expo](https://expo.dev/)

## Criando o Primeiro Projeto React Native com Expo no VS Code

### 1. Criando o Repositório no GitHub
Passos:
1. No GitHub, clique em **New repository**.
2. Defina o nome do repositório como `meuPrimeiroAppRN`.
3. Escolha a opção **Public**.
4. Copie a URL do repositório para uso posterior.

### 2. Clonando o Repositório
No VS Code:
1. Abra o **Source Control** (`Ctrl + Shift + G`).
2. Clique em **Clone Repository**.
3. Cole a URL do repositório.
4. Escolha o diretório para armazenar o projeto.
5. Abra o repositório clonado.

### 3. Inicializando o Projeto com Expo CLI
Com o repositório aberto no VS Code:
```sh
expo init .
```
Selecione:
✅ `blank (TypeScript)`

### 4. Criando a Estrutura do Projeto
Crie a pasta `src/` e dentro dela:
```sh
📂 meuPrimeiroAppRN
├── 📂 src/
│   ├── 📂 components/    # Componentes reutilizáveis
│   ├── 📂 screens/       # Telas do app
│   ├── 📂 styles/        # Estilos globais
│   ├── 📂 services/      # Serviços de API
│   └── 📂 routes/        # Configuração de navegação
├── 📄 App.tsx            # Ponto de entrada do app
├── 📄 package.json       # Dependências do projeto
├── 📄 tsconfig.json      # Configuração do TypeScript
└── 📄 app.json           # Configuração do Expo
```

### 5. Versionando as Alterações no GitHub
No VS Code, **Source Control**:
```sh
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@gmail.com"
git add .
git commit -m "Inicialização do projeto com Expo e TypeScript"
git push origin main
```

### 6. Executando o App
Inicie o Expo:
```sh
npx expo start
```
Isso abrirá o Expo Developer Tools no navegador, permitindo rodar o app no emulador ou dispositivo.

### 7. Rodando o App no Navegador
Se necessário, instale as dependências web:
```sh
expo install react-native-web@~0.18.10 react-dom@18 @expo/webpack-config@^18.0.1
```
E rode o projeto no navegador:
```sh
expo start --web
```
Agora você pode visualizar seu primeiro app React Native rodando com Expo! 🚀

