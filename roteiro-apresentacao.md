Roteiro de Apresentação — BS One (Versão Executiva)
Público: Gestores e Superintendentes | Tempo estimado: ~8 minutos

Diretriz: Narre a estratégia e o valor de negócio, demonstrando domínio técnico de forma natural.

ABERTURA — Capa e Propósito
45 segundos

"Bom dia/boa tarde a todos. Nós somos o grupo Helix, e hoje viemos apresentar o projeto final do Programa de Capacitação: o BS One.

O BS One é um projeto que nasce com um propósito muito claro: levar a inteligência e a conveniência do agendamento digital — que hoje a Bradesco Saúde já consolida nos hospitais da rede Novamed — para dentro do aplicativo do beneficiário, abraçando também as clínicas parceiras e os médicos autônomos.

Ao longo dos próximos minutos, vou mostrar como transformamos essa oportunidade em uma solução de software robusta, escalável e de alto valor para o nosso ecossistema."

BLOCO 1 — O Cenário Atual e a Oportunidade
2 minutos

"Para compreendermos o valor do BS One, precisamos olhar para como a jornada de agendamento funciona hoje na nossa rede credenciada externa.

Atualmente, o Bradesco Saúde oferece uma experiência excelente de agendamento digital para os hospitais integrados à rede Novamed. No entanto, quando o beneficiário precisa de uma consulta com um médico autônomo ou em uma clínica parceira, essa experiência é completamente diferente.

Esse cenário se divide em três grandes dores:

Para o Cliente: Ele precisa abrir o aplicativo, localizar o médico no livro de prestadores, sair do ambiente Bradesco e fazer um contato analógico — seja por telefone ou WhatsApp — para tentar conciliar um horário. É uma jornada fragmentada.

Para Médicos Autônomos e Clínicas: Há total imprevisibilidade. A ocupação das suas agendas depende exclusivamente de o paciente tomar a iniciativa ativa de ligar e marcar.

Para o Bradesco: Nós perdemos a rastreabilidade da jornada do cliente justamente no momento crucial da marcação da consulta."

BLOCO 2 — A Solução: API BS One
2 minutos

"A resposta a esse cenário é o BS One: um novo módulo back-end que estende a capacidade de agendamento nativa do ecossistema Bradesco Saúde.

Em vez de criar uma nova plataforma isolada, o BS One funciona como o motor por trás do aplicativo que o cliente já usa. Ele permite que clínicas credenciadas e médicos autônomos disponibilizem suas grades de horários diretamente na nossa base.

A arquitetura do sistema foi desenhada em três camadas essenciais:

Camada de Consumo: Onde o aplicativo móvel do cliente consome os serviços de agendamento.

Módulo de Negócio (Java e Spring Boot): Onde processamos as regras de elegibilidade, cruzamento de horários e regras de plano.

Camada de Integração: Onde os consultórios parceiros conseguem disponibilizar e sincronizar suas agendas com o ecossistema Bradesco."

BLOCO 3 — Valor Agregado e Regras de Negócio
2 minutos

"O grande diferencial do BS One não é apenas digitalizar um processo, mas sim o impacto estratégico que ele gera para cada ator envolvido:

Para o Cliente: Ele passa a ter a 'experiência padrão Novamed' em toda a rede externa. Ele localiza o médico especialista e agenda a consulta em poucos cliques, sem sair do app. Além disso, o sistema conta com um motor de notificação preventiva: se o beneficiário está no período de realizar um check-up anual ou um retorno, o app sugere proativamente os horários disponíveis desses médicos parceiros.

Para os Médicos e Clínicas: Garante previsibilidade, otimização da ocupação do consultório e redução de absenteísmo através de confirmações automáticas disparadas pelo sistema.

Para a Bradesco Saúde: Retemos o cliente na nossa plataforma do início ao fim da jornada. Isso nos gera dados valiosos sobre o comportamento de utilização da rede externa e, a longo prazo, reduz a sinistralidade ao estimular a medicina preventiva.

Tudo isso opera sob regras de negócio rígidas: validação automatizada de cobertura e carência antes de fechar o agendamento, e total conformidade com a LGPD no tratamento de dados de saúde."

BLOCO 4 — Processo de Desenvolvimento (MVP)
1 minuto e 15 segundos

"Como projeto do Programa de Capacitação, o desenvolvimento do BS One foi conduzido ao longo de quatro semanas utilizando a metodologia ágil para a entrega de um MVP (Mínimo Produto Viável):

Histórias de Usuário: Mapeamos estritamente o fluxo essencial: a busca e reserva de horários pelo beneficiário, e a disponibilização da grade de atendimento pelo médico.

Tecnologia: A solução foi construída utilizando a linguagem Java com o framework Spring Boot, resultando em uma API REST robusta. Como se trata de uma Prova de Conceito, os dados de clínicas e médicos foram simulados em um banco de dados em memória (H2), e todos os endpoints foram documentados de forma transparente via Swagger, permitindo testes práticos e imediatos da solução.

O foco total foi garantir que a arquitetura proposta é viável e que as regras de negócio de agendamento funcionam perfeitamente."

ENCERRAMENTO
45 segundos

"Para concluir, o BS One unifica a jornada de saúde do nosso cliente. Nós pegamos um modelo de sucesso interno e o expandimos para valorizar os médicos autônomos e clínicas parceiras que movem a nossa rede externa. Passamos de uma operadora que apenas indica um telefone para uma operadora que efetivamente conecta o paciente ao cuidado médico.

Muito obrigado a todos pela atenção. Estou à disposição para as perguntas dos senhores."

 
 Q&A: Perguntas Prováveis (Ajustadas para Gestores)
1. "Como os médicos autônomos vão colocar a agenda deles nesse sistema?"

"Para este MVP, a API do BS One foi estruturada para receber essas grades de horários. Em uma fase futura de implantação, o caminho ideal seria disponibilizar um portal simplificado para o médico gerenciar seus horários ou integrar a API do BS One diretamente com os principais softwares de prontuário eletrônico de mercado que as clínicas já utilizam."

2. "Se o agendamento é automático ou sugerido, como fica o controle do usuário?"

"O sistema trabalha com o conceito de sugestão inteligente. Ele identifica que o paciente precisa realizar uma consulta preventiva (por exemplo, um retorno anual) e exibe as opções de horários dos médicos parceiros na tela. O agendamento só é efetivado após o consentimento e clique confirmatório do usuário no aplicativo."

3. "Por que foi escolhido o Swagger para a documentação técnica?"

"Como o foco do projeto de capacitação foi o desenvolvimento do motor back-end (as regras de negócio e integrações em Java), nós não construímos a interface visual do aplicativo (front-end). O Swagger resolve isso perfeitamente: ele gera uma interface gráfica automática a partir do código, permitindo que qualquer pessoa teste os endpoints de agendamento em tempo real e veja o sistema funcionando."
