# retrieve_stash_from_mass

1. generate STASH file from suite using Rose Macro
2. run `python stash_to_json.py "generated-file-from-step-1 > my_stash.json`
3. manually create a JSON record of the STASH requests you wish to retrieve
4. run `python generate_mass_requests -s "suite-id" -c my_stash.json -r "created-file-from-step-3" > moose_script.sh`
5. run `nohup sh moose_script.sh`
6. do any required processing on the retrieved files
