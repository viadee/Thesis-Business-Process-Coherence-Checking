# Business Process Coherence Checking Dataset

## Description

This repository contains a curated dataset designed for the empirical validation of business process coherence checking using Large Language Models (LLMs). The dataset aims to test the effectiveness and robustness of LLMs in identifying and verifying the coherence across multi-level business process documentation.

## Dataset Structure

The dataset consists of 12 model-text pairs, sourced equally from two major BPM repositories. Each pair includes a BPMN model enriched with textual descriptions, organized as follows:

- **Eid-Sabbagh et al. (2012)**:
  - Client Acquisition
  - Credit
  - Invoice
  - Purchasing
  - Replacement Parts
  - Web Design

- **Friedrich et al. (2011)**:
  - Dispatching
  - Hospital
  - Hotel
  - Part Production
  - Recourse
  - Zoo

Each model-text pair is contained within its own sub-folder.

### Structure of Each Sub-folder

- `model.bpmn`: The BPMN model file.
- `description.txt`: The textual description of the process.
- `changes.json`: JSON schema documenting changes introduced for experimentation.

### Selection Criteria

- Models must compile without errors using the bpmn.io VS Code plugin.
- Must be syntactically correct according to BPMN 2.0 standards.
- Must include swim lanes to capture organizational changes.
- Excludes multi-language artifacts for consistency.

### Business Process Change Classification Framework

**Business Process Change Dimensions**:
- Task Dimension
- Control Flow Dimension
- Data Dimension
- Organization Dimension

**Change Relevance Categories**:
- Relevant Change
- Unrelated Change
- Negligible Change

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes or additions.

## License

This dataset is licensed under the GNU General Public License (GPL).

## References

- Eid-Sabbagh, R.-H., Kunze, M., Meyer, A., & Weske, M. (2012). A Platform for Research on Process Model Collections. In W. van der Aalst, J. Mylopoulos, M. Rosemann, M. J. Shaw, C. Szyperski, J. Mendling, & M. Weidlich (Eds.), *Lecture Notes in Business Information Processing. Business Process Model and Notation* (Vol. 125, pp. 8–22). Springer Berlin Heidelberg. https://doi.org/10.1007/978-3-642-33155-8_2

- Friedrich, F., Mendling, J., & Puhlmann, F. (2011). Process Model Generation from Natural Language Text. In H. Mouratidis & C. Rolland (Eds.), *Advanced Information Systems Engineering* (pp. 482–496). Springer Berlin Heidelberg.

- Sànchez-Ferreres, J., van der Aa, H., Carmona, J., & Padró, L. (2018). Aligning textual and model-based process descriptions. *Data & Knowledge Engineering, 118*, 25–40. https://doi.org/10.1016/j.datak.2018.09.001
