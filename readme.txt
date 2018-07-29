The zip file contains two datasets, i.e., football and restaurant, each in a folder.

For all the files, each line corresponds to one record. 
Line separator "\n", column separator "\t". 
Column headers are not in the files.

----------------
The Restaurant dataset
----------------
1, Reference records in "reference_record.csv". 
Column headers: entity_id, full_name, phone.

2, Ground truth for correct attribute values in "truth.csv".
Column headers: entity_id, full_name, address, phone, website.

3, The other files contain the records collected from different sources.
One data source per file, and the file name gives the name of the data source.
Column headers: name, address, phone, website, entity_id, entity_full_name. (The column "entity_full_name" should NOT be used in the matching process.)

----------------
The Football dataset
----------------
1, Reference records in "reference_record.csv". 
Column headers: entity_id, full_name, birth_data.

2, Ground truth for correct attribute values in "truth.csv".
Column headers: entity_id, full_name, birth_data, height, weight, position, birth_place.

3, Folders "ambi_*" and "err_*" give records with different ambiguities ("%ambi" in the paper) or error rates ("%err" in the paper). For example, "ambi_4/" contains records corresponding to %ambi=0.4.
For each folder, we have one data source per file, and the file name gives the name of the data source.
Column headers: name, birth_data, height, weight, position, birth_place, entity_id, entity_full_name. (The column "entity_full_name" should NOT be used in the matching process.)

----------------
Notes
----------------
1, The csv files may contain missing value.
2, Some reference records do not match with any input record, and the corresponding entities are not contained in the ground truth. 
