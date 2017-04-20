## testing a target

>>> import python_jsonschema_objects as po
>>> builder = po.ObjectBuilder("./src/bioentity/target.json")
>>> # generate classes from json schema
>>> ns = builder.build_classes()
>>> Target = ns.OpentargetsTarget
>>>
>>> t = Target(id="http://identifiers.org/ensembl/ENSG00000213724",
...            activity="http://identifiers.org/cttv.activity/predicted_damaging",
...            target_type="http://identifiers.org/cttv.target/gene_variant")
