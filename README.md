# plant-disease-ontology
Repository for the Plant Disease Ontology

Note that this ontology is being replaced by the Ontology of PLant Stress

Please use the files in this repository with caution- the PDO is very much in the testing and preliminary stage right now. 

We are currently adding the diseases and pathogens sourced from the American Phytopathological Society (http://www.apsnet.org/publications/commonnames/Pages/default.aspx), primarily focusing on the rice and maize at this time.

We are not "creating a taxonomy", but we are resolving some very complex naming issues, using the APS, NCBI and the EOL. All the pathogens we are adding are referencing their taxon ids in NCBI If they have one).

Once we have a number in, we will import the taxonomy slice that we have created (see https://github.com/Planteome/planteome-ncbi-taxonomy).

A note about the definitions: Currently we are defining the diseases based on the causal agent(s) and the host plant affected using the relations (still in progress).

```
id: RO:0002608
name: has causal agent
def: "Inverse of 'causal agent in'" []
is_a: RO:0002410 ! causally related to
inverse_of: RO:0002500 ! causal agent in
```

and

```
id: RO:0002500
name: causal agent in
def: "A relationship between a material entity and a process where the material entity has some causal role that influences the process" []
is_a: RO:0002595 ! causal relation between material entity and a process
```
