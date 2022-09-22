# Sampling Methods

# Experimental Set-up

A plant growth experiment was conducted under greenhouse conditions to profile the root-associated bacterial community structure of four wheat varieties.
Field soil was collected from the plough layer (0–25 cm) at the Long-Term Nutrient Depletion Trial at the experimental farm of University of Copenhagen,
Denmark (55° 40′ N, 12° 17′ E). After collecting, the soil was air-dried, and sieved to obtain a fraction ≤4 mm. The soil contained 164 g kg−1 clay, 173 g kg−1 silt, 
333 g kg−1 fine sand, 312 g kg−1 coarse sand, and 17 g kg−1 of soil organic matter, classifying as a sandy loam soil. The field had been fertilized with N:P:K at a rate 
of 120:20:120 kg  ha−1y−1 since 1996. A detailed history of the soil and management practices can be found in van der Bom et al. (2018). PVC pots measuring 24 cm in height 
and 7 cm in diameter were prepared for planting by adding 0.67 L field soil pre-mixed with 0.33 L sand. Soils were fertilized prior to sowing by adding to each pot a liquid 
solution containing (per kg of soil mixture): 142.86 mg N, 39.51 mg Mg, 63.11 mg K. Seeds of winter wheat (Triticum aestivum) cultivars Heerup, Sheriff, Kvium and Rembrandt, 
supplied by Sejet Plant Breeding (Denmark), were sown in soil-filled pots with 105 individuals per variety (1 plant per pot). Plants were germinated for 18 days under 
controlled greenhouse conditions with photoperiods of 8 H/19 °C days, 16 H/15 °C nights, humidity 60% day/ 65% night and light 300 µE prior. Plants were subsequently vernalized
for 106 days with growth chamber settings of 8 h/6 °C days and 16 h/5 °C nights, and 300 µE light. Following 106 days of vernalization, the wheat growth experiment was carried 
out under controlled greenhouse conditions with photoperiods of 8 H/19 °C days, 16 H/15 °C nights, humidity 60% day/ 65% night and 500 µE light. Fertilizer (142.86 mg N per kg 
of soil mixture) was added to each pot and plants were regularly irrigated with deionized water. The different wheat cultivars were subsequently sampled at the flag leaf 
emergence stage at 141 days (Kvium), 142 days (Sheriff), 145 days (Rembrandt), or 146 days (Heerup) after sowing. 


# Sampling of rhizosphere, rhizoplane and bulk soil bacterial communities

On the day of sampling, plant height was measured from the base of the plant to the tip of the longest leaf for all plants within a variety. Based on this measure, the five 
highest plants as well as the five lowest plants were selected for sampling. Each plant was uprooted entirely with its surrounding soil, and excess soil removed manually from 
the roots by gentle shaking, leaving a thin layer of soil which remained attached to the roots. To extract root-associated microbiomes, the root including attached soil was 
separated into four equally sized sub-samples at the longitudinal axis to represent the full length of the root. Subsequently, a sequential transfer was used to separate 
rhizosphere and rhizoplane communities. First, a subsample was transferred to a falcon tube containing 25 ml sterile water, and subsequently shaken. Roots were removed, and the 
soil remaining in the tube, was defined as rhizosphere. The removed roots were transferred to a new falcon tube with 25 ml sterile water, shaken and subsequently subjected to 
sonication for 2 minutes using a sonication bath. Following sonication, the roots were removed. This sample was defined as the rhizoplane sample. For the bulk soil, approximately
1 g of sample was collected. All samples (rhizosphere, rhizoplane and bulk soil) were flash frozen in liquid nitrogen and subsequently freeze-dried. All freeze dried samples
were transferred to sterile 20 ml scintillation vials with two zirconium oxide beads per vial, and samples were ground using a pain shaker for 2 x 4.5 mins. A total of 200 mg
material was then weighed into sterile eppindorf tubes for DNA/RNA co-extraction.

# DNA extraction and PCR amplification

DNA/RNA was co-extracted using the NucleoBond RNA Soil Mini Kit (REF 740142.50 and REF 740143.50 – Macherey-Nagel) and concentration was measured on a Qubit 4.0 
(Thermo-Fischer Scientific) using the High-Sensitivity DNA Assay.

# 16S rRNA gene amplicon sequencing

Amplicon libraries for Illumina sequencing were prepared on a 2-step PCR using the 341F and 806R primer pair targeting the V3-V4 hypervariable region of the 16S rDNA 
gene using the PCR ULTRA Polymerase Mix (PCRBIOSYSTEMS - PB10.32) following the manufacturer's instructions. The only modification is the addition of 0,5 ul of BSA (10mg/ml)
in the first PCR reaction. Our pipeline is similar to the end described in the Earth Microbiome Project (https://earthmicrobiome.org/protocols-and-standards/16s/).

1st PCR profile:
_____________________
95oC	  2 minites

33 cycles of:
95oC	  15 seconds
55oC	  15 seconds
72oC	  40 seconds

72oC	  4 minutes
4oC	    ∞
_____________________

2nd PCR profile
_____________________
98oC	  2 minites

13 cycles of:
98oC	  10 seconds
55oC	  20 seconds
72oC	  40 seconds

72oC	  5 minutes
4oC	    ∞
_____________________

At each step, the samples were run on a 1% Agarose Gel to verify successful amplification and evaluate the presence of primer-dimers. The samples were pooled equimolarly 
and the pool was run on a Tapestation 4150 (Agilent Technologies) using the D1000 tape and reagents. The pool was run on an Illumina MiSeq using the 500 cycles v2 chemistry.

Bioinformatics analysis
The raw sequencing data were analyzed in QIIME2 using the default pipeline as described here: https://shorturl.at/mtDNV. Briefly,
Visualization of QIIME2 artifacts was done in QIIME2view (https://view.qiime2.org/).
