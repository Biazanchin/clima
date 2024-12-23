# Previsão do Clima ☁

Este é um projeto de previsão do clima que exibe as condições climáticas atuais e uma previsão para as próximas horas para uma cidade especificada pelo usuário. O projeto utiliza a API OpenWeatherMap para buscar os dados meteorológicos e foi desenvolvido utilizando React.

## Funcionalidades 🚀

- Exibe as condições climáticas atuais com base na localização geográfica do usuário.
- Permite buscar pelo clima de uma cidade especificada.
- Apresenta uma previsão do clima para as próximas horas.

## Tecnologias Utilizadas 🛠

- **React**: Biblioteca para construção da interface.
- **Axios**: Para fazer requisições HTTP.
- **Styled-Components**: Para estilização dos componentes.
- **API OpenWeatherMap**: Fonte dos dados meteorológicos.

## Instalação e Configuração ⚙

1. Clone este repositório:

   ```bash
   git clone https://github.com/Biazanchin/clima.git
   ```

2. Navegue para o diretório do projeto:

   ```
   cd clima
   ```

3. Instale as dependências:

   ```bash
   npm install
   ```

4. Obtenha uma chave de API no [OpenWeatherMap](https://openweathermap.org/).

5. Crie um arquivo `.env` na raiz do projeto e adicione sua chave de API:

   ```env
   VITE_API_KEY=SUA_CHAVE_DE_API_AQUI
   ```

6. Inicie o servidor de desenvolvimento:

   ```bash
   npm run dev
   ```

7. Acesse o aplicativo em seu navegador no endereço [http://localhost:5173](http://localhost:5173).

## Componentes Principais 📂

### App

- Componente principal que gerencia o estado global (cidade, clima atual e previsão).
- Utiliza `navigator.geolocation` para determinar a localização inicial do usuário.
- Renderiza os componentes Busca, ClimaAtual e Previsao.

### Busca

- Componente responsável por permitir ao usuário digitar o nome de uma cidade e buscar informações climáticas.

### ClimaAtual

- Exibe as condições climáticas atuais, incluindo:
  - Nome da cidade
  - Temperatura
  - Descrição
  - Ícone representando o clima

### Previsao

- Mostra uma lista com a previsão do clima para as próximas horas, incluindo:
  - Temperatura
  - Descrição
  - Ícone representando o clima

## Estilização 🎨

O projeto utiliza Styled-Components para criar componentes estilizados e manter a modularidade do código CSS. Exemplos de arquivos de estilo incluem:

- `AppStyles.js`: Estilos gerais para o container principal e o título.
- `BuscaStyles.js`: Estilos para o campo de entrada e o botão de busca.
- `ClimaAtualStyles.js`: Estilos para a apresentação do clima atual.
- `PrevisaoStyles.js`: Estilos para o container da previsão.

## Como Funciona 📖

1. **Localização Automática**: Na primeira execução, o aplicativo solicita permissão para acessar a localização do usuário. Com base nas coordenadas geográficas obtidas, o aplicativo faz uma requisição à API OpenWeatherMap para buscar o clima atual.

2. **Busca Manual**: O usuário pode inserir o nome de uma cidade no campo de busca e clicar no botão para atualizar as informações exibidas.

3. **Previsão**: Uma lista das condições climáticas para as próximas horas é apresentada ao usuário.

## Visualização 👀

![image](https://github.com/user-attachments/assets/913d3711-642b-4b18-a564-87831ee79a75)

