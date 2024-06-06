# wing-waves
Bird song identification based on audio (.wav) files

### Team Members:
- [Max](https://github.com/midniteclub)
- [Joseph](https://github.com/binaryplatitude)
- [Jonathan](https://github.com/Nemo5a7)

### Project Overview:
This project focuses on the identification of bird songs using data from Kaggle and Xeno-Canto. By converting audio files into spectrograms, we explore the potential of Convolutional Neural Networks (CNNs) for accurate classification of bird species based on their songs. This approach aims to enhance ornithological research and bird conservation efforts.

### Data Acquisition:
- **Sources:** Kaggle, Xeno-Canto
- **Details:** The dataset comprises recordings of 264 different bird species along with metadata such as species data, contributor, length of recording, bit rate, lat/long coordinates, self-reported recording location, date of recording, etc.
- **Kaggle:**
  - https://www.kaggle.com/datasets/rohanrao/xeno-canto-bird-recordings-extended-a-m
  - https://www.kaggle.com/datasets/rohanrao/xeno-canto-bird-recordings-extended-n-z
- **Size:** 29GB across two subsets (species A-M and N-Z)
- **Challenges:** No known issues during acquisition; however, weekly updates to the original dataset on Xeno-Canto may introduce changes not reflected in our static Kaggle dataset.

### Pre-Processing:
- Conversion of audio files into spectrograms to transform the problem from audio classification to image classification.
- Filtering techniques tested: pre-emphasis, spectral subtraction, and median filtering.
- Handling of missing data via imputation and amputation.
- Addressing noise, sparsity, and variability within species in the dataset.

### Exploratory Data Analytics:
- Analysis of numerical and categorical features.
- Identification and treatment of outliers.
- Feature engineering and creation of spectrograms for further analysis.

### Model Development:
- **Primary Model:** Convolutional Neural Network (CNN) for its ability to automatically learn and identify complex patterns in visual data.
- **Other Considered Architectures:** Recurrent Neural Networks (RNNs) and Long Short-Term Memory Networks (LSTMs) for sequential data, traditional machine learning algorithms on MFCC features.

### Future Directions:
- Investigating weighting audio samples based on community ratings.
- Exploring advanced filtering and signal isolation techniques.
- Further refining models for better performance.

### References:
- Boucher, N. J. (2014). SoundID version 2.0. 0 documentation.
- Verteletskaya, E., & Simak, B. (2011). Noise Reduction Based on Modified Spectral Subtraction Method. IAENG International Journal of Computer Science.
- López-Espejo, I., Joglekar, A., Peinado, A. M., & Jensen, J. (2024). On Speech Pre-emphasis as a Simple and Inexpensive Method to Boost Speech Enhancement.
- Kahl, S., et al. (2023). Overview of BirdCLEF 2023: Automated Bird Species Identification in Eastern Africa.
- Katz, J., Hafner, S. D., & Donovan, T. (2016). Assessment of error rates in acoustic monitoring with the R Package Monitor.
- Potamitis, I. (2014). Automatic classification of a taxon-rich community recorded in the wild.
- Priyadarshani, N., et al. (2016). Birdsong denoising using wavelets.
- Rao, R. (n.d.). Xeno-canto bird recordings extended [A-M].
- Rao, R. (n.d.). Xeno-canto bird recordings extended [N-Z].
- Schrama, T., et al. (2007). Automated monitoring of avian flight calls during nocturnal migration.
- Stoudt, S., Goldstein, B. R., & de Valpine, P. (2022). Identifying engaging bird species and traits with community science observations.
- Wildlife Acoustics (2011). Song Scope bioacoustics software version 4.0 documentation.

## License
This project is licensed under the CC0-1.0 License. See the [LICENSE](LICENSE) file for details.
