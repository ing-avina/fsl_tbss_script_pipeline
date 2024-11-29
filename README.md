
## FSL TBSS (implementation script) - README

### Introduction
This tool is tailored for non-coders, requiring only two inputs: the path to the input data and the path where the results should be generated. The script will handle the rest, automating the entire process seamlessly. Additionally, the pipeline allows for customizable parameters, enabling users to adapt the workflow to their specific needs.

The provided scripts incorporate a structured proposal for file naming and organization, ensuring clarity and reproducibility. Users can opt to utilize this system as is or modify it according to their preferences and requirements. This flexibility ensures that the pipeline can accommodate a wide range of research setups and workflows.

With simplicity and efficiency at its core, the TBSS Pipeline is an accessible solution for researchers and clinicians alike, whether they are experienced programmers or entirely new to scripting. 

### Project Overview
The TBSS Pipeline project offers a comprehensive solution for processing and analyzing DWI data. By implementing FSL's TBSS tool, researchers can perform voxel-wise statistical analyses to explore the microstructural properties of white matter tracts in the brain. This pipeline provides a standardized workflow that encompasses preprocessing, registration, and statistical analysis, enabling users to derive valuable insights from their DWI data.

### Key Features and Benefits
- **Efficiency:** The pipeline can be use in local computer or in a high-performance computing (HPC) architectures.
- **Reproducibility:** All scripts and processing steps are transparently documented, ensuring that the results can be reproduced and verified by other researchers.
- **User-Friendly:** The pipeline includes code comments minimizing the need for technical expertise and facilitating usability for a wide range of researchers.
- **Quality Control:** Rigorous quality control measures have been integrated into the pipeline to ensure the reliability and accuracy of the processed data.
- **Open Source:** The TBSS Pipeline project is open-source and hosted on GitHub, enabling collaboration, contribution, and customization by the scientific community.

### Getting Started
To start using the TBSS Pipeline, follow these steps:

1. Clone or download the repository to your local machine.
2. Ensure that you have FSL installed and properly configured.
3. Prepare your DWI data in DICOM format and organize it in a suitable directory structure.
4. Customize the pipeline scripts to specify the paths to your data and desired output directories.
5. Run the pipeline using the provided command-line interfaces or adapt the scripts for your specific needs.

### Workflow:

1. Execute 'data_organization.sh' to organize and convert your data.
2. Execute 'preproc_TBSS.sh' to preprocess your DWI data. 
4. Excecute 'outliersQC_counter.sh' to create the PDF report of image quality control. (https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/eddyqc/UsersGuide)
5. Execute 'run_TBSS.sh' to process the data using TBSS.
6. Use glm_gui to create your design for further analysis.
7. Execute 'run_randomise.sh' to perform statistical analysis.
8. Use 'run_cluster_report.sh' to generate a report on your randomise results.
9. Visualize the results using fsleyes.

Note: Make sure to adjust the necessary parameters and paths within the scripts according to your specific data and requirements.

### Support
If you encounter any issues or have questions regarding the script TBSS Pipeline, please reach me at arielvinag@gmail.com.

### Contributors and Maintainers
The TBSS script Pipeline project welcome contributions from the scientific community to further enhance the functionality and usability of the pipeline. 

Thank you for choosing the TBSS Pipeline for your DWI data analysis needs. I hope this pipeline proves to be a valuable tool in your research endeavors :)
