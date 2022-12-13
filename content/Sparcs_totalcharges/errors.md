## Error for Ensemble

Input contains NaN, infinity or a value too large for dtype('float64').
Traceback (most recent call last):
  File "/usr/local/lib/python3.8/dist-packages/supervised/base_automl.py", line 1083, in _fit
    trained = self.ensemble_step(
  File "/usr/local/lib/python3.8/dist-packages/supervised/base_automl.py", line 401, in ensemble_step
    self.ensemble.fit(oofs, target, sample_weight)
  File "/usr/local/lib/python3.8/dist-packages/supervised/ensemble.py", line 236, in fit
    score = self.metric(y, y_ens, sample_weight)
  File "/usr/local/lib/python3.8/dist-packages/supervised/utils/metric.py", line 408, in __call__
    return self.metric(y_true, y_predicted, sample_weight=sample_weight)
  File "/usr/local/lib/python3.8/dist-packages/supervised/utils/metric.py", line 30, in rmse
    val = mean_squared_error(y_true, y_predicted, sample_weight=sample_weight)
  File "/usr/local/lib/python3.8/dist-packages/sklearn/metrics/_regression.py", line 438, in mean_squared_error
    y_type, y_true, y_pred, multioutput = _check_reg_targets(
  File "/usr/local/lib/python3.8/dist-packages/sklearn/metrics/_regression.py", line 96, in _check_reg_targets
    y_pred = check_array(y_pred, ensure_2d=False, dtype=dtype)
  File "/usr/local/lib/python3.8/dist-packages/sklearn/utils/validation.py", line 800, in check_array
    _assert_all_finite(array, allow_nan=force_all_finite == "allow-nan")
  File "/usr/local/lib/python3.8/dist-packages/sklearn/utils/validation.py", line 114, in _assert_all_finite
    raise ValueError(
ValueError: Input contains NaN, infinity or a value too large for dtype('float64').


Please set a GitHub issue with above error message at: https://github.com/mljar/mljar-supervised/issues/new

