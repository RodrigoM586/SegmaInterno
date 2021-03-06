***************
Obras/Contratos
***************

.. contents:: Tabela de Conteudos

Esta secção têm como objetivo explicar o formulário de Obras/Contratos da base de dados, bem como informar acerca das suas funcionalidades.

Contratos
===========================

Aquando da adjudicação de Contratos, deverá ser seguido o seguinte Workflow. Cada um dos subcapítulos explica detalhadamente, cada uma das fases necessárias para a abertura completa do Contrato.  

.. image:: img/Diagrama_AberturaContrato.png

Criação do Registo
----------------------------

Após a adjudicação formal e o documento, do contrato, respetivamente assinado e digitalizado, deverá ser criado um ``Registo (RCDEE)`` para inicio do processo de criação do Contato. 

.. image:: img/registo_descricao.PNG 

:strong:`Modelo:` PEP - Designação do Cliente - Descrição do Serviço 

:strong:`Exemplo:` S.SRAGRIFLO.CT.0003 - SECRETARIA REGIONAL DA AGRICULTURA E FLORESTAS - Manutenção Preventiva UPS 10kVA

.. Note::  Deverá ser respeitado o modelo de preechimento do assunto do registo. 

Criação da Distribuição
----------------------------

Após criação do ``Registo`` deverá ser criada uma ``Distribuição`` associado ao registo anteriormente criado, respeitando o seguinte modelo: 

.. image:: img/distribuicao_descricao.PNG 

.. Note:: Preenchimento do descritivo da distribuição (despacho/informação):

		- :strong:`Pasta Fisica`: "Endereço/caminho da pasta"
		- :strong:`Proposta`: "Referência da proposta"
		
		Informação Técnica: 
		
		- :strong:`Tipo de instalações`: "Exploração do Posto de Transformação de.... "
		- :strong:`Periodicidade de execução`: "Semestral..."
		- :strong:`Gestor do Contrato SEGMA`: "Identificar gestor, apoio/adjunto do gestor."
		- :strong:`Gestor do Contrato Cliente`: "Identificar gestor e contactos telf."
		- :strong:`Outros Dados/Observações`: 
		
		Informação Financeira: 
		
		- :strong:`Nota de Encomenda`: 
		- :strong:`Valor Anual do Contrato`: "Exemplo: 2000€/ANO”
		- :strong:`Periodicidade de faturação`: 
		- :strong:`Responsável pelo pedido de Faturação`: 
		- :strong:`Duração`: "De: DD/MM/AAAA A DD/MM/AAAA"
		- :strong:`Renovação automática`: SIM/NÃO
		- :strong:`Alerta renovação`: "Indicar Data" 
				
Divulgação
----------------------------
			
Esta é a lista paralela em que a ``Distribuição`` deverá ser divulgada. 
			
 - Etapa final deverá ser o Chefe Departamento Suporte; 
 - Etapas intermédias, em paralelo:
	 - GESTOR DE CONTRATO E APOIOS;
	 - CHEFE DO DEPARTAMENTO A QUE SE REFERE;
	 - COORDENADOR CONFORME ÁREA A QUE SE REFERE;
	 - CHEFE DEPARTAMENTO SUPORTE;
	 - COORDENADOR DEP. SUPORTE;
	 - APOIO DEP.SUPORTE;
	 - DIRETOR TÉCNICO 

Documentação
----------------------------

Deverá ser anexado os seguintes documento na distribuição criada anteriormente. 

 - Contrato digitalizado;
 - Nota de Encomenda (se existir);
 - Proposta;
 - Outros documentos

Formulário Obra
===========================

O formulário da Obra/Contrato agrega toda a informação que seja imputada a um registo, seja hiperligações para pastas, RCD ou criação de Propostas e/ou Ordens de Serviço. 

.. image:: img/frm_obra.PNG

.. Note:: A partir da versão 7.00 da base de dados técnica, tornou-se possível a criação de um registo de Obra por qualquer utilizador. 

.. Important:: Todo o registo de Obra/Contrato está diretamente associado com um registo em SAP, para alocação de custos e proveitos. 

				A criação do registo em SAP é da responsabilidade do departamento de Suporte. Até criação do registo em SAP, a obra ficará temporariamente identificada como ``Por Classificar``. 

Ordens Serviço
===========================

Através do separador ``Ordens Serv.`` é possível visualizar todas as OS's associadas a este registo.

.. image:: img/frm_obra_OS.PNG

Propostas
===========================

Através do separador ``Propostas`` é possível visualizar todas as Propostas associadas a este registo, sejam através do intermédio de uma Ordem de Serviço ou selecão do registo diretamente na Proposta. 

.. image:: img/frm_obra_proposta.PNG


Relatórios
===========================

Através do separador ``Relatórios`` é possível visualizar todas os relatórios técnicos associados a este registo, que tenham sido realizados na base de dados.

.. image:: img/frm_obra_relatorios.PNG

Encomendas
===========================

Através do separador ``Encomendas`` é possível visualizar todas as encomendas efetuadas para este registo, sejam através de SAP ou Access.

.. image:: img/frm_obra_compras.PNG

.. Note:: Qualquer encomenda que seja efetuada para a Obra, a mesma estará vísivel neste separador, independentemente de ter sido criada em Access ou SAP. 

		Se clicar na coluna ``P. Compra`` poderá consultar todos os itens encomendados de forma discriminada. 

.. Important:: A atualização de todos os registos de SAP para Acccess é realizado de forma manual e tipicamente no fím de cada dia útil.

Manutenção (SAP)
===========================

Neste separador poderá consultar todos os registos existentes em SAP, associados ao Contrato. 

.. image:: img/frm_obra_manut.PNG

.. Important:: Qualquer alteração necessária terá de ser efetuada exclusivamente em SAP. 

Resultados Financeiros
===========================

Esta secção pretende explicar como é consultada toda a informação relativa com custos e proveitos da Obra/Contrato.

Faturas Clientes
-----------------------

Esta secção mostra todas as faturas que foram, ou vão, ser faturadas ao Cliente, bem como notas de crédito. 

.. image:: img/frm_obra_fatCliente.PNG

.. Important:: Se o campo ``Data`` e ``Nº Fatura`` estiverem em branco, significa que a fatura ainda não foi enviada para o Cliente.

Faturas Fornecedores
-----------------------

Esta secção mostra todas as fatura de Fornecedores. Sendo que cada linha corresponde a um item, já faturado, do pedido de compra enviado ao Fornecedor. 

.. image:: img/frm_obra_fatFornec.PNG

.. Note:: Todas as linhas aqui apresentadas significa que o item já foi rececionado.

Movimentos Stock
-----------------------

No separador ``Mov. Stock`` é apresentado todo o movimento de stocks entre o armazém e a obra. 

.. image:: img/frm_obra_stock.PNG

Compromissos
-----------------------

No separador ``Compromissos`` são mostrados todos os itens, de Pedidos de Compra, que foram realizados para a Obra mas ainda não foram rececionados/faturados.

.. image:: img/frm_obra_compromissos.PNG

Mão de Obra
-----------------------

Atravês desta secção é possível visualizar toda a mão de obra imputada à Obra.

.. image:: img/frm_obra_MO.PNG

Notificações
===========================

O separador ``Notificações`` pretende agrupar todas as notas, criadas pelos utilizadores, associadas à Obra. 

Estas notificações têm como principal objetivo reunir a informação para renovação de contrato ou outras informações necessárias.

.. image:: img/frm_obra_notif.PNG

