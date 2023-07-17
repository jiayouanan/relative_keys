# relative_keys

This is a preliminary relative keys code for reference.

Firstly, the following packages are necessary:
```
numpy 1.20.3
pandas 2.0.1
scikit-learn 0.24.2
xgboost 1.7.1
redis 4.6.0
```

We provided a briefly processed dataset to put in `data_process` folder.

### 1 Train xgboost and get other necessary information.

```
python preprocess.py
```

With the trained model and the inference set, we can test the algorithm. Make sure the corresponding folder exists.

### 2.1 test srk
```
python main_srk.py
```

### 2.2 test osrk
```
python main_osrk.py
```

### 2.3 test ssrk
```
python main_ssrk.py
```

### 2.4 test dynamic performance
```
python main_dynamic_nosignal.py
```

### 2.5 test the effectiveness of monitoring ML performance
```
python main_indicator.py
```

We have also developed a very simple interface `redis_inter.py` to redis to receive data from redis. 
Make sure the redis server is turned on.
