# StaffFlow — Documento de Requisitos

## 1. Perfis de acesso

### 1.1 RH (Recursos Humanos)
Responsável pela administração geral do sistema, gerenciamento dos cadastros, acompanhamento, aprovação e publicação das escalas mensais.

### 1.2 Líder de setor
Responsável pela elaboração e edição das escalas dos funcionários de seu respectivo setor, encaminhando-as ao RH para aprovação.

### 1.3 Funcionário
Responsável por consultar sua escala mensal, horários de trabalho, turnos e folgas.


## 2. Requisitos funcionais

### 2.1 Gerenciamento de usuários
- O sistema deverá permitir que o RH cadastre funcionários.
- O sistema deverá permitir organizar funcionários por setores e cargos.
- O sistema deverá permitir vincular líderes aos seus respectivos setores.
- O sistema deverá permitir que os usuários acessem o sistema por meio de autenticação.

### 2.2 Gerenciamento de escalas
- O sistema deverá permitir que os líderes criem escalas mensais para seus setores.
- O sistema deverá permitir a definição de horários, turnos e folgas.
- O sistema deverá permitir que os líderes editem escalas antes do envio para aprovação.
- O sistema deverá permitir que o RH consulte as escalas elaboradas pelos líderes.

### 2.3 Aprovação e publicação
- O sistema deverá permitir que o RH aprove ou rejeite escalas.
- O sistema deverá permitir que somente o RH publique as escalas mensais.
- O sistema deverá disponibilizar as escalas publicadas para consulta dos funcionários.

### 2.4 Consulta de escalas
- O sistema deverá permitir que os funcionários consultem suas escalas mensais.
- O sistema deverá apresentar os dias de trabalho, horários e folgas.


## 3. Regras de negócio

### 3.1 Controle de acesso
- Cada usuário deverá acessar somente as funcionalidades permitidas ao seu perfil.
- O RH será responsável por cadastrar e vincular líderes aos setores.
- O líder poderá gerenciar somente as escalas do setor sob sua responsabilidade.
- O funcionário poderá consultar somente suas próprias escalas.

### 3.2 Elaboração das escalas
- As escalas deverão ser organizadas mensalmente.
- Cada funcionário deverá possuir uma programação de trabalho e folgas.
- O sistema deverá identificar conflitos de horários.
- O sistema deverá sinalizar situações em que a quantidade de funcionários escalados seja insuficiente para atender à necessidade do setor.

### 3.3 Aprovação e publicação
- Toda escala elaborada pelo líder deverá ser encaminhada ao RH para aprovação.
- Somente o RH poderá aprovar, rejeitar e publicar as escalas.
- Uma escala rejeitada deverá retornar ao líder responsável para ajustes.
- Os funcionários somente poderão consultar a versão publicada da escala.

### 3.4 Distribuição de turnos e folgas
- O sistema deverá buscar uma distribuição equilibrada de turnos e folgas entre os funcionários.
- A elaboração das escalas deverá considerar as necessidades de cada setor.
- O sistema deverá sinalizar possíveis violações das regras de jornada de trabalho configuradas pela empresa.


## 4. Requisitos não funcionais

### 4.1 Segurança
- O sistema deverá exigir autenticação para acessar funcionalidades restritas.
- As senhas deverão ser armazenadas de forma segura, utilizando hash.
- O sistema deverá controlar as permissões conforme o perfil de cada usuário.
- As operações de aprovação e publicação deverão ser restritas ao RH.

### 4.2 Desempenho
- O sistema deverá apresentar as escalas sem demora excessiva.
- O sistema deverá permitir o gerenciamento de equipes com aproximadamente 50 a 200 funcionários.

### 4.3 Usabilidade
- O sistema deverá possuir uma interface intuitiva e organizada.
- As funcionalidades deverão ser apresentadas conforme o perfil de acesso.
- As escalas deverão ser apresentadas de maneira clara, facilitando a visualização de turnos e folgas.

### 4.4 Manutenibilidade
- O sistema deverá possuir código organizado e modularizado.
- O backend e o frontend deverão ser desenvolvidos separadamente.
- O projeto deverá possuir documentação técnica atualizada.

### 4.5 Compatibilidade
- O sistema deverá funcionar nos principais navegadores modernos.
- A interface deverá adaptar-se a computadores, tablets e smartphones.