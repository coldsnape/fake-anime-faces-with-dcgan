# Fake Anime Faces With DCGAN
By Danh Nguyen and Jared Mlekush

# Overview
- Data
- Methods
- Pros & Cons
- Something we can try

# Data 
Our clean data is just under 400mb, consisting of over 63,000 faces
Data can be found here on Kaggle: https://www.kaggle.com/splcher/animefacedataset
Images’ size ~ 64 x 64 

# Methods
We found an implementation very similar to how we had envisioned our project so we recreated the project to learn from it. Source: https://github.com/braindotai/Fake-Anime-using-DCGAN-Pytorch

We also tried additional approaches to improve the generator and discriminator models:
- Used different lost Functions
- Fine tuned learning rates
    - One uniform rate
    - Different rates for D(x) vs. G(x)
- Tried different transformations

# Pros
- The implemented based model is quite effective at generating unique anime faces out the box. It included some of the industry best practices such as adding random noise to generator and disriminator to enhancing learning capabilities. 

# Cons
- We still experienced mode collapse
- Some of the generated anime faces are unproportional, especially the eyes which are generally large compare to the actual face
- High GPU computation cost

# Something we can try
- Adding additional layers
- Try different loss functions
- Trying additional combinations of image augmentations 
- More images/higher quality images



