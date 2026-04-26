Advanced Customizations in Deep Learning & Neural Networks

CMPE 258 graduate assignment exploring regularization, generalization, multi-modal data augmentation, and advanced Keras/PyTorch customization, with experiment tracking in TensorBoard and Weights & Biases.

Quick Links





All executed Colabs (Google Drive): Drive Folder

Notebooks, Topics, and Video Walkthroughs







#



Notebook



Topics



Video





01



01_regularization_tensorflow.ipynb



TF regularization: L1/L2, dropout, MC dropout, early stop, initializers, batch norm, callbacks, TensorBoard, Keras Tuner



Video 1





02



02_regularization_pytorch.ipynb



PyTorch parity of notebook 01 + Optuna + TensorBoard



Video 2





03



03_kerascv_data_augmentation.ipynb



KerasCV augmenters and policy-based augmentation on tf_flowers



Video 3





04



04_augmentation_image_video_docimg.ipynb



AugLy for image/video, Augraphy for document images



Video 4





05



05_augmentation_text_timeseries_tabular_speech.ipynb



Text, timeseries, tabular, and speech augmentation



Video 5





06



06_keras_custom_training_components.ipynb



One-cycle scheduler, MCAlphaDropout, MaxNormDense, TensorBoard



Video 6





07



07_keras_custom_loss_metrics_functions.ipynb



Custom Huber loss/function family and custom metric



Video 7





08



08_keras_custom_layers_and_model.ipynb



Custom layers and subclassed residual model



Video 8





09



09_keras_custom_optimizer_and_training_loop.ipynb



Custom optimizer + GradientTape loop + tf.function speedup



Video 9





10



10_pytorch_advanced_and_wandb.ipynb



Advanced PyTorch custom constructs + W&B tracking



Video 10

Repository Structure

advanced_dl_customizations/
├── notebooks/         # 10 assignment notebooks
├── videos/            # narration scripts and video link helper files
├── assets/            # small generated/downloaded assets used in demos
├── requirements.txt   # pinned package versions
└── README.md

Run Locally

Each notebook is self-contained, but you can also run from this repo:

git clone https://github.com/<your-username>/advanced_dl_customizations.git
cd advanced_dl_customizations
pip install -r requirements.txt
jupyter lab notebooks/

Key Takeaways

Across all 10 notebooks, the core result is that generalization is best treated as a system of coordinated choices rather than one isolated trick. Regularization, normalization, early stopping, augmentation, and scheduling each constrain a different failure mode.

The multi-modal augmentation notebooks show that invariances are modality-specific: image, text, timeseries, tabular, and speech each need different perturbation strategies to preserve semantics while improving robustness.

The advanced Keras and PyTorch notebooks demonstrate how to move from API usage to mechanism-level understanding by implementing custom losses, metrics, layers, models, optimizers, schedulers, and training loops directly.

Library Versions





tensorflow==2.16.1



keras==3.3.3



keras-cv==0.9.0



keras-tuner==1.4.7



torch==2.3.0



torchvision==0.18.0



wandb==0.17.0



augly==1.0.0



augraphy==8.2.6



nlpaug==1.1.11



tsaug==0.2.1



imbalanced-learn==0.12.3



audiomentations==0.35.0



optuna==3.6.1



tensorflow-datasets==4.9.4

Acknowledgement

This work draws conceptually from Aurélien Géron's Hands-On Machine Learning (3rd ed.), while using original code structure, notebook flow, and explanations for this assignment.
