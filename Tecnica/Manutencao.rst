***************
Manutenção
***************

Esta secção pretende documentar o processo da gestão de manutenção, identificando 
também os respetivos procedimentos de criação e atualização de dados em SAP. 

Procedimentos
=====================================

Pretende-se nesta secção identificar procedimentos gerais, consoante o departamento, para uma gestão mais eficiente. 

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

.. Attention:: É fundamental que a criação do local esteja correto, seguindo as instruções indicadas nos seguintes tópicos. 

.. image:: img/estruuta_PM.png

.. csv-table::
   :file: EstruturaPM.csv
   :header-rows: 1 
   :class: longtable
   :widths: 1 1 1

Criar Local de Instalação
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Para criar um novo local deverá aceder à transação ``IL01``, devendo preencher os seguintes campos, conforme demonstrado infra: 
 
.. image:: img/local_instalacao.PNG

.. Note:: A categoria do local deverá ser sempre ``4`` .
.. Attention:: O código de estrutura deverá respeitar os níveis indicados na tabela anterior.

