

# 1. Getting right the versions.

### surveysim
`git checkout tags/0.5.0`

### desitarget
`git checkout tags/0.9.0`

### fiberassign 
`git checkout tags/0.5.0`

### desimodel
`git checkout tags/0.6.0`

### desisim
`git checkout tags/0.18.2`

### desisurvey
`git checkout tags/0.6.0`

# 2. Generating the list of tiles to be observed

```bash
export DESISURVEY="input"
python ~/surveysim/bin/surveysim --start 2019-10-1 --stop 2019-10-31 --save observed_tiles.fits --seed 42
rm input/obsplan*.fits
```