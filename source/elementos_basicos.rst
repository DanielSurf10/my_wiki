Elementos Básicos do reStructuredText
=====================================

Use sinais de igual ou hífen para criar títulos
O uso de sinais de igual cria um título de primeiro nível
O uso de hífens cria um título de segundo nível

Para criar títulos, use sinais de igual, hífens ou outros caracteres repetidos abaixo do texto:

Título
------

Parágrafos são separados por uma linha em branco.

Listas
------

Listas não ordenadas podem ser criadas usando hífens, asteriscos ou sinais de mais:

- Item 1
- Item 2
- Item 3

Listas ordenadas usam números seguidos por um ponto:

1. Primeiro item
2. Segundo item
3. Terceiro item

Blocos de Código
----------------

Para incluir blocos de código, use a diretiva `.. code-block::` seguida pelo nome da linguagem:

.. code-block:: python

   def exemplo():
       print("Olá, mundo!")

Tabelas
-------

Para criar tabelas simples, use o formato de grade:

+------------+------------+
| Cabeçalho  | Cabeçalho  |
+============+============+
| Linha 1    | Linha 1    |
+------------+------------+
| Linha 2    | Linha 2    |
+------------+------------+

Para criar tabelas CSV, use a diretiva `.. csv-table::`:

.. csv-table:: Título da Tabela
    :header: "Cabeçalho 1", "Cabeçalho 2"

    "Linha 1", "Linha 1"
    "Linha 2", "Linha 2"

Links
-----

Para criar links, use a sintaxe de hiperlink:

`Read the Docs <https://readthedocs.org>`_

Marcadores Inline
-----------------

Para ênfase (itálico), use um asterisco: *texto*.

Para ênfase forte (negrito), use dois asteriscos: **texto**.

Para amostras de código, use crases: ``texto``.

Blocos de Citação
-----------------

Blocos de citação são criados com indentação adicional:

   Este é um bloco de citação.

Blocos Literais
---------------

Blocos de código literal são introduzidos com `::` no final de um parágrafo:

Este é um parágrafo normal. O próximo parágrafo é um bloco de código::

   def exemplo():
       print("Olá, mundo!")

Imagens
-------

Para incluir imagens, use a diretiva `.. image::`:

.. image:: image.svg
    :alt: Texto alternativo
    :width: 200

Notas de Rodapé
---------------

Para criar notas de rodapé, use `[1]_` no texto e defina a nota no final do documento:

Texto com nota de rodapé [1]_.

.. [1] Texto da nota de rodapé.

Citações
--------

Para criar citações, use `[Ref]_` no texto e defina a citação no final do documento:

Texto com citação [Ref]_.

.. [Ref] Referência do livro ou artigo.

Substituições
-------------

Para criar substituições, use `|nome|` no texto e defina a substituição:

.. |nome| replace:: texto substituído

Texto com substituição: |nome|.

Comentários
-----------

Para adicionar comentários, use `..` seguido de um espaço:

.. Este é um comentário.

`.. Este é um comentário.`

Metadados HTML
--------------

Para adicionar metadados HTML, use a diretiva `.. meta::`:

.. meta::
   :description: Descrição da página
   :keywords: palavras-chave, separadas, por, vírgulas
