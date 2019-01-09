***************
Projetos (PEP)
***************

.. contents:: Tabela de Conteúdos

Esta secção pretende documentar a estrutura, bem como os processos utilizados em SAP, no âmbito da criação e gestão de projetos (PEP).


Estrutura PEP
=======================

Na criação de projetos existem estruturas diferentes consoante o tipo de projeto, seja uma Obra, Contrato ou Vendas. Nas próximas tabelas são apresentadas as diferentes estruturas implmentadas. 

Contratos 
-----------

Estrutura utilizada na criação de projetos do tipo Contrato:

+------------+-------------------------+----------+-----------------------------+
| Nível      | Máscara                 | Caract.  | Denominação                 |
+============+=========================+==========+=============================+
| 1º Nível   | S                       | 1        | Segma                       |
+------------+-------------------------+----------+-----------------------------+
| 2º Nível   | S.EDAXXXXXX             | 9        | Nome Cliente                |
+------------+-------------------------+----------+-----------------------------+
| 3º Nível   | S.EDAXXXXXX.CT          | 2        | Tipo Objeto (CT)            |
+------------+-------------------------+----------+-----------------------------+
| 4º Nível   | S.EDAXXXXXX.CT.0001     | 4        | Nº do Contrato (Sequêncial) |
+------------+-------------------------+----------+-----------------------------+

Obras
-----------

Estrutura utilizada na criação de projetos do tipo Obra:

+------------+-------------------------+----------+--------------------------------+
| Nível      | Máscara                 | Caract.  | Denominação                    |
+============+=========================+==========+================================+
| 1º Nível   | S                       | 1        | SEGMA                          |
+------------+-------------------------+----------+--------------------------------+
| 2º Nível   | S.EDAXXXXXX             | 9        | Nome Cliente                   |
+------------+-------------------------+----------+--------------------------------+
| 3º Nível   | S.EDAXXXXXX.OB          | 2        | Tipo Objeto (OB)               |
+------------+-------------------------+----------+--------------------------------+
| 4º Nível   | S.EDAXXXXXX.OB.0001     | 4        | Nº da Obra (Sequêncial)        |
+------------+-------------------------+----------+--------------------------------+
| 5º Nível   | S.EDAXXXXXX.OB.0001.01  | 2        | Nº da sub-projeto (Sequêncial) |
+------------+-------------------------+----------+--------------------------------+

.. note::

	Na criação de um projeto de ``Intervenções Pontuais`` é fundamental seguir a seguinte lógica: 
		- AVAC: ``Interv. Pontuais AVAC 2018``, consoante o ano corrente; 
		- Eletricidade: ``Interv. Pontuais Eletricidade 2018``, consoante o ano corrente; 
	
Vendas
-----------

Estrutura utilizada na criação de projetos do tipo Venda:

+------------+-------------------------+----------+--------------------------------+
| Nível      | Máscara                 | Caract.  | Denominação                    |
+============+=========================+==========+================================+
| 1º Nível   | S                       | 1        | SEGMA                          |
+------------+-------------------------+----------+--------------------------------+
| 2º Nível   | S.EDAXXXXXX             | 9        | Nome Cliente                   |
+------------+-------------------------+----------+--------------------------------+
| 3º Nível   | S.EDAXXXXXX.VD          | 2        | Tipo Objeto (OB)               |
+------------+-------------------------+----------+--------------------------------+
| 4º Nível   | S.EDAXXXXXX.VD.0001     | 4        | Nº da Venda (Sequêncial)       |
+------------+-------------------------+----------+--------------------------------+
| 5º Nível   | S.EDAXXXXXX.VD.0001.01  | 2        | Nº da sub-projeto (Sequêncial) |
+------------+-------------------------+----------+--------------------------------+

.. note::

	Na criação de um projeto de ``Vendas`` é fundamental seguir a seguinte lógica: 
		- O 4º nível deverá sempre, sem exceção, ser associado ao ano corrente;
	
Criar PEP
=======================

Just a place holder...


Liberar PEP
=======================

Just a place holder...

Encerrar PEP
=======================

Just a place holder...

Transções FUT
=======================

Just a place holder...