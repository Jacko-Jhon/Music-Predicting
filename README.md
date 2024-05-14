### Our Work

    First of all, we randomly selected 200 samples from the **dataset** - [Spotify Dataset 1921-2020, 600k+ Tracks]([Spotify Dataset 1921-2020, 600k+ Tracks (kaggle.com)](https://www.kaggle.com/datasets/yamaerenay/spotify-dataset-19212020-600k-tracks/data)) .

    And, what we did is to download those songs manually and analyze the Mel Spectrogram, than, tranfer them to 100-dimensional vectors. Later we used the vectors to train three models to predict the "popularity" defined in the **dataset**. However, due to the small amount of data, the regression models do not perform well. Next, we define a variable $x$ only to indicate whether the song is popular or not.

$$
x = 
\begin{cases}
1,\ if\ popularity\ is\ in\ top\ 25\% \\
0,\ else\\
\end{cases}
$$

    Than we used the new data to train three binary classification models - Sequential neural network, DTree and Random forest. And we got  some results.

* We tried to use PCA to reduce dimensionality, but the effect was not good, so we won’t describe it further.


