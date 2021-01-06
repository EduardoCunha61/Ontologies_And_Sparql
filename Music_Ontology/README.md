This directory contains a RDF file, exported from Protégé, that describes an ontology that initially was created with the following requisites:

- There are 4 different classes: Obra, Compositor, Instrumento e Evento;
- Obra must have the following properties: id, titulo, tipo, duração (int value that represents the number of minutes), temCompositor (relates Obra with Compositor) and temPartituraInstrumento (relates Obra with each Instrument that have musical scores);
- Compositor has the following properties: id, nome, data de nascimento, escreveuObra (relates Compositor with Obra);
- Instrumento has the following properties: id, nome, participaemObra (relates Instrumento with Obra);
- Evento has the following properties: id, nome, local, data and temObra (relates Evento with each Obra that is being played in that event);
- Obra has an attribute "tipo" which possible values are: "Marcha de desfile", "Marcha de procissão", "Marcha de concerto", "Ligeiro" and "Rapsódia";
- According to the value of attribute "tipo", define the following subclasses of Obra : "Marcha", "Ligeiro" and "Rapsódia";
- "Marcha" has the following subclasses: "MarchaDesfile", "MarchaProcissão" and "MarchaConcerto".

After exporting the OWL file in Protégé, it was implemented some SPARQL queries for a brief analysis of the ontology.
The file Queries_Musical_Ontology.txt contains some of those queries as well as the intended purpose of each one of them.
