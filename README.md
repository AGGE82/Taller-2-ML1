# Taller-2-ML1
# Juan David Sanchez y Alejandro Gil
Random Forest, SVM, Decision Tree &amp; kNN comparison


What happens to the performance of kNN and SVM if you skip the feature scaling step?

Se logró evidenciar que con feature scaling el rendimiento mejora, en el caso de diabetes svm dio 0.74 y svm_scaler 0.78.

Which model was the fastest to train?

Decision tree, para iris.csv demoró 0.05s, mientras que kNN demoró 0.06s, SVM 0.07s y Random Forest 0.22s.
Para cancer.csv, Decision tree tardó 0.04s, kNN demoró 0.05s, SVM 0.05s y Random Forest 0.16s.
Y por último para diabetes.csv, Decision tree demoró 0.04s, kNN 0.06s, SVM 0.10s y Random Forest 0.15s.
En total el modelo más rápido fue Decision Tree y el

Did the "out-of-the-box" Random Forest perform well compared to the others?

Tuvo un rendimiento muy bueno, casi igual a los de los demás con un accuracy de 0.9737 para iris.csv, para cancer.csv 0.97 y para diabetes.csv 0.77, para este último tuvo una mejor en comparación con decision tree que dio un accuracy de 0.71.

How much did changing the hyperparameters of SVM and kNN affect their performance?

Al realizar pruebas cambiando los hiperparametros manejados tanto en SVM como en kNN se llego a las siguientes conclusiones: El peor hiperparámetro para SVM para todos los datasets es kernel=rbf y C=0.1. Para kNN en iris.csv no se evidencia diferencia entre los hiperparámetros, mientras que para cancer.csv y diabetes.csv el mejor hiperparametro es k=7. En SVM en iris.csv casi todos los hiperparametros son buenos, para cancer.csv el mejor es kernel=linear y C=0.1, mientras que para diabetes.csv es mejor kernel=rbf y C=1.

Look at the classification report. Are all classes predicted equally well by your best model?

No todos las classes son predecidas de la misma forma, y en especial ocurre la peculariedad que el classification report presento muy bajos rendimientos al trabajar con feature scaling. Los resultados tendieron a ser consistentes, en el caso de iris.csv por el tamaño del dataset daba un desempeño de casi siempre 1, para cancer.csv el mejor modelo fue Random Forest con 0.97 de desempeño, y para diabetes.csv el mejor modelo fue SVM con un desempeño del 0.86.
