

This repository is built directly on top of the **Official Implementation of "[Comparative Study on Performance of ML Models for Fall Detection in Older People](https://doi.org/10.20944/preprints202312.2027.v1)"**
- Link to the original repo: [Fall-Detection-System](https://github.com/mojtabaSefidi/Fall-Detection-System)
  
# Fall Detection With Transformer
- The results shows that Transformers beat all existing traditional and deep learning baselines in the original repository in terms of accuracy and f1 score.
![image](https://github.com/user-attachments/assets/dffadf7d-1a13-4201-81f3-11cfd94d91bc)
- Moreover the Transformer is only has a fraction of the number of parameters with comparable training times.
![image](https://github.com/user-attachments/assets/371f4928-4b00-4743-ab11-1a84839f6aa9)
- The Transformer also converged withiin 1/2 epochs, which is much quicker than existing deep learning models (~ 5 epochs).
![image](https://github.com/user-attachments/assets/d2ac78a0-7300-4664-8e13-62574d502e59)
![image](https://github.com/user-attachments/assets/1ab4285e-f0ee-43da-86d8-858a6bf82b66)

## How to Run

1. Install the required libraries from the `requirements.txt` file:
   ```
   !pip install -r requirements.txt
   ```
2. Download the dataset.
3. Open `Main.ipynb`.
4. Adjust the variables (e.g., relative paths).
5. Run the notebook cells.

## How to Access the Dataset

1. **SisFall Dataset:**
   ```
   !gdown -q 1-E-TLd5_J-DDWZXkuYL-moMpoezlMn4Z
   ```
2. **SisFall Enhanced Dataset (Labels):**
   ```
   !gdown -q 1gvOuxPc8dNgTnxuvPcVuCKifOf98-TV0
   ```

## Implementation Details

#### `data_processor.py`
* **Objective:** Process the dataset and convert it into time-series format.
* **Input:** SisFall dataset.
* **Output:** `X_train`, `y_train`, `X_test`, `y_test`.

#### `deep_models.py`
* **Objective:** Implementation and evaluation of deep learning models.
* **Output:** Separate dictionaries containing results and predictions.

#### `traditional_models.py`
* **Objective:** Implementation and evaluation of traditional machine learning models.
* **Output:** Separate dictionaries containing results and predictions.

#### `utils.py`
* **Objective:** Collection of utility functions used throughout the project.

#### `Main.ipynb`
* **Main Interface:** Provides the main interface for the project.
* **Output:** A data frame with detailed results.

### Citation
For more details, you can read the original publicly available paper:

```
@article{EsfahaniFallDetection2023,
  title={Comparative Study on Performance of ML Models for Fall Detection in Older People},
  author={Mohammadali Sefidi Esfahani and Mohammad Fattahian},
  journal={Preprints.org},
  year={2023},
  doi={https://doi.org/10.20944/preprints202312.2027.v1}
}
```
