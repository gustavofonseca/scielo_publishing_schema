Ahead Of Print
==============

Todos os arquivos Ahead Of Print (AOP) devem apresentar o valor "research-article" em ``@article-type`` e em ``//subj-group[@subj-group-type="heading"]/subject`` considerar "Articles". 
Esse tipo de documento não apresenta volume, número e paginação, portanto considerar "00" para esses elementos. Como segue o exemplo abaixo:

.. code-block:: xml
	
	<article>
	 ...
	 	<article-meta>
			</pub-date>
				<volume>00</volume>
				<issue>00</issue>
				<fpage>000</fpage>
				<lpage>000</lpage>
		</article-meta>
	 ...
	</article>

Para arquivos Ahead Of Print, a data de publicação deve ser apenas "epub" e com os todos os elementos preenchidos: :ref:`elemento-day`, :ref:`elemento-month` e :ref:`elemento-year`.

.. code-block:: xml

	<article>
	 	...
	 	<article-meta>
			</author-notes>
				<pub-date pub-type="epub">
					<day>13</day>
					<month>03</month>
					<year>2015</year>
				</pub-date>
		</article-meta>
		...
	</article>


.. note::
	Em AOP considerar sempre a tag :ref:`elemento-month` para indicação de mês. Nunca inserir :ref:`elemento-season`.

