# mediapipePose

```

load("//mediapipe/java/com/google/mediapipe:mediapipe_aar.bzl", "mediapipe_aar")

mediapipe_aar(
    name = "mediapipe_pose_tracking",
    calculators = ["//mediapipe/graphs/pose_tracking:pose_tracking_gpu_deps"],
)

```

```
bazel build -c opt --config=android_arm64  mediapipe/examples/android/src/java/com/google/mediapipe/apps/build_aar_pose:mediapipe_pose_tracking
```

```
bazel build -c opt mediapipe/graphs/pose_tracking:pose_tracking_gpu_binary_graph
```

```
open bazel-bin/mediapipe/graphs/pose_tracking/
mediapipe/modules/
```