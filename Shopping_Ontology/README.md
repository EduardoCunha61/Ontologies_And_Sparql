This directory contains a created ontology (OWL file) with the following requirements:
- There are 3 different classes: "Cliente", "Loja" and "Product";
- Cliente and Loja have the following properties: nome (string) and email (string) (more properties can be added if are considered to be relevant to this domain);
- Produto has a unique code that identifies it;
- Loja must have a property "vende" that relates with Produto and Produto must have a property "éVendidoPor" that relates it with Loja;
- Client must have a property "compra" that relates it with Produto and Produto must have a property "éCompradoPor" that relates it with Cliente;
- Instances of Loja that sell more than 100 different Produtos are part of a new class: "LojaGrande";
- An instance of Produto can not be an instance of Cliente;
- Instances of Loja and Cliente are part of another class named "CompraVenda";
- Add some different instances for each class.

The file Queries_Shopping_Ontology.txt contains some SPARQL queries about the present ontology.
