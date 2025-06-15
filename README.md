# Soil_quality_testing_model
**Overview**
 This project implements a Random Forest Classifier to predict soil quality ("Poor," "Moderate," or "Good") based on 16 soil properties. It also provides reasons for the predicted quality and actionable recommendations to improve soil health. The model was trained on a dataset of 4000 soil samples, addressing class imbalance using SMOTE to ensure fair predictions across all quality levels.
 
**Features**
1.Prediction: Classifies soil quality into "Poor," "Moderate," or "Good."
2.Explanatory Output: Identifies reasons for the classification (e.g., "Low nitrogen") and suggests   improvements (e.g., "Apply nitrogen fertilizer").
3.Balanced Model: Handles class imbalance using SMOTE for better performance on minority classes.
4.Feature Importance: Highlights key soil properties influencing predictions (e.g., pH, organic matter).

**Example Input:**
  The model takes 16 numerical soil features
   ("Sand %": 58.0, "Clay %": 20.0, "Silt %": 22.0, "pH": 7.7, "EC mS/cm": 0.4,
    "O.M. %": 0.7, "CACO3 %": 6.0, "N_NO3 ppm": 4.2, "P ppm": 6.3, "K ppm": 116.0,
    "Mg ppm": 986.0, "Fe ppm": 12.5, "Zn ppm": 0.6, "Mn ppm": 12.5, "Cu ppm": 0.9,
    "B ppm": 0.2)
    
   **Output**
     The model outputs:
     Soil Quality: "Poor," "Moderate," or "Good."
     Reasons: List of issues (e.g., "Low organic matter").
     Recommendations: List of solutions (e.g., "Add compost").
    **Example Output:**
    Soil Quality: Poor
    Reasons: ['Low organic matter', 'Nitrogen deficiency']
    Recommendations: ['Add compost or manure', 'Apply nitrogen fertilizer']
