# Exercise instructions

## Goal

You should write a python script to convert the VCF file into a variation file to be used as input for simulations.


## Details

This folder containes two files:

- a VCF file, which should be used as your input
- a variation file, which is provided to demonstrate the expected output your script should produce

The output file should be formatted according to the instructions provided by the author at paragraph 4.2.1 of their [manual](https://github.com/qasimyu/simuscop/blob/master/docs/SimuSCoP_User_Guide.pdf).


## Suggestions

First of all, you should notice that SNVs, insertions and deletions are formatted in a different way (different number of columns even): this means your script should check what type of variant is present in your VCF file.

The variation file is simulating the very same variants for 2 samples, named "control" and "disease": you're free to call these samples as you prefer, but keep printing 2 samples in the output file.

The genotype of the variant is not necessarily the same between the 2 samples: you should choose it randomly, assuming there is a higher probability to be heterozygous than homozygous.


## Expected run

The script should be run more or less like:

```
python myscript.py --input source.vcf --output variations.txt
```
