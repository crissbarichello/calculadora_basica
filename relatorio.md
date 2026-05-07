# Relatório de Falhas

## Relatório de Falha – 01
- **ID da Falha:** BUG-INI-001
- **Título:** [BUG] Calculadora aceita texto e concatena valores na soma
- **Data / Hora:** 06/05/2026 – 19:40
- **Reportado por:** Cristiano Barichello
- **Ambiente:** Navegador Desktop / HTML + JavaScript / Ambiente Local
- **Descrição da Falha:**
  - Os campos da calculadora aceitam texto livre e, ao realizar a soma, ocorre concatenação de strings em vez de cálculo matemático.
- **Comportamento Esperado:**
  - A calculadora deve aceitar apenas números e realizar operações matemáticas corretamente.
- **Comportamento Atual:**
  - Ao informar valores como "2" e "3", o resultado da soma é "23" em vez de 5.
- **Passos para Reproduzir:**
  1. Abrir a página do sistema
  2. Inserir 2 no primeiro campo
  3. Inserir 3 no segundo campo
  4. Clicar no botão Somar
- **Evidências:**
  - Resultado exibido como 23 no campo de resultado.
- **Severidade:** Alta
- **Reprodutibilidade:** Sempre ocorre
- **Encaminhado para:** Equipe de Desenvolvimento Front-end

## Relatório de Falha – 02
- **ID da Falha:** BUG-INI-002
- **Título:** [BUG] Campos numéricos da calculadora utilizam type="text"
- **Data / Hora:** 06/05/2026 – 19:42
- **Reportado por:** Cristiano Barichello
- **Ambiente:** Navegador Desktop / HTML
- **Descrição da Falha:**
  - Os campos da calculadora foram definidos como input type="text", permitindo a digitação de letras e caracteres especiais.
- **Comportamento Esperado:**
  - Os campos deveriam ser do tipo number, impedindo a entrada de caracteres inválidos.
- **Comportamento Atual:**
  - É possível digitar letras, símbolos ou texto livre nos campos da calculadora.
- **Passos para Reproduzir:**
  1. Abrir a página
  2. Digitar abc em qualquer campo
  3. Clicar em qualquer operação matemática
- **Evidências:**
  - O sistema executa operações com valores inválidos.
- **Severidade:** Média
- **Reprodutibilidade:** Sempre ocorre
- **Encaminhado para:** Equipe de Front-end

## Relatório de Falha – 03
- **ID da Falha:** BUG-INI-003
- **Título:** [BUG] Divisão por zero não é tratada
- **Data / Hora:** 06/05/2026 – 19:44
- **Reportado por:** Cristiano Barichello
- **Descrição da Falha:**
  - A aplicação permite divisão por zero sem qualquer tratamento ou mensagem de erro.
- **Comportamento Esperado:**
  - O sistema deveria impedir a divisão por zero e exibir uma mensagem de erro adequada.
- **Comportamento Atual:**
  - Ao dividir qualquer número por zero, o resultado exibido é Infinity.
- **Passos para Reproduzir:**
  1. Inserir 10 no primeiro campo
  2. Inserir 0 no segundo campo
  3. Clicar em Dividir
- **Evidências:**
  - Resultado exibido como Infinity.
- **Severidade:** Alta
- **Reprodutibilidade:** Sempre ocorre
- **Encaminhado para:** Equipe de Desenvolvimento

## Relatório de Falha – 04
- **ID da Falha:** BUG-INI-004
- **Título:** [BUG] Senha exibida e armazenada em texto puro
- **Data / Hora:** 06/05/2026 – 19:46
- **Reportado por:** Cristiano Barichello
- **Descrição da Falha:**
  - O campo de senha está configurado como type="text" e a senha é exibida em alerta e registrada no console.
- **Comportamento Esperado:**
  - O campo de senha deveria ser do tipo password e nunca exibido ou logado.
- **Comportamento Atual:**
  - A senha é visível durante a digitação e registrada no console do navegador.
- **Passos para Reproduzir:**
  1. Acessar o formulário de cadastro
  2. Digitar qualquer valor no campo de senha
  3. Finalizar cadastro
  4. Abrir o console do navegador
- **Evidências:**
  - Senha exibida em alerta e no console.
- **Severidade:** Crítica
- **Reprodutibilidade:** Sempre ocorre
- **Encaminhado para:** Equipe de Segurança / Front-end

## Relatório de Falha – 05
- **ID da Falha:** BUG-INI-005
- **Título:** [BUG] Uso de elemento HTML obsoleto `<marquee>`
- **Data / Hora:** 06/05/2026 – 19:48
- **Reportado por:** Cristiano Barichello
- **Descrição da Falha:**
  - O código utiliza a tag `<marquee>`, que é obsoleta e não recomendada pelos padrões atuais da web.
- **Comportamento Esperado:**
  - O uso de animações deve ser feito via CSS ou JavaScript moderno.
- **Comportamento Atual:**
  - O sistema utiliza uma tag descontinuada, comprometendo a compatibilidade e acessibilidade.
- **Severidade:** Baixa
- **Reprodutibilidade:** Sempre ocorre
- **Encaminhado para:** Equipe de Front-end
