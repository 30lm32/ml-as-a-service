|__Problem__|__Data__|__Methods__|__Libs__|__Link__|
|-|-|-|-|-|
|`ML Service`|Randomly Generated|`Random Forest Classifier`|`Flask`, `Docker`, `Redis`, `Sklearn`|https://github.com/erdiolmezogullari/ml-dockerized-microservice|

In this project, a `ML based micro-service` was developed on top of `REST` and `Docker` after building a machine learning model by performing `Random Forest`

We used `docker-compose` to launch the micro services, below.

    1.Jupyter Notebook,
    2.Restful Comm. (Flask),
    3.Redis

After we created three different container, our MLasS would be ready.

You can use simple shell scripts (predict.sh, predict_random.sh)

predict.sh: It is sending features to our service and receiving response.
predict_random.sh: It is picking a row over validation set, randomly and then testing it our ML model under resources directory

Under resources directory, you can find our final pickle files, and cleaned csv files.

To take a look at data processing stage, you can go to directly notebook/code/model.ipynb file, or
You can open it on your browser using the ip address (http://localhost:8888/?token=<token>) of notebook.

Please, note that you need to replace <token> field with your specific token you have in the address.
