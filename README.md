# covid19_study
Keep notes from personal study on the SARS-CoV-2 virus 

## Table of Contents
  1. [PacBio](#pacbio)
  2. [Variables](#variables)
  3. [Functions](#functions)
  4. [Objects and Data Structures](#objects-and-data-structures)
  5. [Classes](#classes)
     1. [S: Single Responsibility Principle (SRP)](#single-responsibility-principle-srp)
     2. [O: Open/Closed Principle (OCP)](#openclosed-principle-ocp)
     3. [L: Liskov Substitution Principle (LSP)](#liskov-substitution-principle-lsp)
     4. [I: Interface Segregation Principle (ISP)](#interface-segregation-principle-isp)
     5. [D: Dependency Inversion Principle (DIP)](#dependency-inversion-principle-dip)
  6. [Don't repeat yourself (DRY)](#dont-repeat-yourself-dry)

## PacBio  

**Background**:  
* SARS-CoV-2 RNA is 5' CAPed and 3' polyadelynated, like an eukaryotic RNA. However, its length (~29 Kb) does not allow it to be fully sequenced via Iso-seq method
* PacBio recommends targeting 5Kb regions (theoretically until 10 Kb fragments would be possible) for genome sequencing, mainly due to reverse transcription (RT) and PCR limitations - not due to PacBio sequencing. Then the genome sequencing would follow an overlapping tiled strategy, generating overlapping amplicons.  
* There are already many PCR primers available for whole genome sequencing  

**General methodological recommendation**:  
* Using RT enzymes that tollerates high temperatures is advisable since running RT at high temperatures (e.g. 55 degrees Celcius) may help to get through RNA secondary structures
