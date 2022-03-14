# mediapipe_portrait_segmentation


## USE

```bash
bazel build -c opt --define MEDIAPIPE_DISABLE_GPU=1 mediapipe/examples/desktop/portrait_segmentation:portrait_segmentation_cpu

LOG_logtostderr=1 bazel-bin/mediapipe/examples/desktop/portrait_segmentation/portrait_segmentation_cpu \
  --calculator_graph_config_file=mediapipe/graphs/portrait_segmentation/desktop_live.pbtxt
```