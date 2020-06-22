---
name: can't pridict
about:code:   regressor = ak.StructuredDataRegressor(max_trials=1,)
              regressor.fit(train_x,train_y)
              model = regressor.export_model()
              predicted_y = model.predict(test_x)

---

### Bug Description
tensorflow.python.framework.errors_impl.UnimplementedError:  Cast double to string is not supported

### Bug Reproduction
              regressor = ak.StructuredDataRegressor(max_trials=1)
              regressor.fit(train_x,train_y)
              model = regressor.export_model()
              predicted_y = model.predict(test_x)

Data used by the code:
2020/6/22
### Expected Behavior

load model  and  can predict,thank you!

### Setup Details
Include the details about the versions of:

 - tensorflow:

### Additional context
<!---
If applicable, add any other context about the problem.
-->
