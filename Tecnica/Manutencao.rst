***************
Manutenção
***************

Esta secção pretende documentar o processo da gestão de manutenção, identificando 
também os respetivos procedimentos de criação e atualização de dados em SAP. 

Procedimentos
=====================================

Pretende-se nesta secção identificar procedimentos gerais, consoante o departamento.

AVAC 
-------------------------------------

.. Note:: Sempre que existir a necessidade de recolha de equipamentos, de um Cliente/Instalação, deverá ser utilizada a lista específicada em baixo! 

:download:`Lista Equipamentos.xls <files/Lista_Equipamentos.xlsx>`.


SAP: Manual
=====================================

Este tópico pretende explicar e documentar os procedimentos referente ao módulo de SAP:PM. 

Locais de Instalação
-------------------------------------

Um local de instalação representa uma estrutura organizacional hierárquica dentro da empresa, serve basicamente para estruturar os 
objectos de manutenção de uma empresa de acordo com critérios funcionais, relacionados com os diversos processos de manutenção. 
Um local de instalação representa o lugar em que trabalhos de manutenção são realizados.

Estrutura
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Gráficamente a estrutura implementada em SAP:PM é mostrada na seguinte imagem: 

.. image:: img/estruuta_PM.png

.. Attention:: É fundamental que a criação do local esteja correta, seguindo as instruções indicadas nos seguintes tópicos e com o número de carácteres. 

.. csv-table::
   :file: EstruturaPM.csv
   :header-rows: 1 
   :class: longtable
   :widths: 1 1 1

Criar Local de Instalação
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Para criar um novo local deverá aceder à transação ``IL01``, devendo preencher os seguintes campos, conforme demonstrado infra: 
 
.. image:: img/local_instalacao.PNG

.. Note:: A categoria do local deverá ser sempre ``4``.
.. Attention:: O código de estrutura deverá respeitar os níveis indicados na tabela anterior.

No separador :guilabel:`Localização` deverá ser preenchidos os seguintes campos: 

.. image:: img/local_localizacao.PNG

No separador :guilabel:`Organização` deverá ser preenchidos os seguintes campos: 

.. image:: img/local_organizacao.PNG

No separador :guilabel:`Estrutura` deverá ser preenchidos os seguintes campos: 

.. image:: img/local_estrutura.PNG

.. Attention:: Qualquer local, ou equipamento, deve estar montado. Ou seja, o local de instalação superior deverá esta preenchido. 

Procedimento: Desginações 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Todos os locais de instalação, após o 4º nível deverão ter a seguinte estrutura de desginação: 

Estrutura: ``Especialidade | Denominação do local``

Exemplo: ``UPS | Continente da Horta``


Procedimento: P. Transformação
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

No 

Procedimento: Especialidades 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Equipamentos
-------------------------------------

Um equipamento é um objecto técnico de manutenção, físico e individual cuja manutenção é gerida no sistema SAP. 
Um equipamento representa uma máquina passível de efectuar manutenção de forma independente. 

Os equipamentos poderão ser montados e desmontados nos locais de instalação sempre haja uma alteração da localização do equipamento havendo 
sempre um registo histórico dos dados.

Criar equipamento
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Para criar um novo local deverá aceder à transação ``IE01``, devendo preencher os seguintes campos, conforme demonstrado infra: 

.. image::  img/equipamento.PNG

.. Note:: A categoria do local deverá ser sempre ``4``.

No separador :guilabel:`Geral` deverá ser preenchidos os seguintes campos: 

.. image:: img/equip_geral.PNG

.. Attention:: Deverá selecionar o tipo de objeto correto, é através desta informação que os modelos em NAVIA estão associados (i.e.: S.PT-200 = Manutenção Posto de Transformação).

No separador :guilabel:`Localização` deverá ser preenchidos os seguintes campos: 

.. image:: img/equip_localizacao.PNG

No separador :guilabel:`Organização` deverá ser preenchidos os seguintes campos: 

.. image:: img/equip_organizacao.PNG

No separador :guilabel:`Estrutura` deverá ser preenchidos os seguintes campos: 

.. image:: img/equip_estrutura.PNG

.. Attention:: Qualquer local, ou equipamento, deve estar montado. Ou seja, o local de instalação superior deverá esta preenchido. 

Desativar/Eliminar equipamento 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Para inativar um equipamento deverão ser feitos os seguintes passos, através da transação ``IE02``:
	- 'Equipamento' > 'Funções' > 'Ativo<->Inativo' > 'Desativar'
	- 'Equipamento' > 'Funções' > 'Marcação para eliminação' > 'Definir'
	- Guardar
	
.. image:: img/equip_inativar.PNG

Transações Frequentes
-------------------------------------