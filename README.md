# Novo Normal - Reserva de mesas
aplicativo.msapp

Esse aplicativo foi desenvolvido para auxiliar no controle de reservas de mesas no escritório considerando um modelo híbrido em que as equipes terão 1 semana presencial e 3 semanas em home office com mesas compartilhadas e revezamento. 

A ideia é que na semana de cada equipe as posições sejam "fixas", ao mesmo tempo que, se alguém quiser/precisar ir para o escritório fora da data combinada, consiga reservar qualquer mesa livre (dispensa confirmação de reserva, tudo automático mesmo).



🎥 https://www.youtube.com/watch?v=oMHUc5VFeaM

--

👾 estou disponibilizando o zip no git pra quem tiver interesse, além dele, vai também um xls com informações a respeito dos tipos de tabelas/colunas que usei na construção do app, e você fica livre pra usar excel, sharepoint, sql, ou qualquer outro como base!

--

🛠️ elementos do layout

HTML/CSS: botões na tela inicial e bg

ClearCollect: layout (mesas)

Gallery: agendamentos e layout

UpdateContext: pop-ups

Botões: em exibição

--

🔌 conectores: 

UsuáriosdoOffice365 - para identificar o usuário logado no set()

Office365Outlook - para envio de e-mails

--

🎞️ mídia

.png (local): mesas e ícones

.png (sp-on): pessoas, 3x4

.gif (local): modelo de mesa notebook

.glb (github): modelo de mesa 3D desktop/cpu

--

🎲 base de dados

Sharepoint List: tabela NN_Pessoas

Sharepoint List: Tabela NN_Agendamento

Sharepoint Library: imagens das pessoas

ClearCollect: tabela do Layout

(minha base dedos é claramente fictícia com os personagens do arrowverse, mas os nomes/tipos de colunas são padrão, basta incluir os dados das pessoas da empresa)

--

🕹️ Controles

Loockup: proc de informações entre tabelas

Set: identificação do perfil do logado

If: condições para validação de reservas.

Launch: links/web 

--

☠️ uma condição crucial do app está na label invisível: Label_SemanaIndicada_Validacao, ela contem o calendário semanal conforme ISOWEEK desde a última semana de 2021 até a última semana de 2025 + a atribuição de qual equipe estará em qual data. Caso haja a necessidade alterar o modelo, como: ao invés de 3 semanas home office sejam 2 semanas home office e 2 no prédio, é essa label que você deve alterar.
