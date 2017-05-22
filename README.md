

# 1. Getting right the versions.

### desitarget
`git checkout tags/0.9.0`

### fiberassign 
`git checkout tags/0.5.0`

### desimodel
`git checkout tags/0.6.0`

### desisim
`git checkout tags/0.18.2`

### desisurvey
`git checkout tags/0.3.1`

### surveysim
`git checkout tags/0.3.1`

# 2. Generating the list of tiles to be observed

```bash
python scripts/generate_tile_list.py
mv obslist_all.fits input/
rm *.fits
```

# 3. Generate the targets
```bash
python ~/desitarget/bin/select_mock_targets -c input/mock_inputs.yaml --output_dir input/
```