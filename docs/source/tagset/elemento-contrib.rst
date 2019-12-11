.. _elemento-contrib:

<contrib>
=========

Atributos obrigatórios:

  1. ``@contrib-type``

+-------------------------------+-------------------+
| Aparece em                    | Ocorre            |
+===============================+===================+
| :ref:`elemento-contrib-group` | Uma ou mais vezes |
+-------------------------------+-------------------+



Identifica dados individuais, institucionais ou de grupo, de contribuintes do 
artigo, podendo ser inclusive anônimos. :ref:`elemento-name`, :ref:`elemento-collab`, 
:ref:`elemento-on-behalf-of`, :ref:`elemento-xref`, :ref:`elemento-role` e 
``<anonymous>`` podem ser encontrados neste elemento.

O atributo ``@contrib-type`` define o tipo de contribuição e pode ter os valores:

+------------+----------------------------------------------------------------+
| Valor      | Descrição                                                      |
+============+================================================================+
| author     | Autor do conteúdo.                                             |
+------------+----------------------------------------------------------------+
| compiler   | Compilador - Indivíduo que compilou o conteúdo a partir de     |
|            | várias fontes.                                                 |
+------------+----------------------------------------------------------------+


Exemplo:

.. code-block:: xml

    ...
    <contrib-group>
        <contrib contrib-type="author">
            <name>
                <surname>Freitas</surname>
                <given-names>Ismael Forte</given-names>
                <suffix>Júnior</suffix>
            </name>
            <xref ref-type="aff" rid="aff01">1</xref>
            <role content-type="https://dictionary.casrai.org/Contributor_Roles/Investigation">Pesquisador</role>
        </contrib>
        ...
    </contrib-group>
    ...


.. note::
  * Utilizar *AACR2* - *Código de Catalogação Anglo Americano*, *Registro de ORCID* 
    e/ou *Currículo Lattes* dos autores e avaliar formas de entrada autorizadas 
    para nomes.
  * Outros tipos de contribuidores como tradutor, ilustrador, assistente de 
    pesquisa, editor etc, devem ser identificados em :ref:`elemento-author-notes`, 
    com :ref:`elemento-fn` e ``@fn-type ="other"``, para editor do artigo ou 
    fascículo usar ``@fn-type ="edited-by"``.
  * Recomenda-se o uso da taxonomia CRediT para representar a função ou papel de
    cada contribuinte individual. Saiba mais detalhes em :ref:`taxonomia-credit`.

