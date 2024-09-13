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
    * Sparse constraints for stacked encoder With shuffled shepherd Optimization

4. Evaluation
    * Relative Image Error (Minimum, Maximum, Average), root mean square error
    * Image Correlation Coefficient (Minimum, Maximum, Average), structural similarity index
