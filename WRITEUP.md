## Privacy Preserving: Incremental Diversity Algorithm for Multiple Sensitive Attributes in Medical Domain

### **Problem Statement**

Existing anonymization techniques either suffer from excessive information loss or fail to effectively handle multiple sensitive attributes in datasets. The challenge is to develop a privacy-preserving model that efficiently anonymizes microdata while maintaining its usability for analysis. Key issues include:

- Balancing anonymity with data utility.
- Handling multiple sensitive attributes effectively.
- Reducing information loss while ensuring strong privacy guarantees.

### **Introduction**

Privacy preservation in data publishing is a critical challenge in modern computing, particularly in sectors such as healthcare and finance, where sensitive attributes must be protected. Traditional anonymization methods like k-anonymity and l-diversity provide privacy guarantees but often lead to increased residue records or reduced data utility. The **Incremental Diversity Algorithm** aims to address these issues by introducing a novel approach that optimizes the balance between diversity and residue records. This report details the development, implementation, and performance evaluation of this new approach.

### **Objectives**

The main objectives of this project include:

- Developing an effective anonymization framework that incorporates **k-anonymity, l-diversity, and Anatomy models**.
- Minimizing **information loss** while ensuring **strong privacy protection**.
- Implementing **efficient handling of multiple sensitive attributes** to enhance dataset security.
- Providing **experimental evaluations** and comparisons with existing methods to demonstrate the effectiveness of the proposed algorithm.

### **Methodology**

The **Incremental Diversity Algorithm** follows a structured approach to enhance privacy while maintaining dataset utility:

1. **Data Standardization**: The microdata table is stored using nested dictionaries to ensure efficient data handling.
2. **Equivalence Class Formation**: A unique group ID is assigned to each record based on a formula ensuring diversity.
3. **Incremental Diversity Processing**: Five different algorithms are evaluated to balance privacy and diversity effectively.
4. **Quasi-Identifier and Sensitive Table Formation**: Data is split into separate tables (QIT and ST) following the **Anatomy model** to improve security.
5. **Masking and Generalization**: Attributes like age, gender, and ZIP codes are masked using predefined transformation formulas.
6. **Performance Evaluation**: Metrics such as **residue percentage, diversity percentage, and execution time** are measured for varying dataset sizes and values of **k**.

### **Results**

The experimental evaluation of the Incremental Diversity Algorithm yielded the following key observations:

- **Residue Percentage**: The algorithm significantly reduced the number of residue records compared to **l, e-diversity** methods.
- **Execution Time**: The algorithm demonstrated improved time complexity, outperforming traditional **l, e-diversity** models in handling large datasets.
- **Diversity**: While ensuring strong privacy, the method led to slightly lower diversity in some cases due to its optimization for residue minimization.
- **Best Algorithm Selection**: The **Disease Semantic Algorithm** (based on unique parents in a hierarchical structure) was found to be the most effective in balancing diversity and residue records.

### **Conclusion**

The **Incremental Diversity Algorithm** presents a **robust and efficient solution** for preserving privacy in datasets with multiple sensitive attributes. By leveraging an optimized balance between **data diversity and residue minimization**, it outperforms traditional anonymization techniques in terms of **efficiency, security, and usability**. Future enhancements could focus on:

- **Automated sensitive attribute selection** for better adaptability.
- **Machine learning integration** to dynamically adjust privacy settings.
- **Scalability improvements** to support real-time anonymization of large datasets.
- **Real-world validation** across various industries such as healthcare, defense, and finance.

This research demonstrates that the **Incremental Diversity Algorithm** is a **viable alternative** for privacy-preserving data publishing, paving the way for future advancements in secure data handling.
