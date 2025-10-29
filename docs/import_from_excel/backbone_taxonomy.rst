Backbone Taxonomy
=================

1. The Excel Files
------------------

You have to create one Excel file:

1. Excel file containing the Backbone taxonomy, named exactly like you have named your Backbone Taxonomy component on localcosmos.org

Naming the Excel file
^^^^^^^^^^^^^^^^^^^^^

The import will only succeed if you name your Excel files correctly. The name of the Excel file containing the Backbone taxonomy **must match** the name of your Backbone Taxonomy component on localcosmos.org.

+-----------------------------------------------+-----------------------------+
| Name of Backbone Taxonomy on localcosmos.org  | Name of Excel file          |
+===============================================+=============================+
| Backbonetaxonomy                              | ``Backbonetaxonomy.xlsx``   |
+-----------------------------------------------+-----------------------------+

**Important:** Ensure that the file name is spelled exactly as it appears on localcosmos.org, including spaces and capitalization.

2. Backbone Taxonomy Excel
--------------------------
The Backbone Taxonomy Excel enables you to upload relationships between Taxa, like Predation or similarity of species.
Before you continue to read, it is recommended to download the example Excel file. :download:`download example Excel file </_static/Backbone Taxonomy/Backbone taxonomy.xlsx>`.

**Important: all content you put into your Excel files has to be in the primary language of your Local Cosmos App**

The Taxon Relationship Types sheet
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The Backbone Taxonomy Excel requires at exactly one sheet named ``Taxon Relationship Types``. This is where you define the types of relationships between taxa.
The sheet has to contain the following columns:

**Example: Sheet "Taxon Relationship Types" of "Backbone taxonomy.xlsx":**

.. raw:: html

   <div style="overflow-x: auto; white-space: nowrap;">

+---+---------------------+-----------------------+-------------------------------+
|   | A                   | B                     | C                             |
+---+---------------------+-----------------------+-------------------------------+
| 1 | Relationship Name   | Taxon Role (optional) | Related Taxon Role (optional) |
+===+=====================+=======================+===============================+
| 2 | Similar species     |                       |                               |
+---+---------------------+-----------------------+-------------------------------+
| 3 | Predation           | Predator              | Prey                          |
+---+---------------------+-----------------------+-------------------------------+

.. raw:: html

   </div>

Rows of the Taxon Relationship Types sheet
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The first row is for definitions. From the second row on, types of taxon relationships are listed.

**Row 1: Definition of a type of relationship**

Mandatory columns are:

* **Relationship name**: the name of the relationship.
* **Taxon Role (optional)**: The name of the role of the first taxon in this relationship.
* **Related Taxon Role (optional)**: The name of the role of the second taxon in this relationship.

These columns have to be present in your spreadsheet.
This means, that the first three cells of row one are fixed cells. You cannot change the content of these cells.


**Row 2 onwards: Types of relationships**

Some Data types require further definition in row 2. The following data types require further definition:

* **text**: the text column requires a title. The title is the text that will be displayed in the app. The title is mandatory.
* **seo**: the SEO column requires further definition in row 2. You have two options: "title" and "meta_description".



The Taxon Relationships sheet
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The Backbone Taxonomy Excel requires at exactly one sheet named ``Taxon Relationships``. This is where you define the specific relationships between taxa.
The sheet has to contain the following columns:

**Example: Sheet "Taxon Relationships" of "Backbone taxonomy.xlsx":**

.. raw:: html

   <div style="overflow-x: auto; white-space: nowrap;">

+---+---------------------+-----------------------+-------------------------------+-------------------------------+-------------------------------+-------------------------------+-------------------------------+-------------------------------+
|   | A                   | B                     | C                             | D                             | E                             | F                             | G                             | H                             |
+---+---------------------+-----------------------+-------------------------------+-------------------------------+-------------------------------+-------------------------------+-------------------------------+-------------------------------+
| 1 |                     | Taxon                 | Taxon                         | Taxon                         | Related Taxon                 | Related Taxon                 | Related Taxon                 |                               |
+---+---------------------+-----------------------+-------------------------------+-------------------------------+-------------------------------+-------------------------------+-------------------------------+-------------------------------+
| 2 | Relationship        | Scientific Name       | Author (optional)             | Taxonomic Source              | Scientific Name               | Author (optional)             | Taxonomic Source              | Description (optional)        |
+===+=====================+=======================+===============================+===============================+===============================+===============================+===============================+===============================+
| 3 | Predation           | Turdus merula         |                               | taxonomy.sources.col          | Lumbricus terrestris          |                               | taxonomy.sources.col          | Blackbird eats worm           |
+---+---------------------+-----------------------+-------------------------------+-------------------------------+-------------------------------+-------------------------------+-------------------------------+-------------------------------+
| 4 | Similar species     | Turdus merula         | Linnaeus, 1758                | taxonomy.sources.col          | Sturnus vulgaris              |                               | taxonomy.sources.col          |                               |
+---+---------------------+-----------------------+-------------------------------+-------------------------------+-------------------------------+-------------------------------+-------------------------------+-------------------------------+

.. raw:: html

   </div>

Rows of the Taxon Relationships sheet
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The first two rows are for definitions. From the third row onwards, specific taxon relationships are listed.
Cee A1 has to be empty.

**Row 1: Defining the columns for Taxon, Related Taxon**

Mandatory columns are:

* **Column A**: Empty in the first row.
* **Taxon**: B1, C1 and D1 have to contain `Taxon`.
* **Related Taxon**: E1, F1 and G1 have to contain `Related Taxon`.
* **Column H**: H1 has to be empty.

These columns have to be present in your spreadsheet.
This means, that the first eight cells of row one are fixed cells. You cannot change the content of these cells.

**Row 2: Defining the Relationship**

Mandatory columns are:

* **Relationship**: Column A points to a relationship defined in the Taxon Relationship Types sheet.
* **Scientific Name**: The scientific name of the first taxon.
* **Author (optional)**: The author of the scientific name of the first taxon.
* **Taxonomic Source**: The taxonomic source of the first taxon.
* **Scientific Name**: The scientific name of the related taxon.
* **Author (optional)**: The author of the scientific name of the related taxon.
* **Taxonomic Source**: The taxonomic source of the related taxon.
* **Description (optional)**: A description of the relationship.

These columns have to be present in your spreadsheet.
This means, that the first eight cells of row two are fixed cells. You cannot change the content of these cells.


**Row 3 onwards: Specific taxon relationships**

From row 3 onwards, you can list specific taxon relationships, following the definitions in rows 1 and 2.