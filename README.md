# Leitor CNAB 444

<div align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/CNAB%20444-0a5c0a?style=for-the-badge&logoColor=white" alt="CNAB 444">
</div>

## 📋 Índice

- [Sobre o Projeto](#-sobre-o-projeto)
- [Funcionalidades](#-funcionalidades)
- [Estrutura do Arquivo CNAB 444](#-estrutura-do-arquivo-cnab-444)
- [Instalação e Uso](#-instalação-e-uso)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Contribuição](#-contribuição)
- [Licença](#-licença)
- [Contato](#-contato)

## 📖 Sobre o Projeto

O **Leitor CNAB 444** é uma aplicação web desenvolvida para processar e analisar arquivos no formato CNAB 444, seguindo estritamente as especificações do manual FIDC (Fundo de Investimentos em Direitos Creditórios). 

A ferramenta permite a leitura de arquivos de remessa, extraindo e organizando as informações de forma clara e intuitiva, facilitando a análise de dados financeiros para profissionais que trabalham com fundos de investimentos em direitos creditórios.

O projeto foi desenvolvido com base no layout CNAB 444 - REMESSA (MERCADO), que define a estrutura padrão para troca de informações entre sistemas de Fundos de Investimentos de Direitos Creditórios.

## ✨ Funcionalidades

- ✅ **Upload de Arquivos**: Permite o upload de arquivos CNAB 444 nos formatos .txt ou .rem através de arrastar e soltar ou seleção manual.
- ✅ **Processamento Exato**: Segue estritamente as especificações do manual para processamento dos registros Header, Detalhe, Lastro e Trailler.
- ✅ **Visualização Organizada**: Exibe os dados em abas organizadas por tipo de registro, com cards informativos e tabelas responsivas.
- ✅ **Filtros**: Oferece filtros para busca específica de dados, facilitando a localização de informações relevantes.
- ✅ **Paginação**: Implementa paginação para tabelas com grande volume de dados, melhorando a performance e usabilidade.
- ✅ **Resumo Estatístico**: Apresenta um resumo estatístico dos dados processados, incluindo totais de registros e valores.
- ✅ **Exportação CSV**: Permite exportar os dados processados para formato CSV, facilitando a análise em outras ferramentas.
- ✅ **Design Responsivo**: Interface adaptável a diferentes tamanhos de tela, funcionando bem em desktops, tablets e smartphones.
- ✅ **Feedback Visual**: Indicadores visuais durante o processamento de arquivos e mensagens de erro/sucesso.

## 📊 Estrutura do Arquivo CNAB 444

O arquivo CNAB 444 é composto por quatro tipos de registros, cada um com uma estrutura específica definida no manual:

### Registro Header (Tipo "0")
Contém informações gerais sobre o arquivo, como identificação do originador, banco, data de geração, entre outros.

Principais campos:
- Identificação do Registro (posição 1)
- Identificação do Arquivo Remessa (posição 2)
- Literal Remessa (posições 3-9)
- Código de Serviço (posições 10-11)
- Literal Serviço (posições 12-26)
- Código do Originador (posições 27-46)
- Nome do Originador (posições 47-76)
- Número do Banco (posições 77-79)
- Nome do Banco (posições 80-94)
- Data da Gravação do Arquivo (posições 95-100)
- Identificação do Sistema (posições 109-110)
- Nº Sequencial do Arquivo (posições 111-117)

### Registro Detalhe (Tipo "1")
Contém informações detalhadas sobre os títulos e operações, como dados do sacado, valores, vencimentos, entre outros.

Principais campos:
- Identificação do registro (posição 1)
- Data de Carência (posições 2-7)
- Tipo de Juros (posição 8)
- Taxa de Juros (posições 11-20)
- Coobrigação (posições 21-22)
- Característica especial (posições 23-24)
- Modalidade da operação (posições 25-28)
- Natureza da operação (posições 29-30)
- Nº de controle do participante (posições 38-62)
- Identificação ocorrência (posições 109-110)
- Nº do documento (posições 111-120)
- Data do vencimento do título (posições 121-126)
- Valor do título (posições 127-139)
- Espécie de título (posições 148-149)
- Data da emissão do título (posições 151-156)
- Valor presente da parcela (posições 193-205)
- Nome do sacado (posições 235-274)
- Endereço completo (posições 275-314)
- CEP (posições 327-334)
- Cedente (posições 335-394)

### Registro Lastro (Tipo "3")
Contém informações sobre os lastros que dão suporte às operações, como dados de emissão, vencimento, valores, entre outros.

Principais campos:
- Identificação do registro (posição 1)
- Data de Emissão (posições 2-7)
- Data Vencimento (posições 8-13)
- Valor Nominal (posições 14-26)
- Valor do Total Pedido (posições 27-39)
- Valor da Nota Fiscal (posições 40-50)
- Identificação do Tipo de Recebível/Lastro (posições 51-52)
- Tipo de Lastro Performado (posições 53-54)
- Número do Título/Lastro (posições 55-64)
- Número do Pedido (posições 65-79)
- Nome do sacado (posições 96-135)
- Endereço completo (posições 136-175)
- CEP (posições 176-183)
- Código de Verificação da NFS-e (posições 184-215)
- Número Da Nota Fiscal (posições 238-257)
- Chave De Acesso NFE (posições 258-301)
- Cedente (posições 302-361)

### Registro Trailler (Tipo "9")
Contém informações de fechamento do arquivo, como número sequencial do último registro.

Principais campos:
- Identificação registro (posição 1)
- Número sequencial de registro (posições 439-444)

## 🚀 Instalação e Uso

### Pré-requisitos

- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Arquivo CNAB 444 no formato .txt ou .rem

### Instalação

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/leitor-cnab-444.git
   ```

2. Acesse o diretório do projeto:
   ```bash
   cd leitor-cnab-444
   ```

3. Abra o arquivo `index.html` em seu navegador:
   ```bash
   # Apenas clique duas vezes no arquivo index.html
   # Ou utilize um servidor local como o Live Server do VS Code
   ```

### Como Usar

1. **Upload do Arquivo**:
   - Arraste e solte um arquivo CNAB 444 na área indicada ou
   - Clique em "Selecionar Arquivo" para escolher um arquivo .txt ou .rem

2. **Processamento**:
   - Aguarde enquanto o arquivo é processado
   - Um indicador de carregamento será exibido durante o processamento

3. **Visualização dos Dados**:
   - Após o processamento, os dados serão exibidos em abas organizadas:
     - **Resumo**: Exibe estatísticas gerais do arquivo processado
     - **Header**: Mostra as informações do registro Header
     - **Detalhes**: Exibe os registros do tipo Detalhe em formato de tabela
     - **Lastros**: Exibe os registros do tipo Lastro em formato de tabela
     - **Trailer**: Mostra as informações do registro Trailler

4. **Filtragem e Exportação**:
   - Utilize os filtros para encontrar informações específicas
   - Navegue pelas páginas usando os controles de paginação
   - Clique em "Exportar CSV" para baixar os dados processados

## 🛠 Tecnologias Utilizadas

- **HTML5**: Estrutura semântica e organização do conteúdo
- **CSS3**: Estilização e design responsivo da interface
- **JavaScript**: Processamento dos dados e interatividade da aplicação
- **Material Icons**: Ícones para melhorar a experiência do usuário

## 🤝 Contribuição

Contribuições são bem-vindas! Se você deseja contribuir com o projeto, siga os passos abaixo:

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/nova-funcionalidade`)
3. Faça commit das suas alterações (`git commit -m 'Adicionando nova funcionalidade'`)
4. Faça push para a branch (`git push origin feature/nova-funcionalidade`)
5. Abra um Pull Request

## 📄 Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.

## 📧 Contato

Lucas Moura - pf.lucasmoura@gmail.com

Link do Projeto: [https://github.com/mouraluck/cnab-reader](https://github.com/mouraluck/cnab-reader)
