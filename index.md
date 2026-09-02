# Política de Privacidade — Achados da Geru

**Última atualização:** 2 de setembro de 2026

Esta Política de Privacidade descreve como a extensão para navegador **"Achados da Geru"** ("a Extensão") trata as informações dos usuários. Ao instalar e utilizar a Extensão, você concorda com os termos descritos abaixo.

## 1. Quem somos

A Extensão é desenvolvida e mantida por **Achados da Geru**, um projeto dedicado à divulgação de ofertas e promoções de produtos vendidos na Amazon Brasil.

Contato: gustavotravnik@outlook.com

## 2. Qual é o propósito da Extensão

A Extensão tem um único propósito: exibir, dentro das páginas de busca do site **amazon.com.br**, um painel com produtos em oferta relacionados ao termo pesquisado pelo usuário, com base em um catálogo de produtos mantido pelo Achados da Geru.

## 3. Quais dados a Extensão coleta

**A Extensão não coleta, armazena, transmite ou compartilha nenhuma informação de identificação pessoal dos usuários.**

Especificamente, a Extensão **não coleta**:
- Nome, e-mail, endereço, idade ou qualquer identificador pessoal;
- Dados de saúde;
- Dados financeiros ou de pagamento;
- Senhas, credenciais ou dados de autenticação;
- Comunicações pessoais (e-mails, mensagens, chats);
- Localização (GPS, IP ou região);
- Histórico de navegação;
- Atividade do usuário (cliques, digitação, rolagem, monitoramento de rede);
- Conteúdo de outros sites.

## 4. Como a Extensão funciona (uso técnico de dados, sem coleta)

Para cumprir seu único propósito, a Extensão realiza localmente as seguintes operações, sem enviar dados pessoais a nenhum servidor:

- **Leitura da URL da aba ativa:** a Extensão verifica, em tempo real e apenas no domínio `amazon.com.br`, se a página atual é uma página de busca e qual termo foi pesquisado (parâmetro `k` da URL, que já é público e visível na barra de endereço do navegador). Essa leitura é feita apenas para comparar o termo com o catálogo de ofertas e **não é armazenada, registrada ou transmitida a nenhum servidor**.
- **Armazenamento local (IndexedDB):** a Extensão mantém, exclusivamente no dispositivo do usuário, uma cópia local do catálogo de produtos em oferta (título, imagem, preço, preço promocional, condição de parcelamento e link do produto) e a data da última sincronização. Nenhum dado pessoal do usuário é armazenado nesse banco local — apenas informações públicas dos produtos do catálogo.
- **Comunicação de rede:** a Extensão realiza requisições `fetch` para a API pública `api.divulgadorinteligente.com`, exclusivamente para baixar o catálogo de produtos em oferta (dados públicos, sem qualquer informação do usuário anexada à requisição). Nenhum dado de navegação, identificador de usuário ou termo de busca é enviado a essa API.
- **Injeção de conteúdo visual:** a Extensão insere um painel HTML/CSS ("Achados da Geru") na página de resultados de busca da Amazon, exibindo produtos do catálogo local que correspondem ao termo pesquisado. Essa injeção ocorre inteiramente no navegador do usuário.

## 5. Compartilhamento de dados com terceiros

A Extensão **não vende, aluga, transfere ou compartilha** qualquer dado do usuário com terceiros. A única comunicação de rede realizada é a busca do catálogo público de ofertas, que não contém nem transmite dados do usuário.

## 6. Uso de dados para fins não relacionados

A Extensão **não usa nem transfere dados do usuário para fins não relacionados** ao seu único propósito (exibição de ofertas relacionadas à busca), e **não utiliza dados para determinar crédito ou para fins de empréstimo**.

## 7. Permissões solicitadas e por que são necessárias

| Permissão | Finalidade |
|---|---|
| `storage` | Armazenar localmente (IndexedDB) o catálogo de ofertas e a data da última sincronização. |
| `tabs` | Detectar se a aba ativa está no domínio `amazon.com.br`, para habilitar ou desabilitar o ícone da Extensão. |
| `alarms` | Agendar verificações periódicas de atualização do catálogo em segundo plano. |
| `host_permissions` (`api.divulgadorinteligente.com`) | Buscar o catálogo de produtos em oferta. |
| `host_permissions` (`www.amazon.com.br`) | Ler o termo de busca da URL e injetar o painel de ofertas na página de resultados. |

## 8. Código remoto

A Extensão **não carrega nem executa código JavaScript ou WebAssembly remoto**. Todo o código-fonte está empacotado dentro da própria Extensão. As únicas requisições de rede realizadas em tempo de execução retornam exclusivamente dados em formato JSON (o catálogo de produtos), nunca código executável.

## 9. Segurança

Como nenhum dado pessoal é coletado ou transmitido, não há risco de exposição de dados pessoais dos usuários por meio da Extensão. As informações armazenadas localmente (catálogo de produtos) ficam restritas ao navegador do próprio usuário e podem ser removidas a qualquer momento desinstalando a Extensão.

## 10. Direitos do usuário

Como a Extensão não coleta dados pessoais, não há dados pessoais para acessar, corrigir ou excluir. Caso o usuário deseje remover todos os dados armazenados localmente pela Extensão (catálogo em cache), basta desinstalá-la pelo navegador — isso apaga automaticamente o banco de dados local (IndexedDB).

## 11. Alterações nesta política

Esta Política de Privacidade pode ser atualizada periodicamente para refletir mudanças na Extensão ou em requisitos legais/da Chrome Web Store. A data da última atualização estará sempre indicada no topo deste documento. Recomendamos revisitar esta página periodicamente.

## 12. Contato

Em caso de dúvidas sobre esta Política de Privacidade ou sobre o funcionamento da Extensão, entre em contato: [e-mail ou canal de contato a definir]

---

*Esta política foi redigida para atender aos requisitos de transparência do Chrome Web Store Developer Program Policies.*
