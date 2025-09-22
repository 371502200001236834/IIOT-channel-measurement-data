In this study, part of the data and code used in the paper has been made open-source. The specific content and usage instructions are as follows:
I.Description of Open-Source Data
The open-source data in this study includes the Channel Impulse Response (CIR) data measured under sparse and dense scenarios, as well as some key channel data. The CIR data serves as the core foundation for calculating channel statistical characteristics and plays a crucial supporting role in subsequent channel characteristic analysis.
(1)Data Naming Rules
Data files follow a unified naming format. Taking the example of "cir_m_test_35G1G_1_1", the meaning of each field is as follows:
A.Prefix "cir": Represents the data type of Channel Impulse Response (CIR);
B.Field "m": Indicates that the data collection scenario is a dense scenario (the corresponding field for sparse scenarios is "x", for details, please refer to the instruction document in the folder);
C.Field "35G1G": Represents a measurement frequency band of 3.5 GHz and a bandwidth of 1 GHz, respectively (the format is "frequency band + bandwidth", with both units in GHz);
D.Suffix "1_1": Serves as the identifier for data collection batches, used to distinguish different measurement samples under the same scenario, same frequency band/bandwidth.
In the open-source data folder, the CIR data for the following frequency bands can be obtained directly:
Dense scenarios: 3.5 GHz (1 GHz bandwidth), 4.9 GHz (1 GHz bandwidth), 6 GHz (1 GHz bandwidth). The corresponding files are "cir_m_test_35G1G_1_1", "cir_m_test_49G1G_1_1", and "cir_m_test_60G1G_1_1" respectively;
Sparse scenarios: The data follows the same naming format as that for dense scenarios, except that the scenario identifier "m" is replaced with "x". Specific files can be found in the corresponding subfolder.
(2)Key Channel Characteristic Data
In addition to the Channel Impulse Response (CIR) data, this study also makes open-source the derived data of key channel characteristics under partial scenarios. The naming rule is consistent with that of the CIR data, and the meanings of the core fields are supplemented as follows:

A.Prefix "DS": Represents Delay Spread data;
B.Prefix "K": Represents K-factor data;
C.Prefix "PL": Represents Path Loss data.
Example: "DS_m_test_49G1G_1_1" indicates the Delay Spread data under a dense scenario, with a measurement frequency band of 4.9 GHz and a bandwidth of 1 GHz.

II. Description of Open-Source Code
To facilitate researchers in calculating the Power Delay Profile (PDP) based on Channel Impulse Response (CIR) data, a dedicated calculation code has been made open-source in this study. The specific information is as follows:

Code file name: "PDP_process" (supports MATLAB 2022a and above);
Code function: Takes Channel Impulse Response (CIR) data as input, automatically calculates and outputs the corresponding Power Delay Profile (PDP);
Usage notes: Detailed comments are included in the code, explaining the input parameter format, calculation steps, and the meaning of output results. Researchers can directly call the code or adjust it according to their needs.
III. Other Notes
If you encounter any issues during data reading, code execution, or characteristic calculation, please contact us via the research group email provided in the paper. We will provide timely technical support.
