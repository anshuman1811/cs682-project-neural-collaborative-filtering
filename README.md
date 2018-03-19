# neural-collaborative-filtering
Neural collaborative filtering(NCF), is a deep learning based framework for making recommendations. The key idea is to learn the user-item interaction using neural networks. Check the follwing paper for details about NCF.

> He, Xiangnan, et al. "Neural collaborative filtering." Proceedings of the 26th International Conference on World Wide Web. International World Wide Web Conferences Steering Committee, 2017.

The authors of NCF actually published [a nice implementation](https://github.com/hexiangnan/neural_collaborative_filtering) written in tensorflow(keras). This repo instead provides my implementation written in **pytorch**. I hope it would be helpful to pytorch fans. Have fun playing with it !

## Dataset
[The Movielens 1M Dataset](http://grouplens.org/datasets/movielens/1m/) are used to test the repo.

## Files

> `data.py`: prepare train/test dataset
> `utils.py`: some handy functions for model training etc.
> `metrics.py`: evaluation metrics including hit ratio(HR) and NDCG
> `gmf.py`: generalized matrix factorization model
> `mlp.py`: multi-layer perceptron model
> `neumf.py`: fusion of gmf and mlp
> `engine.py`: training engine
> `training.py`: entry point for train a NCF model


## TODO
- pretraining of NeuMF
- Convergence curve