# Healthcare Data Warehouse ETL

A Pentaho Data Integration (PDI) project for building a healthcare data warehouse using dimension and fact table transformations.

## Overview

This project demonstrates an ETL pipeline that extracts healthcare-related data, transforms it into dimensional structures, and loads it into a data warehouse.

The pipeline follows a star schema approach consisting of:

- Dimension tables for reference data
- Fact tables for patient visit and healthcare transaction data
- Job orchestration for running dimension and fact processes

## Project Structure

```text
.
├── dim/
│   ├── d_Agama.ktr
│   ├── d_Alamat.ktr
│   ├── d_JenisKelamin.ktr
│   ├── d_Pendidikan.ktr
│   └── ...
├── fact/
│   ├── d_Entitas.ktr
│   ├── f_PatientVisite.ktr
│   ├── f_PatientVisiteIn.ktr
│   ├── f_PatientVisiteMD.ktr
│   ├── f_PatientVisiteMR.ktr
│   └── f_PatientVisiteOut.ktr
├── init/
│   └── init.ktr
├── dimension_job.kjb
├── fact_job.kjb
└── eis_pipeline.kjb
