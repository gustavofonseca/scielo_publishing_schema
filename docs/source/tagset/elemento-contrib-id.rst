.. _elemento-contrib-id:

<contrib-id>
============

Este elemento possui :ref:`scielo-brasil`.

Atributos obrigatórios:

  1. ``@contrib-id-type``

+-------------------------+--------------------+
| Aparece em              | Ocorre             |
+=========================+====================+
| :ref:`elemento-contrib` | Zero ou mais vezes |
+-------------------------+--------------------+


Determina um identificador digital a um pesquisador.

O atributo ``@contrib-id-type`` possui os seguintes valores:

+------------+-------------------------------------------------------+
|  Valor     | Descrição                                             |
+============+=======================================================+
| lattes     | Identifica um pesquisador no *Currículo Lattes*.      |
+------------+-------------------------------------------------------+
| orcid      | Identifica um pesquisador na *ORCID Organization*.    |
+------------+-------------------------------------------------------+
| researchid | Identifica um pesquisador na *Thomson Reuters*.       |
+------------+-------------------------------------------------------+
| scopus     | Identifica um pesquisador no sistema da *Scopus*.     |
+------------+-------------------------------------------------------+


Exemplo:

.. code-block:: xml

    ...
    <contrib-group>
        <contrib contrib-type="author">
            <contrib-id contrib-id-type="orcid">0000-0001-8528-2091</contrib-id>
            <contrib-id contrib-id-type="scopus">24771926600</contrib-id>
            <name>
                <surname>Einstein</surname>
                <given-names>Albert</given-names>
            </name>
            ...
        </contrib>
        <contrib contrib-type="author">
            <contrib-id contrib-id-type="lattes">4760273612238540</contrib-id>
            <name>
                <surname>Meneghini</surname>
                <given-names>Rogerio</given-names>
            </name>
            ...
        </contrib>
        ...
    </contrib-group>
    ...


.. note:: ``<contrib-id>`` não pode conter dados do tipo URI (URL), **não sendo aceitos** os exemplos:

          * ``<contrib-id contrib-id-type="lattes">http://lattes.cnpq.br/4760273612238540</contrib-id>``
          * ``<contrib-id contrib-id-type="orcid">http://orcid.org/0000-0001-8528-2091</contrib-id>``



.. {"reviewed_on": "20160803", "by": "gandhalf_thewhite@hotmail.com"}
