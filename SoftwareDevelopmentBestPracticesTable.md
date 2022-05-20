# Software Development Best Practices for the CIG Community (Summary Table)

|           | Minimum | Standard | Target |
| --------- |:--------|:---------|:-------|
| Licensing | Open source | Same as Minimum | Same as Minimum |
| Version Control | All source in version control. | Differentiation between maintenance and new development. | (a) New features added in separate branches. (b) Stable development branches for rapid release of new features. |
| Coding | | (a) User-friendly specification of parameters at run time. (b) Development plan, updated annually. (c) Comments in code with purpose of each function.  (d) Users can add features or alternative implementations without modifying main branch. (e) User errors generate message that helps user correct the problem. | Standard + (a) Functionality implemented as a library rather than an application. (b) Output of provenance information. (c) Parallel access to inputs/outputs. (d) Checkpointing. |
| Portability, configuration, and building | (a) Codes builds on Unix-like machines with free tools. (b) Portable build system. | Minimum + (a) Dependency checking. (b) Automation and portability of configuration and building. (c) Each simulation outputs all configuration and build options for reproducibility. | Standard + (a) Selection of compilers, optimization, build flags during configuration without modifying files under version control. (b) Multiple builds using same source. (c) Allows installation to a central location. |
| Testing | (a) Code includes tests that verify it runs properly. (b) Results of accuracy and/or performance benchmarks (if established by the community). | Code includes pass/fail tests that verify it runs properly.  (b) Development pipeline uses continuous integration to automate running test suite.| (a) Pass/fail unit testing for verification at a fine grain level. (b) Method of Manufactured Solutions for verification at a coarse grain level. (c) Use of code coverage tools to asses gaps in test coverage.|
| Documentation | (a) Instructions for installation. (b) Description of all parameters. (c) Explanation of physics the code simulates. (d) Cookbook examples with input files. (e) Citable publication. (f) Documentation provided online or offline. | (a) Description of workflow for research use. (b) Description of how to extend code in anticipated ways. | Standard + (a) Guidelines on parameter scales/combinations for which code is designed/tested. (b) FAQs or knowledge base. (c) Documentation provided in dynamic form and available offline. |
| User workflow | | (a) Changing simulation parameters does not require rebuilding. (b) User-specified directories and filenames for input/output. (c) Use of standard binary formats. (d) Citation for code version. | Standard + Reproducibility via archiving of workflow. |

**Minimum**: Practices that codes must follow in order to be accepted by CIG.

**Standard**: Practices in addition to the Minimum that should be used by all codes developed within the CIG community. Codes not meeting these standards should be actively working to eliminate deficiencies.

**Target**: Desirable practices beyond the Standard that developers should consider in defining development priorities for codes developed within the CIG community.
