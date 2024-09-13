+------------------------+------------------------+
| Electrical Resistance Tomography Reconstruction |
+------------------------+------------------------+

    1. Dataset
        * data_Sen_Mesh
            * Sensitivity = (208, 812)
            * Mesh = (812, 2)
            * IDX_NUM = (812, 1)
            * Mesh_SQ = (1024, 2)

        * Ten Groups
            -> traineu = (37011 simulations, 812 voltage measurements per map)
            -> trainec = (37011 simulations, 208 elements per map)
            -> testeu  = (4111 simulations, 812 voltage measurements per map)
            -> testec  = (4111 simulations, 208 elements per map)

    2. Preprocessing
        * Standard Scaling

    3. Reconstruction
        * ConvRNN (Hybrid of Conv1D and BiLSTM) With FireFly Optimization

    4. Evaluation
        * Relative Image Error (Minimum, Maximum, Average)
        * Image Correlation Coefficient (Minimum, Maximum, Average)
