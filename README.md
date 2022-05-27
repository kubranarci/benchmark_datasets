# Benchmark Datasets
Benchmark and test datasets

HGSVC freeze3 dataset is downloaded from here:
http://ftp.1000genomes.ebi.ac.uk/vol1/ftp/data_collections/HGSVC2/release/v1.0/integrated_callset/freeze3.sv.alt.vcf.gz

chr21 is extracted by:
bcftools view freeze3.sv.alt.vcf.gz --regions chr21 > freeze3.chr21.sv.alt.vcf.gz

HG00512 subsampled using:
bcftools view -s HG00512 -Oz freeze3.chr21.sv.alt.vcf.gz > HG00512_freeze3.chr21.sv.alt.vcf.gz
